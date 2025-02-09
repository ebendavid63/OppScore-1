﻿# OppScore

Yet another R script for calculating opportunity scores and plotting the Opportunity Map / Landscape.

__UPDATE: OppScore calculation was yielding wrong values! It's fixed now.__

This one does not require anything beyond base R. A sampledata.csv file is included for testing purposes.

How to use:
1. Format your data as a CSV file. It should have at least 3 columns: _outcome_, _importance_ and _satisfaction_. You can also customize the        file names and column names in the script to match those in your CSV file. Additional columns will be ignored.
3. Optionally, __if your input scale is not 1-5__, modify the _midpoint_ parameter in the script. It should be equal to the middle point of the scale. E.g., for a 1-5 scale _midpoint_ should be 3. If your scale is 1-7, then it should be 4 and so on.
4. Make sure the data and the script are in the same folder.
5. Run the whole script. Voila.

*_Values above the midpoint parameter (either importance or satisfaction) will be considered positive. This is an important consideration when computing the score. Note that using a scale other than 1-5 deviates from Ulwick's recommendation._

# References:

* Ulwick, Anthony. [What customers want](https://www.amazon.com/What-Customers-Want-Outcome-Driven-Breakthrough/dp/0071408673). McGraw-Hill Professional Publishing, 2005. _This is the main source for the Opportunity Score method._
* [Function to round numbers in data frame that contains non numeric data](http://jeromyanglim.tumblr.com/post/50228877196/round-numbers-in-data-frame-that-contains-non) by Jeromy Anglim.
