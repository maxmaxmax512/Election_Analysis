## Overview of Election Audit

The Election Commission has contracted with our firm to review all votes and validate the election results. They have asked us to analyze the data to identify several key elements, including:
* The voter turnout for each county
* The percentage of votes from each county out of the total count
* The county with the highest turnout

By auditing this data accurately, our firm can help ensure that the election was a fair democratic process and that the outcomes are an accurate representation of the voter's intent.

## Election Audit Results
The following elements represent a final audited and verified summary of the election results.

* How many votes were cast in this congressional election?
  * Total Votes: 369,711 
* What were the total number of votes and the percentage of total votes for each county in the precinct?
  * Jefferson: 10.5% (38,855)
  * Denver: 82.8% (306,055)
  * Arapahoe: 6.7% (24,801)
* Which county had the largest number of votes?
  * Denver county had the largest number of votes (306,055) by a margin of 267,200.
* What were the total number of votes and the percentage of the total votes each candidate received?
  * Charles Casper Stockham: 23.0% (85,213)
  * Diana DeGette: 73.8% (272,892)
  * Raymon Anthony Doane: 3.1% (11,606)
* Which candidate won the election, what was their vote count, and what was their percentage of the total votes?
  * Winner: Diana DeGette
  * Winning Vote Count: 272,892
  * Winning Percentage: 73.8%

## Election Audit Summary
Now that we have written this script, it could be easily modifying to audit any election. Specifically, we will only need to change the path for the file_to_load and the file_to_save depending on the election we are auditing. For example, during the midterm election we could change the code to instead read:
```py
# Assign a variable for the file to load and the path.
file_to_load = os.path.join("Resources", "midterm_results.csv")
# Assign a variable to save the file to a path.
file_to_save = os.path.join("Resources", "midterm_results.txt")
```
Alternatively, if we want to change the program in such a way that it can be run over any file, we could ask for a user input to identify the file name.
```py
# Assign a variable for the file to load and the path.
file_name = input("Please indicate the election file you would like to audit:")
file_to_load = os.path.join("Resources", file_name)
# Assign a variable to save the file to a path.
file_to_save = os.path.join("Resources", "election_results.txt")
```
