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
**Packages:** numpy, pandas, seaborn, matplotlib, nltk, SentimentIntensityAnalyzer, gensim <br>
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

## EDA

#### Reviews Topics Distribution 
![](/images/Topic_Distribution.png)

#### Keywords for Each Topic
![](/images/KeywordsforEachTopic.png)

#### Topics Distribution Based On Ratings
![](/images/TopicDistributionBasedOnRatings.png)

#### Topics Distribution Based On Sentiments
![](/images/TopicDistributionBasedOnSentiments.png)

<br> Based on the findings, it can be seen that the reviews are with high ratings (3 to 5). Reviews with low ratings (1-2) are minimal. Besides, the reviews are with very high positive sentiments as compared with neutral and negative sentimens.  <br>

## Model Building and Discussion

Topic modeling is used to identify the topics commented by the visitors. The model used is Latent Dirichlet Allocation (LDA). The model is finally group the reviews into 5 topics as follows:

**Topic 1: Park (Theme/Water Parks)**

As for topic 1, it covers the recommendation on the visitation to Legoland Malaysia as well as summary of the visitors' experiences with legoland Malaysia. The reviews range from the overview, condition of the parks, hospitality/services provided by the staff, suggestion on planning on the visitation and food. 

**Topic 2: Park Rides**

As for topic 2, it covers the experiences of the visitors on the rides in the park, water park, sea life as well as other attractions located in the legoland.

**Topic 3: Transporation to Legoland**

As for topic 3, the reviews covers mainly on the travelling mode to Legoland Malaysia. 

**Topic 4: Recommendation on Leogland to Kids**

For topic 4, it mainly covers the reviews on kids/children experiences with legoland Malaysia as well as the family and age group that suitable to Legoland Malaysia. Food choices and prices are also discussed. 

**Topic 5: Kids Experience with Legoland**

For topic 5, the visitors shared their experiences on the rides and attraction on Legoland Malaysia. 

Generally, the reviews are positive, satisfied with the services provided, rides and attractions in the parks. Poor comments on staff attitude/services and the maintenace of the parks are minimal. However, Legoland Malaysia may look into continuous training program to the staff and a proper maintenance schdule on the rides. Besides, deals to improve the visitation of visitors from Singapore or other states can be considered to compensate the travelling time to Legoland Malaysia. But not to forget the visitors with origin from Johor! 
<br><br>
Other than that, Food choices provided in the parks can be improved by introducing more choices at a lower price. Many of the visitors commented that the food is overprived. Other than that, allowing outside food for kids with ages < 3 - 4 can be considered as the food provided in the park is not suitable for kids with ages < 3 - 4. <br>


