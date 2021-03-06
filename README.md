# VBA Stock Analysis

## Overview of Project
The current project is aimed to analyze Stock Market fluctuations to consequently allow the end-users to make informed decisions on the Stock Market arena.
### Purpose
Current projects examines a subset of the Stock Market data between 2017 and 2018 through the use of VBA code snippets to determine whether a particular stock performed well on the market or if it lost its value over time. This quick analysis would allow the end-user to guide their future stock decisions based on the stock behaviour that is available for them thus far.

Additionally, a secondary goal of the current project was to attempt to refacture the associated VBA code to cut on the execution time and provide for a more flexible and less memory-consuming algorithm.
## Results

### Stock Performance For 2017 Versus 2018
![Screenshot_6](https://user-images.githubusercontent.com/99566803/158032126-68e0fb2d-e4ca-4c7e-9565-d28d3bc33708.png)
![Screenshot_4](https://user-images.githubusercontent.com/99566803/158032127-da797091-a4f6-472a-aff9-048d1be6752a.png)

When comparing the results of stock performance between 2017 and 2018, a number of trends can be immediately identified. First, it should be evident that 2017 was a much more successful year for the stock market overall, with only the TEPR stock category performing negatively during that year. Opposite to that, most of the stocks ended up in the negative skew in 2018 (meaning that they lost in value, as oppoosed to gaining it), with only two stocks - ENPH and RUN - performing positively during said calendar year.

The TERP stock can be identified as a "red flag" anamoly - it lost its value in both 2017 and 2018. As such, one should exercise extreme caution when deciding on whether they would like to buy said stock. On the other hand, ENPH and RUN stocks had a positive closing statement at the end of both years, thus making them a potentially safe bet for stock traders.

Overall, however, it is hard to establish any sort of predictable stock pattern based solely on the two years examined, thus further analysis of the years to follow (i.e., 2019, 2020, 2021) should be considered prior to making any substantial stock market decisions.

### Code Performance Between The Original Script and The Refactored Version
![Screenshot_2](https://user-images.githubusercontent.com/99566803/158032132-dbcebff2-d9bc-45c0-a742-f6bbb4040659.png)
![Screenshot_3](https://user-images.githubusercontent.com/99566803/158032133-ade7f52f-44ad-45bc-b838-3a21a74a4a47.png)

The original, "raw" code ran the script in 0.76 seconds for the year 2017 and in 0.75 seconds for the year 2018. Arguably, in both instances the original code ran relatively fast and smoothly. It should be taken into consideration, however, that the data analyzed with the use of the code consisted of approximately 3000 rows of Excel data, meaning, in other words, that the code can have substantial timing flaws if we were to run it on a much bigger dataset.

![VBA_Challenge_2017](https://user-images.githubusercontent.com/99566803/158032139-74600d68-9b55-4004-a3b6-a6abfee85968.png)
![VBA_Challenge_2018](https://user-images.githubusercontent.com/99566803/158032141-c1cc1a1a-aa54-46a7-8d4a-c8113631b75b.png)

As a result, the process of refactoring have been applied to the original code in order to improve the logic of it, and to minimize execution time by reducing the number of steps that the program would have to take in order to calculate the outcome. As can be seen on the associated screenshots, refactoring proved to be a worthy endeavour, as the execution time was cut down to 0.11 seconds for 2017 and to 0.10 seconds for 2018. In other words, these small logistic changes allowed our code to run, on average, about **0.64 seconds faster** for either of the datasets.


## Summary

### Advantages and Disadvantages of Refactoring Code
**Advantages:**

Refactured code oftentimes appears more clear and comprehensible than an "unpolished" one. It is also generally shorter than the originally created code, simply for the solutions within refactured code are more "elegant" in their execution and write-ups, such as the case with nested for loops.
Refactured code allows also for the developer to more easily come back to it later on, especially if a substantial amount of time has passed since the original submission have been made. This is partially attributed to the "modular" nature of the refactored code, and partially due to the less challenging coding functions employed.

**Disadvantages:**

Naturally, refacturing the code can take a long time - potentially longer than it would take to simply run the program with the original code. In that sense, it is a trade-off between fast completion of original work versus possibility to expand the applicability of the code when refactoring for it to be reusable later on.
Certain refacturing processess can be overlooked or plain out completely invisible to and by the end-user, resulting in an unpleasant feeling of wasted time on the client side.

### Applicability to Current Code
In terms of the current code, similar pros and cons apply. Thus, for example, the original VBA script served its purpose as intended - it found the appropriate stocks, calculated their starting and ending prices, and delivered the information specifically important to the end-user in that the stock was either losing or gaining in value. The original code, however, as have been mentioned previously, executed itself in a slower manner than the refactored code, which in and by itself might not be a big issue. However, the original code was also logically inferior to the refactored script, as the original code had to scan through the entire document more than once in order to collect the required information, while the refactored code only had to go through the document once (reducing that way both the time it took for the code to run, and the memory load that the computer is silently taking in the background).

To conclude, refactoring seems to always be beneficial for the developers, the code itself, and the end user, for varying reasons. And while the effects of refacturing might not be immediately available for us to see, they truly lower the amount of hard work, debugging, and "brute force" that the developers would need to initiate if they were to come back to their code later on.
