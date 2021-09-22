# Project proposal for interpreting the relationship between Non-Fungible Tokens ("NFTs") and their prices

While valuation of artistic assets or collectibles in general are not standardized in process as well as, say, regulated financial products are and in large part based on subjectivity, this project aims to find whether there are any features that makes a Non-Fungible Token more expensive than another. 

Non-Fungible Tokens ("NFTs") are 'digital assets' stored on certain blockchain ledgers such as Ethereum and can be 'minted' as almost anything from short films to virtual cannabis farms. The interest in this space among investors has been around digital arts and sports collectibles recently, as cryptocurrency asset prices reached newer heights, and often in connection with their extravagant price tags. The underlying technology behind NFTs is designed to be able to verify originality of a digital artwork and secure record of ownership through records on a blockchain ledger. 

NFTs have primary and secondary markets where they are bought and sold like any other artworks. The project will attempt to quantify any relationships between NFT valuations and their features, if at all, by analyzing recent primary and secondary NFT transaction details from various public sources in the manner described below.

- Data:
  - Primary dataset will be scraped and compiled from websites with NFT transaction information, including but not limited to sites such as SuperRare (https://superrare.com/), Foundation (https://foundation.app/), NBA Top Shop (https://nbatopshot.com/), Open Sea (https://opensea.io/), and Coinranking.com (https://coinranking.com/). 
  - Each rows of about 1,000, will represent an individual NFT artwork
  - Each columns of about 10 or more features, will include latest sale price (the target value), art dimension, art type (e.g. animation, moving, real, abstract, has character/subject), days since creation, edition #, secondary transactions information (frequency traded in per days since created, max price change in %, median price change in % between transactions), concurrent Ethereum price (at the time of latest sale in US$ and price change in % vs. previous all-time-high price)

- Algorithms:
  - Exploratory data analysis techniques and visualizations for surveying the datasets
  - Linear regression model and validation techniques to interpret any patterns within the data

- Tools:
  - BeautifulSoup and Selenium for data collection (web scraping)
  - Matplotlib, Seaborn, Numpy, pandas and others for data manipulation
  - Scikit-learn for linear regression model

- Minimum viable product: 
  - Linear regression model output (e.g. coefficients, R2, etc) using subset of data and interpretation of such outputs in the context of the target variable
