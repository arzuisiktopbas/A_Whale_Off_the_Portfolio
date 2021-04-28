# A Whale Off the Port(folio)
   *by Arzu ISIK TOPBAS*

![Portfolio Analysis](https://s3.amazonaws.com/static-assets.m1finance.com/wp-content/uploads/2019/04/16201340/investment-portfolio-01.jpg)

## Background

In this HW, I used quantitative analysis techniques with Python and Pandas to determine which portfolio is performing the best across many areas: volatility, returns, risk, and Sharpe ratios. And I created an analysis notebook that analyzes and visualizes the major metrics of the portfolios across all of these areas, and determine which portfolio outperformed the others.

I had the historical daily returns of several portfolios: some from the firm's algorithmic portfolios, some that represent the portfolios of famous "whale" investors like Warren Buffett, and some from the big hedge and mutual funds. 

In this homework assignment, I accomplished three main tasks:

1. Read in and Wrangle Returns Data - Preparing the Data
2. Determine Success of Each Portfolio - Conducting Quantitative Analysis
3. Choose and Evaluate a Custom Portfolio - Creating a Custom Portfolio(both preparing the data & conducting quantitative analysis)

---
## Analysis

#### Performance Analysis

1. Calculate and plot cumulative returns. Does any portfolio outperform the S&P 500?
* In the "Daily Returns" plot, I am not able to see which portfolio is outperform the S&P 500, but Tiger and BHI have some one-day volitilities. 
* In the **"Cumulative Returns" plot**, I can easily see that **the most outperformed** portfolios are **Algo1 and BERKSHIRE HATHAWAY INC .**

![Cumulative Returns](https://github.com/arzuisiktopbas/03-A_Whale_Off_the_Portfolio/blob/main/Images/HW3-Cumulative%20Returns.png)

#### Risk Analysis

1. Create a box plot for each of the returns. Which box has the largest spread? Which has the smallest spread?
* In the **"Portfolio Risk" plot**, **BERKSHIRE HATHAWAY INC** has **the largest** spread which means that It has the largest deviation in the daily returns.
* **PAULSON & CO.INC.** has **the smallest** spread which means that It has the smallest deviation in the daily percentage change.

![Portfolio Risk](https://github.com/arzuisiktopbas/03-A_Whale_Off_the_Portfolio/blob/main/Images/HW3-Portfolio%20Risk.png)

2. Calculate the standard deviation for each portfolio. Which portfolios are riskier than the S&P 500?
* When I checked the standard deviations of all portfolios, both **BERKSHIRE HATHAWAY INC (0.012919) and TIGER GLOBAL MANAGEMENT LLC (0.010894)** have higher standard deviations than S&P 500 (0.008342). This means these portfolios are **riskier** than the S&P 500.

![Standard Deviations](https://github.com/arzuisiktopbas/03-A_Whale_Off_the_Portfolio/blob/main/Images/HW3-Standard%20deviations.png)

#### Rolling Statistics

1. Plot the rolling standard deviation of the various portfolios along with the rolling standard deviation of the S&P 500 using a 21 day rolling window. Does the risk increase for each of the portfolios at the same time risk increases in the S&P?
 * When I checked the **"21 Day Rolling Standard Deviation" plot** , It seems that all portfolios have been moving with the S&P 500. Specifically, **BERKSHIRE HATHAWAY INC** has a greater standard deviation,and it is more volatile than the other portfolios.
 
 ![21 Day Rolling Standard Deviation](https://github.com/arzuisiktopbas/03-A_Whale_Off_the_Portfolio/blob/main/Images/HW3-21%20Day%20Rolling%20St%20dev.png)

2. Construct a correlation table for the algorithmic, whale, and S&P 500 returns. Which returns most closely mimic the S&P?
 * **Algo 2** has the best mimic SP500, means that **Algo 2** has **the best correlation** to SP500.
 
 ![Correlation](https://github.com/arzuisiktopbas/03-A_Whale_Off_the_Portfolio/blob/main/Images/HW3-Correlation.png)
 
3. Choose one portfolio and plot a rolling beta between that portfolio's returns and S&P 500 returns. Does the portfolio seem sensitive to movements in the S&P 500?
* **BERKSHIRE HATHAWAY INC beta** is **1.134.** This suggests that for every +1% move in the S&P 500 our portfolio will go up 1,134 % in value.

 ![BERKSHIRE HATHAWAY INC beta](https://github.com/arzuisiktopbas/03-A_Whale_Off_the_Portfolio/blob/main/Images/HW3-BHI%20Beta.png)


### Plot Sharpe Ratios

2. Determine whether the algorithmic strategies outperform both the market (S&P 500) and the whales portfolios.
On the basis of this performance metric, do our algo strategies outperform both 'the market' and the whales? 
* **Algo 1** outperformed S&P500 and whales while Algo 2 fell below S&P500  and BERKSHIRE HATHAWAY INC.

 ![Sharpe Ratios](https://github.com/arzuisiktopbas/03-A_Whale_Off_the_Portfolio/blob/main/Images/HW3-Sharpe%20Ratios.png)
 
### Create Custom Portfolio

5. How does your portfolio fair?

* When I checked the standard deviations of all portfolios,**My portfolio(0.211496)** has **the one of the highest standard deviations,(others : TIGER GLOBAL MANAGEMENT LLC (0.232531) and BERKSHIRE HATHAWAY INC (0.247155))**. This means these  are **riskier portfolios.** 

![Standard Deviations](https://github.com/arzuisiktopbas/03-A_Whale_Off_the_Portfolio/blob/main/Images/HW3-%20Annualized%20My%20portfolio%20sta%20dev.png)

* When I am looking **the "Sharpe Ratios" plot**, I can say **my portfolio performs well** after Algo 1.

![Sharpe Ratios](https://github.com/arzuisiktopbas/03-A_Whale_Off_the_Portfolio/blob/main/Images/HW3-%20My%20portfolio%20Sharpe%20Ratios.png)

* **My portfolio** is **highly correlated** with S&P 500.

![Correlations](https://github.com/arzuisiktopbas/03-A_Whale_Off_the_Portfolio/blob/main/Images/HW3-My%20portfolio%20Corr.png)

* **My portfolio beta** is **1.212.** This suggests that for every +1% move in the S&P 500 our portfolio will go up 1,212 % in value.

![My portfolio beta](https://github.com/arzuisiktopbas/03-A_Whale_Off_the_Portfolio/blob/main/Images/HW3-%20My%20port%20Beta.png)
---
