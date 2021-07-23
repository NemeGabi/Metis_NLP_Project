NLP Project

The aim of my project to analyze tweets posted on the week after a "kid protection" law came into effect in Hungary on 08/07/2021. I created a dataset with posted tweets from Twitter and then cleaned, analyzed it and identified the positive or negative "motion" of the tweets. The results include information about the total number of tweets per topic and the daily breakdown of the topics with the information if it was a positive or negative tweet. This information can give me boarder view of the reaction that the law caused on international field.

Design

On 15/06/2021 the Hungarian Government passed a law that aim was to fight against pedophilia but it has a supplementation paragraph about “kids right sexual education” that seems to target something totally different group. 
That part of the law regulates that in no public media can appear any "non-traditional" sexual relationship or people who changed sex what any underage audience has opportunity to watch. They believe that this kind of "promotion" can cause damage in children healthy mental progress and might "confuse" them under a certain age. The law includes other new restrictions about the sexual education what the school can provide for the children under the age of 18, and requirements for the cover of the books that has "non-normal" content.

Despite of the Europe wide (worldwide) protest the law came into effect on 08/07/2021. 
The law has a very damaging effect on the LGBTQI communities and encouraging exclusion what is not acceptable in any democratic country.


Data

The dataset includes 1395 tweets that are scrapped from Twitter via Twitter API. The criteria of the selection is to have "Hungary" or "Hungarian" hashtags in the post. The tweets are posted between 07/07/2021 and 07/15/2021. The most frequent users in the dataset are news portals and the user with the highest follower group is the Human Right Watch with over 4.5 million followers.

After the dataset was generated, some pre-processing steps were taken to make sure its ready for effective modeling. During the cleaning process the below items were removed/changed: 
 - removed URLs, punctuation, numbers, stopwords, foreign characters caused words - starts with 'x'
 - changed to lowercase
 - remove "Hungary" and "Hungarian" words  


Algorithms

On the cleaned dataset with Countvectorizer the document-term matrix was created. Then non-negative matrix factorization (NMF) model was used for topic modeling. See below the ten separated topics that were identified:

 EU_HU relationship
 Anti_LGBT
 Poland
 Coronavirus
 Tourism
 Sex_edu
 Mix
 Book_censure
 International_news
 Weather

 On the identified topic's then sentiment analysis were done so it shows if the tweets have negative or positive content.


Tools

 - Data scrapping with Twitter API
 - Data cleaning and pre-processing in Python NLTK package
 - Sentiment analysis with TextBlob
 - Result are visualized in Tableau


Communication

Please see below the total sentiment score of the topic chart and the sentiment score per day per topic chart.

![Total_sent_per_top](https://raw.githubusercontent.com/NemeGabi/Metis_NLP_Project/main/Total_sent_score_per_topic.png)

![Sent_score_per_day_per_topic](https://raw.githubusercontent.com/NemeGabi/Metis_NLP_Project/main/Sent_score_per_day_per_top.png)



