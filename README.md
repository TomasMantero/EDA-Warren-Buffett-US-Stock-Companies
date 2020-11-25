# EDA - Warren Buffett US Stock Companies

![Python](https://img.shields.io/badge/Python-3.7.6-blue) ![License](https://img.shields.io/badge/License-Apache%202.0-orange) ![Contributions](https://img.shields.io/badge/Contributions-Welcome-green)

In this notebook we analyze a dataset call [Warren Buffett US Stock Companies](https://www.kaggle.com/tomasmantero/warren-buffett-us-stock-companies), which you can find in Kaggle.

We will be analyzing companies from the technology sector. We will analyze their behaviors over the past few years, as well as their behaviors during the COVID-19 Pandemic.

We will try to determine new trends that can help investors make more informed decisions.

To see the Kernel directly from Kaggle click [here.](https://www.kaggle.com/tomasmantero/eda-warren-buffett-us-stock-companies)

## Context

**These are the publicly traded U.S. stocks owned by Warren Buffett’s holding company Berkshire Hathaway, as reported to the SEC.**

[Warren Edward Buffett](https://en.wikipedia.org/wiki/Warren_Buffett) is an American investor, business tycoon, philanthropist, and the chairman and CEO of [Berkshire Hathaway.](https://en.wikipedia.org/wiki/Berkshire_Hathaway) He is considered one of the most successful investors in the world and has a net worth of US$78.9 billion as of August 2020, making him the world's seventh-wealthiest person.

The information can be found in the [SEC 13F File.](https://www.sec.gov/Archives/edgar/data/1067983/000095012320009058/xslForm13F_X01/960.xml) The Securities and Exchange Commission's (SEC) [Form 13F](https://www.investopedia.com/terms/f/form-13f.asp) is a quarterly report that is required to be filed by all institutional investment managers with at least $100 million in assets under management. It discloses their equity holdings and can provide some insights into what the smart money is doing in the market.

After obtaining the list of companies in which Berkshire Hathaway invests, we proceeded to search the historical data of each company on NASDAQ.

## Content

In total there are 49 files in csv format. They are composed as follows:

- 45 files contain the U.S. stocks owned by Berkshire Hathaway. 
- 2 files contain the historical data from Berkshire Hathaway. Class A stock (BRK-A) and Class B stock (BRK-B).
- 1 file contain the list of all the companies with additional information.
- 1 file contain the SEC Form 13F.

## Column Description

Every company file has the same structure with the same columns:

- **Date:** It is the date on which the prices were recorded.
- **Close/Last:** Is the last price at which a stock trades during a regular trading session.
- **Volume:** Is the number of shares that changed hands during a given day.
- **Open:** Is the price at which a stock started trading when the opening bell rang.
- **High:** Is the highest price at which a stock traded during the course of the trading day.
- **Low:** Is the lowest price at which a stock traded during the course of the trading day.

The two other files have different columns names:

***Company List***

- **Name:** Name of the company.
- **Symbol:** Ticker symbol of the company.
- **Holdings:** Number of shares.
- **Market Price:** Current price at which a stock can be purchased or sold. (10/18/20)
- **Value:** (Holdings * Market Price).  
- **Stake:** The amount of stocks an investor owns from a company.

***SEC Form 13F***

**Name of Issuer, Title of Class, CUSIP Number, Market Value, Amount and Type of Security, Investment Discretion (Sole, Shared-Defined, Shared-Other), Other Managers, Voting Authority.**

You can find detail information of each column in the SEC [General Instructions Form 13F](https://www.sec.gov/pdf/form13f.pdf) in page 5.

## Acknowledgements

[SEC EDGAR | Company Filings](https://www.sec.gov/edgar/searchedgar/companysearch.html)

[NASDAQ | Historical Quotes](https://www.nasdaq.com/)

## Inspiration

Possible questions which could be answered are:

- **Of the companies that make up the Berkshire Hathaway portfolio, which are the most profitable companies?**
- **On February 21, 2020, Berkshire Hathaway suffered a large drop in its share price, what was the reason for this large drop?**
- **The presidential elections in the United States will be soon, do you think this will affect a particular company in the Warren Buffett portfolio and if so, which would affect them more?**

**[More Datasets](https://www.kaggle.com/tomasmantero/datasets)**

## License

This Notebook has been released under the Apache 2.0 open source license.
