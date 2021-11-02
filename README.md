# Legoland Malaysia Review Analysis

## <p align="right">[Portfolio Main Page](https://github.com/WengWeng0410/Weng_Portfolio)</p>

Sentiment analysis can be a key indicator of customer satisfcation or customer experience on the product or services that they consumed. In fact, customer experience is the key to business success. With a positive experience, more than 85% of customer will return or purchase more. However, a bad experience may result a drop of a product or brand. Hence, poor customer experiences can be costly. 

In this project, reviews on the visitation experience to Legoland Malaysia are analyzed. Suggestions on the change on the business are also provided based on the findings from the analysis. 

**Business Question**: What are the topics commented by the visitors after visitation to Legoland Malaysia? And what are the sentiments of the visitors towards experiences with Legoland Malaysia?

Works done as follows

* Perform reviews gathering from TripAdvisor
* Perform data cleaning on the reviews gathered  
* Develop a LDA model to identify the topics discussed by the visitors based on their experiences with Legoland Malaysia

## Code and Resources Used

**Python Version:** 3.7 <br>
**Packages:** numpy, pandas, seaborn, matplotlib <br>
**IDE:** Jupyter Notebook <br>
**Dashboard Software:** Google Data Studio <br>
**Dataset:** from [Tripadvisor](https://www.tripadvisor.com.my/Attraction_Review-g298278-d3491018-Reviews-Legoland_Malaysia-Johor_Bahru_Johor_Bahru_District_Johor.html) <br>

## Data Gathering

The dataset used in this project is gathered through Tripadvisor website. Selenium and BeautiSoup packages are used to crawl data from the searched results (keyword used: Legoland Malaysia). Data that gathered are review title, review as well as the rating rated. A total of 5069 reviews have been gathered and save in csv format. 

## Data Cleaning

In this stage, the reviews are clean by considering the following;

* convert all the characters to lower case
* remove non-alphabet and numbers
* remove stopwords
* N-gram (Bigram/Trigram) is also used to identify words that often show up together

