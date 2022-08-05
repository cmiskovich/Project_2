# Project_2
# Primary application file

Produce a Google Colab file to compare four psychedelic stocks, a psychedelic ETF, and S&P 500 and predicting the closing price 90 days ahead.  The psychedelic stocks are Mind Medicine (MNMD), Cybin Inc (CYBN), ATAI Life Sciences (ATAI), and Compass Pathways PLC (CMPS).  The ETF is PSYK ETF (PSYK) and it has 59,592 shares in 26 different psychedelic stocks with holdings of $1,175,934 including $2,509 in cash as of 8/1/2022.  The Standard and Poor's 500, or simply the S&P 500 (SPY), is a stock market index tracking the stock performance of 500 large companies listed on exchanges in the United States. It is one of the most commonly followed equity indices.


---

## Technologies

The following Technologies were used to develop this program:

Python 
    Version 3.9.7

Terminal
    Version 2.12.5 (444)
 
 Git version 2.24.0.windows.2

Visual Studio Code
    Version: 1.66.2 (Universal)
    Commit: dfd34e8260c270da74b5c2d86d61aee4b6d56977
    Date: 2022-04-11T07:49:20.994Z
    Electron: 17.2.0
    Chromium: 98.0.4758.109
    Node.js: 16.13.0
    V8: 9.8.177.11-electron.0
    OS: Darwin x64 21.4.0
    
    
Google.colab
    


---

## General information about analysis.

We pulled data for the past year for the our four stocks (MNMD, CYBN, ATAI, and CMPS), along with the psychedelic ETF (PSYK), and also the S&P 500 (SPY).  After that we created data frames for each of them with a datetime stamp and closing price.  









---

## Information about datasets

Create the alpaca API object:

alpaca

Format current data as ISO format:

start_date, end_date

Set the tickers for psychedelic stocks and ETF:

psyche_tickers

Obtain 1 year worth of data for tickers:

psychedelics_stocks

Reorganize Dataframe and separate ticker data:

MNMD, CYBN, ATAI, CMPS, PSYK

Concatenate DataFrames for psychedelic stocks using MNMD, CYBN, ATAI, CMPS:

mind_trip_portfolio

Create DataFrame for psychedelic ETF:

psyk_psychedelics_eft

Create DataFrame for S&P 500:

sp_tickers


---

## Libraries used in analysis

os

requests

pandas

dotenv

alpaca_trade_api

hvplot

---

## Contributors


**Chris Miskovich**

Contact Information:

Email: cmiskovich@verizon.net

[LinkedIn](https://www.linkedin.com/in/christopher-miskovich-9a61b0234/) 



**Antiwan Maxwell**

Contact Information:

Email: antiwan.maxwell@outlook.com

[LinkedIn](https://www.linkedin.com/in/antiwan-maxwell-205a11233/) 



---

## License

[MIT](/license.txt)
