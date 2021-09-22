# Project proposal for interpreting the relationship between Non-Fungible Tokens ("NFTs") and their prices

While valuation of artistic assets in general are not standardized in process and in large part based on subjectivity, this project aims to find whether there are any features that makes a Non-Fungible Token more expensive than another. 

Non-Fungible Tokens ("NFTs") are [XXXXXXXXXXXXXXXX] and 
NFTs have gained significant fame recently, as cryptocurrency asset prices reached newer heights, and often in connection with their extravagant price tags. The underlying technology behind NFTs is designed to be able to verify originality of a digital artwork and confirm its rightful owner(s) through records on a distributed ledger. [Some NFT buyers] would argue that this ability imbues value in artworks of NFT format. 

NFTs, although traded via different channels, have primary and secondary markets where they are bought and sold like any other art pieces. By analyzing recent primary and secondary NFT transaction details from various public sources in the manner described below, the project will be quantifying any relationships among NFT valuations and their features, if at all. 

- Data:
  - Primary dataset will be scraped and compiled from websites with NFT transaction information, including but not limited to sites such as SuperRare (https://superrare.com/), Foundation (https://foundation.app/), NBA Top Shop (https://nbatopshot.com/), Open Sea (https://opensea.io/), and Coinranking.com (https://coinranking.com/). 
  - Each rows of about 1,000, will represent an individual NFT artwork
  - Each columns of about 10 or more features, will include latest sale price (the target value), art dimension, art type (e.g. animation, moving, real), days since creation, edition #, secondary transactions information (frequency traded in per days since created, price change in % max, price change in % median), concurrent Ethereum price (at the time of latest sale and price change in % vs. previous all-time-high price)

- Algorithms:
  - Exploratory data analysis techniques and visualizations for surveying the datasets
  - Train linear regression model and interpret any patterns within the data
  - Cross-validation for testing

- Tools:
  - BeautifulSoup and Selenium for data collection (web scraping)
  - Matplotlib, Seaborn, Numpy, pandas and others for data manipulation
  - Scikit-learn for linear regression model

- Minimum viable product: 
  - Linear regression model output (e.g. coefficients, R2, etc) and interpretation of such outputs in the context of the target variable
