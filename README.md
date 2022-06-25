# VBA Challenge Stock Analysis

## Overview of Project
The purpose of this analysis is to compare the stock performances between the years of 2017 and 2018. Also we need to find the advantages and dis-advantages to refactoring the All Stock Analysis code in order to anaylaze the data.

## Results

![image](https://user-images.githubusercontent.com/106887052/175757819-feb99cd1-4e67-472b-ab9c-8f561fe8ed21.png)

![image](https://user-images.githubusercontent.com/106887052/175757984-b0b510e5-1e43-4055-aa47-4c09e123ebd6.png)

As you can see it looks like besides the "TERP" and "RUN" stocks, every stock performed worse in 2018 than it did in 2017. The TERP stock is also the only stock of the group that had a negative return in both years, while the "ENPH" and "RUN" stocks are the only stocks to have a positive return in both years. The time it took for the original code to run was 0.8203125 seconds for 2017 and 2018.

#### Refactored Code
This refactored code I used to attempt to get a faster result.
![image](https://user-images.githubusercontent.com/106887052/175758425-375d5b60-d6b6-4666-8fef-6984c20fa76f.png)

![image](https://user-images.githubusercontent.com/106887052/175758447-1ec65363-9440-4e44-a549-cab1c24a2752.png)


##### Refactored Code Results

![image](https://user-images.githubusercontent.com/106887052/175758555-c5498fc2-fe28-448a-9ff9-b8106a8ebbfe.png)

![image](https://user-images.githubusercontent.com/106887052/175758570-5aa13f2c-d433-48bc-9e74-991af34c7014.png)

The use of the refactored code has resulted in a much faster run time for the code, with 0.1328125 seconds for the year 2017 and 0.125 seconds for the year 2018.

## Summary
By establishing tickerIndex as a variable and setting it to equal 0, we are able to use tickerIndex and insert it into the formulas to run in the tickerVolumes, tickerStartingPrices and tickerEndingPrices arrays. Thus saving time, instead of the original code where it featured a nested loop. The advantage to having a code refactored is because since it takes takes less time to run, it is more efficient in preserving CPU power. One disadvantage I found was properly writing the code in order for it perform correctly. It feels like it increases the odds of one small mistep causing the code to not work, due to the code being a little more complicated.
