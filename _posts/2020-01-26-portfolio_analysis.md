**Performance Measurement Metrics**

Portfolio performance measurement is one of the most significant part of investment performance evaluation and risk management analysis. Screening the performance of the invesments with due diligence requires to a comprehensive approach. Todays financial instruements and investment approaches complicates continuous monitoring of investment performances. Coming up with a single number which indicates the sole performance of an investment is very difficult if not impossible. However, as each metric has its own strengths and weaknesses, screening several of them can help to alleviate this task. Nevertheless, number of metrics available may exceed the number of concerns one have over the investment she has done. Therefore, choosing the right metric to follow may not be easier than screening the performance of an investment.

In this report, we intend to provide seventeen of the most prominent performance metrics and an overview of each them together with a ready-to-use Python module. Some of the metrics calculated are straightforward and may not attract attention as much as others. Nevertheless, these arethe measures, that we find worth monitoring independent of its complexity.

The Python module not only calculates the below mentioned metrics but also creates beautiful graphs which visualize the key events for the portfolio/asset class under investigation. Nevertheless, the weaknesses and strengths of each metric presented below are different and unfortuantely beyond the scope of this report.

**1.Sharpe Ratio**

Sharpe ratio is proposed by William F. Sharpe as a measurement method of mutual fund performance (Sharpe 1965). The ratio originally named as Reward-To-Variability ratio but reviewed and restored in 1994 by Sharpe. The Sharpe ratio measures the excess return of the risk free rate per unit of total risk or volatility of a trading and portfolio management strategy. This implementation is also called the risk premium compared with the total risk of the portfolio which is measured by standard deviation. The Sharpe Ratio takes as reference the Capital Market Line and be termed as Information Ratio.

