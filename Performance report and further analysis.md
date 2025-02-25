# Indian gorwth stock mutual fund construction (2024/03/18-2024/05/24)

## Abstract

This study aims to explore the performance of growth-oriented funds in India by analyzing different stock selection strategies, portfolio returns, and risk characteristics to evaluate the fund’s investment effectiveness in the current market environment.

We selected 10 company stocks as the fund’s components and adjusted the stock holdings based on market performance during the investment period.

The study shows that over two months, the fund achieved a positive alpha, a beta value less than 1, and Sharpe and Treynor ratios higher than the benchmark index, indicating that the fund outperformed the market benchmark.

The growth portfolio significantly outperformed the value portfolio in the short term, validating the effectiveness of the stock selection strategy in the short run.

However, the main limitation of this study is the short research period (only two months), which does not fully reflect the long-term investment performance.

## Introduction
This fund is a growth-oriented fund that selects companies with higher price-to-earnings (P/E) ratios. Referring to the three-year average P/E ratio of the Indian market at 22.2, we choose companies with a P/E ratio greater than 24. Additionally, we consider the revenue growth rate as an indicator, selecting companies with a growth rate exceeding 15%. A company qualifies if it meets either of these criteria.

To avoid excessive investment in a single industry, the fund aims to diversify across different sectors for optimal allocation. The fund adopts an equal-weighting approach, distributing the same amount of capital to each selected stock.

The following table shows the overall report of the stock components.

| Stock Code  | Opening Price | Closing Price | Change  | P/E Ratio | Revenue Growth (1 Year) | Beta (1 Year) | Industry        |
|------------|--------------|--------------|---------|----------|-----------------|------------|--------------|
| BHARTIARTL | 1223.5       | 1388.5       | +13.5%  | 97.8     | +7.79%          | 0.35       | Wireless Communication |
| TRENT      | 4054.8       | 4715.4       | +16.3%  | 97.0     | +50.15%         | 0.21       | Apparel Retail |
| SIEMENS    | 4771         | 7283.3       | +52.7%  | 72.8     | +19.49%         | 0.79       | Electronics    |
| KPITTECH   | 1427.5       | 1551.55      | +8.7%   | 65.5     | +44.77%         | 1.22       | Automotive Software |
| CYIENT     | 1976         | 1815         | -8.1%   | 32.1     | +18.81%         | 1.13       | Diversified Software |
| MARUTI     | 11438.4      | 13000.45     | +13.7%  | 26.0     | +20.26%         | 0.56       | Automobile Manufacturing |
| JSWSTEEL   | 783          | 908.65       | +16%    | 25.2     | +5.45%          | 1.38       | Steel         |
| HDFCBANK   | 1451.15      | 1517.2       | +4.6%   | 16.1     | +99.35%         | 1.32       | Banking       |
| TATAMOTORS | 943.8        | 960.55       | +1.8%   | 11.6     | +26.58%         | 1.28       | Automobile Manufacturing |
| SBIN       | 728.75       | 826.6        | +13.4%  | 9.7      | +25.6%          | 1.17       | Banking       |
| VBL        | 1507         | 1498.3       | -0.6%   | 90.5     | +15.65%         | 0.4        | Beverages     |
| SENSEX     | 72587.3      | 74005.94     | +2%     | -        | -               | -          | Index        |

## Stop loss strategy
We have established a rule that if a stock's price drops to 10% below its opening price, we will replace it with another stock. The replacement stock is selected based on a similar market capitalization while ensuring no overlap with existing sector holdings.

On May 6th, the fund decided to replace CYIENT by selling its entire position and purchasing VBL instead. In retrospect, if we had continued to hold CYIENT instead of buying VBL, we would have incurred an additional loss of -US$262,740, or -0.24% of the total return.

## Performance analysis
The fund's net asset value (NAV) initially stood at approximately USD 8.2 billion. After accounting for transaction fees and exchange rate fluctuations, it increased to around USD 9.2 billion, achieving a return of 12.5% over the period.

The standard deviation was 0.7%, with the largest drawdown occurring between April 12 and April 16, amounting to -2.8%.


| Metric                     | Value      |
|----------------------------|-----------|
| **Expected Daily Return**  | 0.2431%   |
| **Holding Period Return (HPR)** | 12.4956%  |
| **Standard Deviation**     | 0.7259%   |
| **Maximum Drawdown**       | -2.8%     |

After regressing the fund's returns against the Indian market returns, we obtained the regression results.

**PR = a + b Rm + et**

In this regression, PR represents the fund's daily return, while Rm represents the daily return of the Indian Sensex 30 index, both denominated in USD. The results indicate that the portfolio's beta is 0.9406, which is lower than the market portfolio beta of 1. This suggests that the fund is less volatile than the overall market.

Using the CAPM formula, we calculated an alpha of 0.0015, indicating that the fund generated excess returns during this investment period.

Additionally, the p-value of 0.067 suggests that at a 90% confidence level, our excess return is statistically significant.

| Portfoilo           | alpha  | beta   | R²   |
|------------------|--------|--------|------|
| *Portfolio/Sensex* | 0.0015 | 0.9406 | 0.634 | 
|     *Standard error*     | (0.001) | (0.109) |  

We evaluate the fund's performance using different metrics. The daily Sharpe ratio of this fund is 0.2393, which is higher than the market’s 0.085. Similarly, the Treynor ratio is 0.0022, which exceeds the market’s 0.0006. This indicates that the portfolio achieves higher returns than the market for both systematic risk and total portfolio risk, demonstrating greater efficiency.

Furthermore, the Information Ratio is 0.2839, meaning that for each additional unit of unsystematic risk taken, the portfolio generates an alpha of 0.2839. Since this portfolio represents our entire investment rather than just one of multiple portfolios, we primarily focus on evaluating the Sharpe ratio. Given that our fund’s Sharpe ratio is higher than that of the market, it suggests that our investment performance surpasses the market.

