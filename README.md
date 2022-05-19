# stock-analysis

## Overview

The intention of this analysis is to view the overall stock performance for the years of 2017 and 2018. In order to do this, I created columns that organize worksheet with the ticker of the stock, its total daily volume and return. Afterwards, an array from 0 to 11 was created to correspond with the stock tickers in alphabetical order. This let me create a nested for loop to sort through the 2017 and 2018 worksheets in order to match the tickers to the total volume and return values. Within the nested loop, I also included conditional statements that would check the previous and following rows to see if the tickers would match which would determine whether the row was the starting or ending price, thus giving me the overall return of the stock for the given year (ending price / starting price -1). Finally, I formatted the return values to correspond to either red or green depending on whether the value was negative or positive. After creating the original code via the module instructions we were asked to refactor the code to run faster.

## Results

How I achieved Deliverable 1 was by creating a variable called "tickerIndex" which was used as a reference for the ticker array in the original code and was increased by 1 at the end of the loop so that it could begin sorting by the next ticker. By inserting the tickerIndex variable into the conditionals for the total volume and starting/ending prices I was able to sort through the entire 2017 and 2018 worksheets after a single pass. In contrast, the original code had to pass the worksheets once for each ticker which resulted in a slower run time.

## Summary

I do think that a significant benefit to refactoring code would be efficacy. For example, in the original code the analysis was doing a pass for every individual ticker whereas the same analysis could be achieved with a single pass. While this may not be very significant in an isolated instance, like this assignment, when industry code has so many analyses running simultaneously it's important to save resources when possible. I think a significant disadvantage would be the intuitiveness. I found this challenge to be extremely difficult given the module instructions that we were given and I wouldn't have thought to create the tickerIndex variable without help from my instructors. I definitely believe that refactoring code is important, however I think it really depends on whether the time and labor used to refactor the code is worth the time you save running it. Specific to the challenge, I think that an advantage would be the single pass as opposed to the multiple it took to run the original code. A disadvantage was the time it took to figure out a solution and reconceptualize the entire project. However, I do believe that this disadvantage diminishes over time with practice. 


