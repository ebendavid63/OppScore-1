# OppScore

Yet another R script for calculating opportunity scores and plotting the Opportunity Map / Landscape.

This one does not require anything beyond base R. A sampledata.csv file is included for testing purposes.

How to use:
1. Format your data as a CSV file. It should have at least 3 columns:
   _outcome_, _importance_ and _satisfaction_
   Alternatively, set the "threshold" parameter if your input scale is not the recommended 1-5*.
   _threshold_ should be your scale mid point. E.g., for the recommended 1-5 scale it would be 3. If your scale is 1-7, then it should be 4 and so on.
2. You can also customize the file names and column names to match those in your CSV file.
   The script will ignore any extra columns.
3. Run the whole script. Voila.

*_Note that this deviates from Ulwick's recommendation which is asking people for Importance and Satisfaction on a 1-5 scale._


Source:

> Ulwick, Anthony. [What customers want](https://www.amazon.com/What-Customers-Want-Outcome-Driven-Breakthrough/dp/0071408673). McGraw-Hill Professional Publishing, 2005.