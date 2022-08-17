# Election-Analysis

## Project Overview
A Coloarado Board of Elections employee has given you the following tasks to complete the election audit of a recent local congressional election.

1. Calculate the total number of votes cast.
2. Get a complete list of candidates who received votes.
3. Calculate the total number of votes each candidate won.
4. Calculate the percentage of votes each candidate won.
5. Determine the winner of the election based on popular vote.

## Resources
- Data Source: election_results.csv
- Software: Python 3.6.1, Visual Studio Code, 1.38.1

## Challenge Overview

The Colorado Board also wants to expand the analysis to cover the voter turnout in each county, the percentage of votes from each county out of the total count, and the county with the highest turnout. These results will be printed to the terminal as well as saved in a text file. 

## Election Audit Results

This analysis shows that:

* There were 369,711 votes cast in the election

* Breakdown of the vote count and percentages for each county:
  * Jefferson: 10.5% (Total Votes: 38,855)
  * Denver: 82.8% (Total Votes: 306,055)
  * Arapahoe: 6.7% (Total Votes: 24,801
  
* Denver is the county with the largest voter turnout

* The candidates and their results:
  * Charles Casper Stockham: 23.0% (TOtal Votes: 85,213)
  * Diana DeGette: 73.8% (Total Votes: 272,892)
  * Raymon Anthony Doane: 3.1% (Total Votes: 11,606)
  
* The winner of the election was:
  * Diana DeGette: 73.8% (Total Votes: 272,892)

### Important Pieces of Code Used in Analysis

  * For this analysis, the "with open" python function was utilized to open the election results data (as shown below) for the analysis and then to open the text file  where the results were written. 
  
![With_Open.png](/Resources/With_Open.png)

  * This "for loop" python function was utilized to get the number of votes for each county as well as calculate the percentage of votes for each county. This code was repeated to obtain the results for the number of candidate votes and their percentage of the total vote. The last line (txtfile.write(county_results)) is the code to write the results to the text file.
  
![For_Loop_County_Votes.png](/Resources/For_Loop_County_Votes.png)

 * This "if" statement was used to compare the results of each county and determine which had the most votes and was therefore the winner. This same logic was used to determine the winning candidate.
 
 ![Winning_Percentage.png](/Resources/Winning_Percentage.png)


## Challenge Summary

This analysis has shown that Denver by far had the largest voter turnout of the counties and the winning candidate is Diana DeGette. This analysis also found the voter turnout for each county and the percentage of votes for each candidate. This code can be modified for future analysis of other elections or components of elections: it could easily be applied to state or presidential elections. It could be used to analyze different methods of voting (mail-in ballots versus in-person machines) or to analyze data of voting population using the same key python features (for loops, with open statements, if statements) but with some refactoring of the code.
