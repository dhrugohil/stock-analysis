# stock-analysis
VBA module 2 DATA ANALYTICS
# Refactoring assignment
## By Dhru

### Overview of Project:
The purpose of this assignment is to develop skills in refactoring code. [Refactoring](https://en.wikipedia.org/wiki/Code_refactoring) or code refactoring is the process of changing an **existing** code to make it more efficient—by taking fewer steps, using less memory, or improving the logic of the code to make it easier for future users to read. In this analysis, we took daily ticker data for 12 stocks for 2 years in an MS Excel spreadsheet. Using scripting in visual basic (VB) we modified the Module 2 script to run in a more automated fashion so as to reduce code complexity, improve run times and make the code cleaner.

### Purpose of this analysis:
The purpose of the analysis is to analyse stock ticker data. Ticker data consists of the symbol of the stock, daily volume of shares traded, its open, high, low, close and adjusted close prices every day of the year when the share is traded. A cursory analysis of the spreadsheet shows that there were 251 trading days in 2017/2018. The volume of the shares traded shows the interest of traders and investors in a stock. The annual appreciation (return) of the stock is calculated by the formula below:

```(closing price on last day of year / closing price on first day of year) - 1```

These two indicates the profitability and risks involved in a stock. The Module 2 script found the total annual volume and annual appreciation for the 12 stocks. In this assignment, we have modified that script to use arrays and loops to calculate the same for either of the years, based on user input (year).

### Results

#### Stock performance
The image below shows the stock performance in 2017. As we see all the stocks (except TERP) gave positive returns. The highest returns was obtained from DQ (=199.4%) and lowest from TERP (=7.2%). FSLR traded roughly 68 billion shares during 2017, whereas DQ traded just 3 billion shares.

![VBA_Challenge_2017_screenshot](Resources/VBA_Challenge_2017.png)

The image below shows the stock performance in 2018. As we see all the stocks (except ENPH and RUN) gave negative returns. The highest returns was obtained from RUN (=84.0%) and lowest from DQ (=62.6%). ENPH traded roughly 60 billion shares during 2018, whereas AY traded just 8 billion shares.

![VBA_Challenge_2018_screenshot](Resources/VBA_Challenge_2018.png)

#### Code execution times
The original solution took 0.4336 and 0.4297 seconds (rounded off to 4 decimal places) to run for 2017 and 2018, respectively. The refactored solution completed within 0.0664 and 0.0703 seconds (rounded off to 4 decimal places) for 2017 and 2018, respectively. This is **6 times speed-up**. If we had more data, the time speed-up would be more appreciable. This was possible due to use of arrays and loops. The execution time comparison is pictorial represented below.

![comparison](Resources/comparison.png)


### Summary
The code did a quick analysis of ticker data for 12 stocks for 2 years. The refactoring helped improve the execution time by manifolds. Next we discuss the advantages or disadvantages of refactoring code; and finally how these apply to refactoring the original VBA script.

#### Advantages
By refactoring an existing code base we improve several aspects of the program, some of which are listed below:

1. Improves the design, structure, and/or implementation of the software
2. Improves code readability
3. Reduces code complexity
4. Improves source code's maintainability
5. Creates a cleaner internal architecture to improve extensibility
6. Improves performance

#### Disadvantages
Refactoring has some disadvantages too. Some of them are listed below:

1. Loss of accurate knowledge of the system
2. Lot of additional effort 
3. Generates architectural modifications that may damage the system
4. Trade-off between memory and speed

In the current example, the summarized datasets were stored in arrays. These arrays occupy memory. In low memory systems, this kind of refactoring may not improve performance. 

Overall, code refactoring is an important exercise to improve the updatability and maintainability of any software system. 

