# **Election Result Analysis**

## **Project Overview** 
A Colorado Board of Elections employee wanted us to do an analysis of election results for submission of election results by doing the election audit of a recent local congressional election. 

To complete the audit, we were provided a list of outcomes that our analysis should be able to provide. The election commission was already aware that the desired tasks could be completed using Microsoft Excel. But manager of employee wanted us to automate the process of audit through our analysis using Python. 

### Purpose:
For the fulfillment of election commission’s project requirement, we were required to create a script using Python programming language which could perform the following for the audit and analysis of the election results:

1.  Calculate the total number of votes cast.
2.  Calculate the number of votes cast in each county and the percentage of total votes for each county in the precinct
3.  Determine name of the county which had the largest number of votes 
4.  Calculate the number of votes and percentage of total votes received by each candidate 
5. Determine the winner of the election based on popular vote.

### Resources:

* Data Source: election_results.csv (Input file which will be read by our Python program script to determine the required information)
* Software Used: Python 3.7.6, Visual Studio Code, 1.51.0
* Starter file: PyPoll_Challenge_starter_code.py (Starter Python Script file for the module challenge completion which is renamed as **PyPoll_Challenge.py** as the final solution script for this challenge)
* Output file: election_results.txt (The results will automatically be written and saved to this text file when we run our Python script)

** Also, the results will be displayed on the terminal on which final Python script 'PyPoll_Challenge.py' is run, i.e. Command prompt (as required by module challenge) 

## **Election-Audit Results**

The analysis of the election show that:

* There were "***369,711***" votes cast in the election. 
    
    Below is the code snippet from Python script that helps in obtaining this total vote count for entire election. This snippet shows the opening of input file in the read mode, reading the header row and storing it in a separate header variable. From the next row, starting the row count for total votes and saving it, for each row, under a repetition statement of 'for'.

    ![Total_Vote_Code_Snippet](https://github.com/kirtibhandari/Election_Analysis/blob/main/Resources/Vote_count.png)


* There were three counties as listed below depicted below with their results:
  - **Jefferson**: 
    - In Jefferson, “**38,855**” total votes were cast which were “**10.5%**” of the total votes 

  - **Denver**: 
    - In Denver, “**306,055**” total votes were cast which were “**82.8%**” of the total votes

  - **Arapahoe**:
    - In Arapahoe, “**24,801**” total votes were cast which were “**6.7%**” of the total votes

    Below code snippet helps in fetching out total votes in each county and percentage of votes for each county, out of total '369,711' votes cast in election.

    ![Code_Snippet_County](https://github.com/kirtibhandari/Election_Analysis/blob/main/Resources/Code_Snippet_County.png)
 
* **County** that had largest number of votes cast: **Denver**

    Below is the code snippet through which we find out which county had maximum number of votes cast and prints it to the terminal:

    ![Winning_County_Code_Snippet](https://github.com/kirtibhandari/Election_Analysis/blob/main/Resources/Winning_County.png)

* There were three candidates as presented below with their results:
    - **Charles Casper Stockham**
: Received "**23.0%**" of the vote and "**85,213**" number of votes.
    - **Diana DeGette**
: Received "**73.8%**" of the vote and "**272,892**" number of votes.
    - **Raymon Anthony Doane**
: Received "**3.1%**" of the vote and "**11,606**" number of votes.

        Here we present code snippet screenshot that helped in extracting total votes for each candidate as well as percentage of their votes out of total votes in election which prints the results on the terminal as well.

        ![Code_Snippet_Candidate](https://github.com/kirtibhandari/Election_Analysis/blob/main/Resources/Code_Snippet_Candidate.png)

* The **winner** of the election was:
    - ***Diana DeGette***, who received "**73.8%**" of the vote and "**272,892**" number of votes.

    Last, but not least, here we use the follwong code in the script to find out who is the winner of the election, along with candidate's total number and percentage of votes for the winning candidate, printing at the terminal.

    ![Winning_Candiate_Code_Screenshot](https://github.com/kirtibhandari/Election_Analysis/blob/main/Resources/Winning_Candidate.png)

## Deliverable 1 requirement:
When the PyPoll_Challenge.py script is run on Command prompt, the required outcomes gets printed on the terminal as below:

#### Command_Prompt_Results Screenshot

![Command_Prompt_Results_Screenshot](https://github.com/kirtibhandari/Election_Analysis/blob/main/Resources/Command_Prompt_Output.png)

After writing and saving the ouput to 'election_results.txt' file, following output was obtained in the this output file as required in this module challenge.

## Deliverable 2 requirement:
#### Election_Results.Txt Screenshot  

![Election_Results_Text_File_Output](https://github.com/kirtibhandari/Election_Analysis/blob/main/Resources/Election_Results_Txt_Screenshot.png)


## **Election-Audit Summary**
The current Python script is being used to obtain the information about the total votes cast and percentage of votes, out of total, for each county, and total votes received and percentage of votes, out of total, received by each candidate. This script can be modified to obtain more outcomes some of which are as follows:

If election commission is interested, we want to submit our proposal to enhance the analysis script so that it can also be used for the following:

1.	If we are provided with election results for other the Congressional Precincts, we can use the script to obtain results for all the other congressional Precincts as well.

2.	In addition, we can enhance the script to find out the Senatorial districts’ election results and local elections’ results as well, for the entire country.

3.	The current script can also be modified to provide information about most preferred method of voting out of the three methods namely ‘Mail-in-Ballot’, ‘Punch-Cards’ and ‘Direct Recording Electronic’. This information can be helpful in deciding preferred method of voting by country people. This method can be used to facilitate voting in future elections in other counties and districts to increase the participation of voters. The higher the number of votes cast, the fairer the election results will be and hence, the most popular leader will win.