| Metric       | Portfolio | Market |
|-------------|-----------|--------|
| **Sharpe Ratio** | 0.2393   | 0.085  |
| **Treynor Ratio** | 0.0022   | 0.0006 |
| **Information Ratio** | 0.2839   | ------ |
| **M Square (M²)** | 0.0011   | ------ |

## Furthur discussion of value versus growth stocks in India
To evaluate whether an investment strategy focused on growth stocks is appropriate, we will analyze it from both long-term and short-term perspectives.

From a long-term perspective, we will examine historical literature on the performance of the value factor in the Indian stock market and identify the most suitable asset pricing model for the Indian market.

From a short-term perspective, we will use the Nifty 200 index as a benchmark and employ the price-to-earnings (PE) ratio as a growth reference to construct both growth-oriented and value-oriented portfolios. We will then compare their returns and risks to provide an overview of the value premium during the investment period.

Finally, we will compare our fund’s performance with the self-constructed growth portfolio to assess whether the fund's stock selection demonstrates a relative advantage within growth stocks.

Regarding data selection, we have chosen Nifty 200 as a reference because all stocks in our fund are constituents of this index. This allows us to minimize the short-term impact of the size factor.

For the investment approach, we adopt an equal-weighted strategy to align as closely as possible with our fund’s investment method while eliminating the influence of weighting techniques on portfolio returns. The impact of different weighting methods will be further explored in the next section.

## Literature review

To identify whether factors beyond market risk premium can explain stock return generation in India over the long term, we reviewed the empirical results of the five-factor model proposed by Fama and French (2015) in the Indian market.

Harshita et al. (2015) analyzed data from 1999 to 2014, using CNX 500 companies to construct the value, size, investment, and profitability factors and formed four investment portfolios incorporating these factor premiums for testing. Their findings indicate a positive relationship between return rates and book-to-market ratio, suggesting the presence of a value premium in the Indian market.

Agarwalla et al. (2017) conducted a systematic review of value, size, and momentum factors. Regarding the value factor, their study reported a 9.08% stable annualized return with a 16.33% volatility, outperforming the global average value premium reported by Fama and French (2012) and aligning closely with the value premium observed in emerging markets.

Based on these studies, it is evident that the value factor exists in both India and other emerging markets over the long term. Therefore, a high-growth strategy may not be suitable for long-term investors with an investment horizon of over 10 years as a long-term asset management target. However, given that this fund has only been in existence for two months, it remains uncertain how the value premium fluctuates in the short term, which will be further discussed in the next section.

## Short term value premium

To identify the value premium during the existence of this fund, we ranked all Nifty 200 constituent stocks by their price-to-earnings (PE) ratio from highest to lowest. We excluded companies with missing data and selected the top 30 stocks as the Growth Portfolio (GP) and the bottom 30 stocks as the Value Portfolio (VP). Both portfolios were equally weighted.

![image](https://github.com/user-attachments/assets/a368546c-485f-474f-913c-d0f89dce00e5)



Where:
-  R_t  represents the **risk premium**.
-  GR_t  is the **daily risk premium** of the top 30 **growth stocks** (high PE ratio) in Nifty 200, measuring the return of growth stocks.
-  VR_t  is the **daily risk premium** of the bottom 30 **value stocks** (low PE ratio) in Nifty 200, measuring the return of value stocks.
-  t  represents the **investment period**.
- **Data sources**: **Yahoo Finance** and **TradingView**.

Ignoring transaction costs, we solely compare the performance of the growth and value portfolios during the investment period using the following regressions:

![image](https://github.com/user-attachments/assets/e6eacdc6-3d27-4eb2-b830-43d210f7fc58)


The following table presents the performance metrics of both portfolios. The results indicate that regardless of the performance metric used, the growth portfolio consistently outperformed the value portfolio over the two-month period. Therefore, in the short term, the fund’s strategy of primarily investing in growth stocks appears to be the correct direction.

| Model/Portfolio | alpha  | beta | Average Return | Sharpe Ratio | Treynor Ratio | Information Ratio |
|----------------|------------|------------|----------------|--------------|--------------|------------------|
|  GR_t / GP  | 0.0021 | 0.8590 | 0.0029 | 0.3199 | 0.0033 | 0.3072 |
| *Std. Error* | (0.001) | (0.160) |  |  |  |  |
|  VR_t / VP  | 0.0019 | 0.9227 | 0.0027 | 0.2264 | 0.0029 | 0.1860 |
| *Std. Error* | (0.002) | (0.238) |  |  |  |  |

We attempted to use the Growth Portfolio (GP) as a benchmark portfolio and compared the regression results with the original benchmark portfolio, SENSEX 30. The following table presents the coefficient returns of both models.

From the results, we observe that while GP does not explain the fund's performance as effectively as SENSEX 30, this may be due to the fund incorporating multiple growth indicators, such as price-to-earnings (PE) ratio and annual revenue growth rate, and diversifying investments across high-growth companies in various industries.

Moreover, when using GP as the benchmark portfolio, the fund's ability to generate excess returns appears to be relatively lower. This suggests that the fund does not demonstrate a strong ability to select superior growth stocks, nor does it exhibit relative superiority in returns compared to GP.

| Portfolio Benchmark | alpha | beta  |  R^2  |
|---------------------|------------|------------|---------|
| **Portfolio / GP** | 0.0002 | 0.6473 | 0.453 |
| *Std. Error* | (0.001) | (0.110) |  |
| **Portfolio / SENSEX** | 0.0015 | 0.9406 | 0.634 |
| *Std. Error* | (0.001) | (0.109) |  |