Sharpe ratio is calculated by subtraction of R<sub>p</sub> (the annualized multi-period return over period T) and R<sub>f</sub> (the annualized base currency risk free return over period T) divided by σ **(**R<sub>p</sub>) (the annualized volatility of the portfolio return over period T.

![](/images//2020-01-26-portfolio_analysis/image2.png)

![](images/2020-01-26-portfolio_analysis/image2.png)

A greater Sharpe ratio ratio indicates a better performance on a risk adjusted basis. One remark though is, a higher Sharpe ratio may not be the most desired one since Sharpe ratio puts two things together; excess return and its associated risk.

**<span class="underline">Strengths and weaknesses of Sharpe Ratio</span>**

  - Sharpe ratio provides simplicity to the while measuring and following aggregate portfolio performance. Facilitates appropriate portfolio returns that are not exactly decomposed.

  - The Sharpe ratio indicates both upward and downward volatility equally, investors mainly notices the downward values however eliminating upward values may increase the Sharpe ratio.

  - It is measured by followed the stationary and parametric path. Each daily change creates greater statistical characteristic hence have heavier tails and higher peaks than normal distribution then reveals kurtosis and skewness and biased estimates of standard deviation.

  - The portfolio with the highest Sharpe Ratio is not the most desirable ratio alone for investors.

**2.Sortino Ratio**

Sortino Ratio is conceived by Dr. Frank Sortino in Pension Research Institute in 1991. The Sortino ratio is one of the risk – adjusted measurement techniques which was provided to hendle one of the weaknesses of the Sharpe ratio. That is, Sortino ratio upward and downward volatility equally.

Sortino Ratio is calculated the subtraction of Rp (Annualized multi-period return over period) and T<sub>A</sub> /Multi period target rate of return to the investment strategy under consideration over period T) by divided DR √T (where DR is target semi-deviation or downside risk that measures the variability of returns below a minimum target rate. T is the number of single observations in reporting period.

![](images/2020-01-26-portfolio analysis/image3.png) ![](images/2020-01-26-portfolio analysis/image4.png)

The Sortino Ratio is ordinarily used in a relative context in order to compare two or more funds in a benchmark index. A higher Sortino Ratio exhibits better risk adjusted performance. The important point is that while measuring Sortino ratio is should be used the same minimum acceptable return, MAR.

Sortina ratio ignores updside varaition and only considers downside risk. This may be seen an incompatible perspective on the definition of risk.

<span class="underline"></span>

**3. Risk Return Ratio**

Rsimilar to Sharpe ratio and Sortino ratio, Risk Return Ratio is a measure of return in terms of risk for a specific period. The risk measure udes by Risk Reward ratio is maximum drawdown in percentage. The RRR was first defined and popularized by Dr. Richard CB Johnsson (Johnsson, 2010). Risk reward ratio is widely used and has strengths over other return-to-some-risk ratios.

Risk Return ratio can be regarded as the percent return per unit of the losses happened during the worst days of the portfolio. So, if a portfolio get over the bad days, the risk measure used in the risk return ratio, maximum drawdown, may not change until the next maximum drawdown. In such a situation, the only effect which result a fluctutation in the risk return ratio would come from the cahnge in the return of the portfolio in that period.

Risk Reward Ratio is calculated by equating minimum win rate which is defined by investor, 1 over addition 1 and reward/risk ratio.

> ![](images/name/image5.png)

Again since this a return-to-some-risk-ratio, higher the ratio better the portfolio performs.

**4.Treynor Ratio**

The Treynor Ratio was conceived by Jack L. Treynor in 1965 and also called Reward-To-Volatility Ratio or Treynor measure. The Treynor Ratio is a risk-adjusted performance measurement method that is calculated as a ratio of excess return to portfolio’s sensitivity to market risk, namely market risk. Clearly, instead of total risk a measure of systematic risk is used in the Treynor ratio. Hence, Traynor ratio is the measurement of returns earned in excess of risk free rate (which is assumed to have no diversifibale risk) per each unit of market risk taken.

For a one-year measurement of performance, the annualized Treynor Ratio is calculating as **R<sub>f</sub>** (The annualized base currency risk free return over period **T**) subtracted by **R<sub>p</sub>** (The annualized multi period return over period **T**) then divided **β** (**R<sub>p,</sub> R<sub>B)</sub>** (Beta of return **R<sub>p portfolio</sub>** return relative to benchmark return **R<sub>B.</sub>**

> ![](images/2020-01-26-portfolio analysis/image6.png)

The higher ratio values indicate better portfolio on a relative risk-adjusted basis.

**5.Maximum Drawdown**

The Maximum Drawdown method is measures the largest peak through decline in the value of a portfolio. Another definition is the maximum equity loss that have experienced during an investment. Obviously, a drawdown can be only measured once a new peak is generated.

The Maximum Drawdown is calculated by subtraction of Equity Peak High and Equity Through Low divided by equity peak high.

> ![](images/2020-01-26-portfolio analysis/image7.png)

<span class="underline"></span>

The maximum drawdown can be used either as a standalone risk assesment measure or as a combination with other metrics. One drawback of the maximum drawdown is that It only measures the largest loss but do not give information about the frequency of large losses. The maximum drawdown measure can also be seen as the magnitude of the pain, ie. How low it goes, an investor has taken.

**6. Maximum Drawdown Duration**

The drawdown duration indicates the time period from a peak point in the value of a portfolio. The Maximum Drawdown duration is the longest period between peaks. Ideally, an investor would expect these drawdown durations to be as short as possible. So, the maximum of these durations would aslo be shorter.

As long as the price or value remains below the old peak, independent of the amount of loss the portfolio experienced, the drowdaown duration increases.

FORMULA

The maximum drawdown duration can be used either as a standalone risk assesment measure or as a combination with other metrics. One drawback of the maximum drawdown duration is that It only measures the longest time pariod of loss but do not give information about the amount of magnitude of losses. The maximum drawdown measure can also be seen as the duration of the pain, ie. How long it lasts, an investor has lived through.

**7. Market Beta**

Market Beta is the measurement technique that quantifies stock’s volatility in relation to the market. It is a measure of systematic risk a portfolio has taken as opposed to idiosyncratic factors. In other words, market beta shows how volatile a portfolio compared to market portfolio. A beta greater than 1 generally means that the asset both is volatile and tends to move up and down with the market.

Market Beta is calculated;

> ![](images/2020-01-26-portfolio analysis/image8.png)

Which R<sub>e</sub> represents the return of the individual stock, R<sub>m</sub> is the return on the overall market, and covariance is how changes in a stock’s return are related or changes in the market’s return, variance is how far the market’s data points spread out from their average value.

Beta represents the the risk that can not be eliminated by diversification. Beta is one of the most widely used measures in finance. Especially, portfolio perforamnce analysis, beta is used as a measure of risk arising from a exposure to a benchmark for the portfolio.

**8. Alpha**

Alpha is a measurement technique that indicates when strategy, investor or portfolio manager has managed to beat the market return over specified period compared to a benchmark portfolio. Alpha can be describes as active return on an investment, quantifies the performance of portfolio against market index or whole movements in markets.

Alpha can be seen as abnormal rate of return and it differs from beta significantly. In rough terms, alpha is excess return relative to peers, but beta measures market volatility or risk of security of a portfolio. Both alpha and beta are historical measurement methods which can be seen as a deficiency.

Alpha is calculated;

> ![](images/2020-01-26-portfolio analysis/image9.png)

summation of end price and distribution per share minus start price divided by start price.

**Example. Alpha CAPM**

CAPM Alpha is the rate of return that exceeds what was expected or predicted by models to exemplify Capital Asset Pricing Model (CAPM). The formula of Alpha CAPM is

> ![](images/2020-01-26-portfolio analysis/image10.png)

formula represents **r** is portfolios return, **R<sub>f </sub>**is risk free rate of return, **beta** is portfolio’s price volatility relative to the whole market and **R<sub>m</sub>** is the market return.

The main part of the CAPM formula exhibits the return on a certain portfolio will be under certain market conditions. Two similar portfolios can move with same beta however may generate different alphas.

<span class="underline"></span>

**11. VaR (Value at Risk)**

Value at Risk (VaR) is a measurement method that indicates riskiness of financial portfolio or entities. In other words it exhibits the amount of potential loss that may occure. VaR has a wide range of usage cases across the finance industry. VaR has four main uses in finance: risk management, financial control, financial reporting and computing regulatory capital. VaR is typically used by firms and regulators in the financial industry to gauge the amount of assets needed to cover possible losses.

A more technical definition of VaR can be; for a given portfolio, time horizon, and probability p, the p VaR can be defined informally as the maximum possible loss during that time after we exclude all worse outcomes whose combined probability is at most p.

There are different methodoliges to calculate VaR. Below you may find historical. Depending on the approach you adopt, the calculation may become complicated. Below you may find a simple method to calculate VaR which assumes p as 1%.

It is calculated;

> ![](images/2020-01-26-portfolio analysis/image11.png)

Where **V<sub>i</sub>** represents the number of variables on day **i**, **m** is the number of days from which historical data is taken(historical method), in parametric method two factors are to be estimated but it is not reliable when the sample size is very small. In parametric method variance and covariance factors are using to estimation for return or standard deviation. Another calculation method is Monte Carlo method which is calculated randomly creating a number of scenarios for future rates and calculating VaR according to worst losses.

**12. Maximum Single Period Return**

Maximum Single Period Return indicates the highest return acquired in a time step during the a specified period of an investment portfolio. It represetns the historical higher bound.

![](images/2020-01-26-portfolio analysis/image12.png)

**13.Minimum Single Period Return**

Maximum Single Period Return indicates the highest return acquired in a time step during the a specified period of an investment portfolio. It represetns the historical higher bound.

FORMULA

**14.Skewness**

Skewness is asymmetry in a statistical distribution which the curve appears distorted or skewed either to the left or to the right. Skewness can be quantified to define the extent to which a distribution differs from a normal distribution. The famous normal distribution has a skewness value of zero while lognormal distribution exhibits some degree of right skew. Right skewness is positive and left skewness is negative varying degrees.

![](images/2020-01-26-portfolio analysis/image13.png) ![](images/2020-01-26-portfolio analysis/image14.png)

Where S<sub>k</sub>1 represents Pearson’s first coefficient of skewness and S<sub>k</sub>2 the second, s is the standard deviation for the sample, X<sup>-</sup> is the mean value, Mo the mode value and the Md is median value.

Skewness considers extreme values of the data rather than focusing solely on average. A left skewed portfolio return distribution tells that the rare events with high losses have happende in the life time of the investment whereas small and positive returns are more common.

> ![](images/2020-01-26-portfolio analysis/image15.png)

**15. Kurtosis**

Like skewness, Kurtosis is a statistical measure that is used for describe a distribution. However unlike skewness, Kurtosis measures the frequency of extreme values in either tail. A distribution with large Kurtosis indicates tail data exceeding the tails of normal distribution.

> ![sample kurtosis equation](images/2020-01-26-portfolio analysis/image16.png)

Where n is the sample size, s is the standard deviation and X is the mean value. The formula takes into account the sample size and it subtracts 3 from the kurtosis. With this equation the kurtosis of a normal distribution is 0.

For investors or portfolio managers the high Kurtosis of return exhibits they will experience occasional extreme returns (positive or negative) which are more extreme than usual risk.

**16. Conditional DrawDown**

Conditional drawdown handles the key drawback of maximum drawdown; instead of presenting the maximum of drawdowns, conditional Drawdown presents a particular percentage of these drawdowns. From this persepective the CDD is similar to the conditional value at risk and may be viewed as a modification to it. It takes into account the path of the value of a portfolio through its drawdowns, which the maximum drawdown concentrates on single event of loss from its previous peak.

Researches (REFERNCE\!\!\!) indicates that the CDD with an appropriate level (alpha = 0, 8, i.e. optimizing 20% of the worst drawdowns generates a more stable weights allocation rather than that produces using Maximum Drawdown measure.

The Conditional Drawdown at Risk is calculated as;

![](images/2020-01-26-portfolio analysis/image17.png)

**17. Conditional Drawdown Duration**

Similar to the case of Conditional Drawdown Duration, the conditional drawdown duration rectifies a deficit of Maximum drawdown duration. Instead of focusing the longest period betrween peaks in the value of a portfolio, CDD Duration calculates the a percentage of longest drawdown duration. In this way, it displays a more comprehensive measure for the risk assesment.

Maximum draw down duration can be calculated as follow:

**Appendix**

**References**

1.  A Universal Performance Measure (Con Kreating, William F. Shadwick) (Con Kreating, 2002)

2.  Risk Aversion vs the Omega Ratio : Consistency Results (Sven Balder, 2017)

3.  Portfolio Optimization With Drawdown Constraints (Alexei Cheklov, 2003)

4.  Common Metrics for Performance Evaluation: Overview of Popular Performance Measurement (Dr. Oliver Steinki, 2013)

5.  Drawdown Measure in Portfolio Optimization (Alezei Chekhlov, 2004)

6.  Omega as a Performance Measure (Hosein Kazemi, 2003)

7.  Drawdown: From Practice to Theory and Back Again (Lisa R. Goldberg, 2016)

8.  Leverage space Portfolio Model (Vince, 2007)

9.  [<span class="underline">https://github.com/backtrader/backtrader/blob/master/samples/pyfoliotest/backtrader-pyfolio.ipynb</span>](https://github.com/backtrader/backtrader/blob/master/samples/pyfoliotest/backtrader-pyfolio.ipynb)

10. [<span class="underline">https://www.backtrader.com/</span>](https://www.backtrader.com/)

11. https://github.com/quantopian/pyfolio/blob/master/pyfolio/examples/full\_tear\_sheet\_example.ipynb

12. https://quantopian.github.io/pyfolio/
