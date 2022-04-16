# Project 1 Challenge

## Financial Planning with APIs and Monte Carlo Simulations

We are approached by a client who would like to invest $500,000 over the next 15 years in order to plan for her retirement. She is debating on whether to purchase a home in her local market (Seattle, Tacoma, Everett), stocks & bonds, or crypto. She would like us to analyze possible outcomes in order to maximize the return on her investment.


User Story:

As an investor I want to invest $500k in either real estate, stocks and bonds, or crypto so that I can maximize on the return in 15 years.

Acceptance Criteria:

Given the analysis on real estate markets, stocks and bonds, and crypto, when the ROI is higher in one of the portfolio options then we would recommend the portfolio to the client.


We plan to analyze historical data of real estate by getting an annual appreciation rate for neighborhoods in Seattle, Tacoma, and Everett and then applying that to the initial investment. We will analyze crypto and stock/bonds with Monte Carlo simulations to propose different investment portfolios to the client in order to estimate possible outcomes.



## Technologies

This project is written in python. The required libraries in order to use the application are: 
os, requests, json, pandas, load_dotenv from dotenv, alpaca_trade_api, MCSimulation from MCForecastTools, %matplotlib inline, Path from pathlib, and hvplot.pandas.



## Examples

![RealEstate](https://github.com/theop-55410/Project-1/blob/main/Images/RE1.jpg)

![RealEstate2](https://github.com/theop-55410/Project-1/blob/main/Images/RE2.jpg)

![MC_StockBonds](https://github.com/theop-55410/Project-1/blob/main/Images/SB1.jpg)

![MC_StockBonds](https://github.com/theop-55410/Project-1/blob/main/Images/C2.jpg)


## Analysis Summary

Real estate: Based on historical data analysis,  Central Seattle provided the greatest amount of annual appreciation at just over 15%. If the investor chooses to invest their $500,000 into the real estate market in Central Seattle, we estimate their investment would be worth approximately $1,633,327.08 at the end of a 15 year ownership period.

Stocks and bonds: There is a 95% chance that an initial investment of $500,000 in the portfolio over the next 15 years will end within in the range of $1,626,961.92 and $6,270,274.26.

Crypto: There is a 95% chance that an initial investment of $500,000 in the portfolio over the next 15 years will end within in the range of $53,063,020,989,972,864.00 and $754,312,303,589,329,600,512.00.

DISCLAIMER: Although this result presents potentially fantastic news, it’s important to note that these forecasted return values are based on only three years of historical price data. The forecast simulates more variability than the data that the simulation is based on includes. In general, it’s ideal to supply one year of historical data for each year of simulated data. If we simulate using only small amounts of data during a recent time when markets are booming, or instead falling precipitously, a Monte-Carlo Analysis will inadvertently extrapolate this temporary market movement too far into the future. Getting data over a longer time period mitigates this effect. Due to the limitations of the Alpaca API, however, we can typically produce just three full years of historical data.



## Contributors

Cody Schroeder, codeman@uw.edu

Hilary Willis, hilarywillis@gmail.com

Theo Prentice, theoprentice14@gmail.com

Aaron Bumgarner, aaron.j.bumgarner@gmail.com

Aranda Furth, arandafurth@gmail.com



## License

Copyright 2022 Cody Schroeder, Hilary Willis, Theo Prentice, Aaron Bumgarner, Aranda Furth

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
