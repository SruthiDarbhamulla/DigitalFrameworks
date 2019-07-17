# Digital Frameworks Assignment 3

_by Sruthi Darbhamulla_

## Description of dataset:
This dataset was downloaded from the Federal Election Commission’s website (available [here](https://www.fec.gov/data/independent-expenditures/?data_type=processed&is_notice=true))      

It is campaign finance data pertaining to independent expenditures by specific spenders for particular candidates. It includes addresses of each, amounts, dates of expenditure, party affiliation of candidate and a host of other parameters. 

## What it can be used for: 
It would be interesting to understand which committee is contributing to what candidate/s and how it aligns with their policy or business goals. Similar data can be obtained for several years and analyzed to see if there are any interesting trends or deviations in the contributions. If there are interesting divergences, such as the same committee donating to both Democratic and Republican candidates, that might make for an interesting story too. 

## Steps undertaken to clean data: 
* Separated the date and time in the expenditure date column by 
    * Changing cell format to date in one column and time in the other 
    * Using the formula =int(original cell) in Cell 1
    * Using the formula =Cell 1-original cell in Cell 2

* Combined the two address columns using the formula =address cell1 &" "&address cell2

* Sorted the committee name in reverse alphabetical order (since alphabetical order yielded names with numbers first, a bit confusing visually) 

* Inserted filters for all the fields, particularly useful for committee names, report year, and candidate name 

## Issues that need to be fixed: 
* Something is off with the zip code column. Not sure how the error got introduced or how to fix it. 
* Not sure how to clean other date and time columns, where information is filled in only for some transactions.

