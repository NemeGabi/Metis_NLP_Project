NLP - Project



On 15/06/2021 the Hungarian Government passed a law that aim was to fight against pedophilia but it has a supplementation paragraph about “kids right sexual education” that seems to target something totally different. 
That part of the law regulates that in no media can appear any "non-traditional" sexual relationship what any underage audience has opportunity to watch as they believe that this kind of "provocation" can cause damage in the kids healthy mental progress and might "confuse" them under a certain age. The law includes other new restrictions about the sexual education what the school can provide for the children under the age of 18.

Despite of the Europe wide (worldwide) protest the law came into force on 08/07/2021. The law has damaging effect on the LGBTQI communities and encouraging for the conservative/extreme groups.

The goal of my project to analyze the tweets posted the week after the law came to force and see how the topic of the tweets changed during the 7 days.

The dataset of tweets were exported from Twitter and after the cleaning and pre-processing almost 1500 tweets were ready for modeling.


I used the CountVectorizer to get the document-term matrix. Then NMF topic modeling was chosen with 5 components, as it suits well for fairly short documents and more interpretable than PCA/SVD.

Please see below the word topic matrix variable values sorted by the 5 defined categories.


![Topic_modeling](https://raw.githubusercontent.com/NemeGabi/Metis_NLP_Project/main/Topic_modeling.png)


For the first look, it seems topic 4 is about the tweets related to the coronavirus. The other 4 topics are close to each other further model tuning is necessary to get better defined topics out of them.

For further work I would like to amend my model until the differences between the topics are more significant, and then analyze day by day how the topic appearance changed during the selected period of time.



