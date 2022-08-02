# Project_2
# Primary application file

Produce a Google Colab file to compare four psychedelic stocks, a psychedelic ETF, and S&P 500 comparing them on volatility, profits, and cumuluative profits.  The psychedelic stocks are Mind Medicine (MNMD), Cybin Inc (CYBN), ATAI Life Sciences (ATAI), and Compass Pathways PLC (CMPS).  The ETF is PSYK ETF (PSYK) and it has 59,592 shares in 26 different psychedelic stocks with holdings of $94,651 including $2,509 in cash as of 8/1/2022.  The Standard and Poor's 500, or simply the S&P 500 (SPY), is a stock market index tracking the stock performance of 500 large companies listed on exchanges in the United States. It is one of the most commonly followed equity indices.


---

## Technologies

The following Technologies were used to develop this program:

Python 
    Version 3.9.7

Terminal
    Version 2.12.5 (444)

Visual Studio Code
    Version: 1.66.2 (Universal)
    Commit: dfd34e8260c270da74b5c2d86d61aee4b6d56977
    Date: 2022-04-11T07:49:20.994Z
    Electron: 17.2.0
    Chromium: 98.0.4758.109
    Node.js: 16.13.0
    V8: 9.8.177.11-electron.0
    OS: Darwin x64 21.4.0
    
Jupyter Lab 
    Version 3.2.9
    
Google.colab
    


---

## General information about analysis.

The Lesson consists of three technical deliverables:

Preprocess data for a nerual network model.

Use the model-fit-predict patten to complile and evaluate a binary classification model.

Optimize the model.



First you have to prepare the data for a nerual network model.  You create a data frame using the applicant data csv file.  Then drop EIN and NAME columns from the file since they are not needed for the model.  You then encode the data set's variables using one hot encoder.  After that numerical_variables_df and encoded_df data frames are concatenated to add numberical variables from original data frame to match the one hot encoded data frame.  You then prepare the X and y data frames and run a train_test_split function.  You will then need to scale the data.  Now we are ready to compile and evaluate a binary classification using a neural network.

The first neural network "Original Model Results" used all of the input features and the first hidden layer of 25 nodes and a second hidden layer of 12 nodes and used the "relu" activation.  We then compiled the model using binary crossentropy as the loss, optimizer equal to adam, and metrics equal to accuracy and fit the model using 50 epochs.  The results were 61.25% loss and 73.01% accuracy.  We then created an HDF5 file called AlphabetSoup.hd and saved it in our Resources directory.

The next step was to run an Alternative Model 1 and in this model we used all inputs for number of input features then used only one hidden layer of 58.  The hidden layer we used "relu" as activation and "sigmoid" activation in the output layer.  The results improved, loss decreased to 55.64% and accuracy increased to 73.15%.

Alternative Model 2 I was hoping to increase accuracy by adding more nodes to hidden layer 1 along with adding two addtional hidden layers from Alternative Model 1.  Using "relu" on the three hidden layers and "sigmoid" on the output layer.  Also wanted to increase accuracy by running additional epochs increasing the amount from Alternative Model 1 at 50 to 110 for Alternative Model 2.  Loss was worse slightly going from 55.64% in Alternative Model 1 to 59.27% in Alternative Model 2.  However, accuracy slightly increased from 73.15% in Alternative Model 1 to 73.17% in Alternative Model 2.  

After comparing the two alternative models you then create a HDF5 file and save them to Resources directory for Alternative Model 1 (AlphabetSoup_A1.hd) and for Alternative Model 2 (AlphabetSoup_A2.hd).



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

---

## License

[MIT](/license.txt)
