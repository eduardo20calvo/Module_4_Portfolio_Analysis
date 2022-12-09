## Portfolio_Analysis

The purpose of this analysis is to analyze and visualize the major metrics of the portfolios, and determine which portfolio outperformed the others. The major metrics includes Volatility, Returns, Risk and Sharpe Ratio. Several CSV files contain the historical daily returns of several portfolios: some from a fictional firm's algorithmic portfolios, some that represent the portfolios of famous "whale" investors like Warren Buffett, and some from the big hedge and mutual funds. Then this analysis was used to create a custom portfolio of stocks and compare its performance to that of the other portfolios, as well as the larger market S&P 500 Index.

## Prepare the Data

To begin, three of the CSV files ("whale_returns", "algo_returns", and "sp500_history") were read into a DataFrame. The main purpose of this section is to clean and preprare the data by indexing the "Date" column, dropping any nulls in the dataset and in the case of the "sp500_history" CSV file, calculating the daily returns of the data to reduce the variance amongst the data. Lastly, the three DataFrames were concatenated into one DataFrame.

## Conduct Quantitative Analysis

The daily returns of all the portfolios were plotted in a graph to show the comparison amongst them:

![Screenshot 2022-12-08 201646](https://user-images.githubusercontent.com/104874384/206600978-4abbce10-d005-4445-99de-52ae97c17c23.png)

The cumulative returns of all the portfolios were then calculated and plotted into the graph below:

![Screenshot 2022-12-08 201834](https://user-images.githubusercontent.com/104874384/206601201-3dab7397-7b16-40f0-a506-508bed760ca4.png)

A risk analysis was then performed for each of the portfolios. A box risk was created to visually show the risk of each of the portfolios:

![image](https://user-images.githubusercontent.com/104874384/206601434-0112d29f-0b8e-4aa5-8c9c-c88ada155ff2.png)

The standard deviation of each portfolio was calculated to show which portfolios were riskier than the S&P 500 index. Findings conclude that TIGER GLOBAL MANAGEMENT LLC & BERKSHIRE HATHAWAY INC. were risker than the S&P 500 portfolio. 

![Screenshot 2022-12-08 202355](https://user-images.githubusercontent.com/104874384/206601773-939d5553-265e-4fd3-90a4-2aed5cfce7a7.png)

The annualized standard deviation was also calculated:

![Screenshot 2022-12-08 202700](https://user-images.githubusercontent.com/104874384/206602138-8a1fc270-4a81-4155-a392-f07b5b9718a4.png)

The rolling 21-day standard deviation was then calculated and plotted in a line graph for all the portfolios:

![Screenshot 2022-12-08 202751](https://user-images.githubusercontent.com/104874384/206602243-867b69d1-445b-4623-8585-e95e23171a8e.png)

The correlation of all the portfolios were calculated and organized in a correlation matrix:

![Screenshot 2022-12-08 202923](https://user-images.githubusercontent.com/104874384/206602381-771da327-6dc4-49e4-b5e8-94d0bd239fff.png)

The exponentially weighted average of all the portfolios were calculated and plotted in a graph:

![Screenshot 2022-12-08 204249](https://user-images.githubusercontent.com/104874384/206603945-55877e1a-d89c-4ade-8110-8d99af005f90.png)

Last but not least, the sharpe ratio was calculated and plotted in a bar graph:

![Screenshot 2022-12-08 204418](https://user-images.githubusercontent.com/104874384/206604117-391d8a7d-79e0-41e5-a836-e43a285d8ec3.png)

Based on all the calculations and graphs created, Algo 1 portfolio did outperform the S&P 500 and the whales portfolios while Algo 2 did not outperform S&P 500 and BHI portfolios.

The Apple, Costco, and Google historical stock prices were imported from a CSV file and using the same steps prior, all metrics were calculated and graphed to compare the results from the other portfolios.

![Screenshot 2022-12-08 204834](https://user-images.githubusercontent.com/104874384/206604665-6376658f-6253-495c-82d6-eb8ee9b88d9f.png)

![Screenshot 2022-12-08 204902](https://user-images.githubusercontent.com/104874384/206604804-d939cb31-c359-402c-bc56-aec49401f211.png)

![Screenshot 2022-12-08 204934](https://user-images.githubusercontent.com/104874384/206604956-e773060f-6298-4b15-bc86-f51ed888a993.png)

![Screenshot 2022-12-08 205023](https://user-images.githubusercontent.com/104874384/206605089-d334fba6-3ff0-4ccc-8382-c7be28dd1d82.png)

Based on the results, my portfolio outperforms every other portfolio except the Algo 1 portfolio.
