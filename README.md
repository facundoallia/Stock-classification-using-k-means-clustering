# Stock classification using k-means clustering

This work presents an approach to use the K-means algorithm for stock classification, with the aim of helping investors to diversify their investment portfolios. It´s divided in 3 parts:

1. Clustering of stocks according to their average annualized return and average annualized volatility.

2. Clustering of shares according to their per (price-earnings ratio) and dividend rate

3. 3-dimensional analysis using the k-means++ algorithm using mean annualized return, mean annualized volatility and price-to-book ratio as a new dimension.

# Clustering of stocks according to their average annualized return and average annualized volatility.

We work with all the S&P 500 stocks. The S&P 500 consists of 500 companies representing all the sectors of the economy. The index covers only large-cap companies listed on the U.S. market, either the New York Stock Exchange or the Nasdaq. Because the S&P 500 represents the largest publicly traded companies in the U.S., it is considered one of the most widely quoted stock market indexes.

K-means clustering is an unsupervised learning algorithm used to group data points into clusters. In the context of creating 4 clusters of stocks using K-means algorithm, the algorithm will iteratively assign data points to clusters based on their similarity of characteristics, or "features", such as returns and volatility. The algorithm initially assigns the data points randomly to the clusters, and then calculates the centroid of each cluster, which is the mean of all the data points within the cluster. The algorithm then compares the data points to the centroid and reassigns them to clusters accordingly. This process is repeated until the centroid of each cluster remains relatively stable, at which point the algorithm stops and each cluster is assigned a label. The end result is a set of 4 clusters, each containing stocks that have similar returns and volatilities.

![return and volatility k-means clustering]((https://github.com/facundoallia/Stock-classification-using-k-means-clustering/blob/main/assets/ret_vol.png?raw=true))

The graph shows 4 clusters that were generated using a K-means algorithm with 2 variables: average annualized return and average annualized volatility. These variables are used to measure the risk and return of a stock. The 4 clusters represent 4 groups of actions with different levels of risk and return in the period under study.

Clustering is useful for identifying peer groups among stocks, thus allowing differentiation between stocks with different levels of risk and return. This is useful for investors looking to diversify their investment portfolios, as it allows them to identify groups of stocks with different levels of risk and return.

Investors could use the 4 clusters to select a mix of stocks with different levels of risk and return based on their investment objectives. This will help them diversify their portfolio and reduce the risk of their investment, since they will be investing in a variety of assets with different levels of risk.

# Clustering by P/E and dividend rate

It is possible to apply a clustering similar to the one performed previously, exchanging the variables Annualized Average Return and Annualized Average Volatility for PER (Price-Earnings Ratio) and Dividend Rate. In this way we could differentiate between “value” companies and “growth” companies.

![return and volatility k-means clustering]([(https://github.com/facundoallia/Stock-classification-using-k-means-clustering/blob/main/assets/ret_vol.png?raw=true](https://github.com/facundoallia/Stock-classification-using-k-means-clustering/blob/main/assets/per_div.png?raw=true)))
