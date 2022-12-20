# NLP Mixed Sentiment Analysis based on Keyword Similarity Score

**Background**: Much research has been done for sentiment analysis on tweets, the analysis result represents public perception and are often used to provide guidance to political poll, commerical campaign, etc. This project will dive into the tweets following Queen Elizabeth's passing, and analyze public opinions to each British royal family members.

**Problem**: Tweet context often contains multiple opinions towards different subjects. An example is, 
> We all love and miss #QueenElizabeth, the passing of her is a loss for the whole world. #KingCharles is not ready to lead England out of this crisis.

Traditional ML approaches to sentiment analysis would evaluate the context together, which might simply classify this text as neutral and lose critical sentiment information.

**Goal:**
The tweet above shall be classified as "positive" for "QueenElizabeth", and "negative" (or "neutral") for "KingCharles".

**Innovation**: 
- Use Local Interpretable Model-Agnostic Explanations (**LIME**) to extract top keywords (also referred to as features) with the highest **similarity score** towards tweet labeling for each tweet in the entire training dataset.

- Calculate sentiment score **for each subject (person)** in tweet, based on **keyworkd score** and the **relative distance** between keyword and subject. The sentiment score is further used to predict the subject sentiment.

| file                                   | description                                                             |
| -------------------------------------- | ----------------------------------------------------------------------- |
|TweetDataExtraction.ipynb               |Source tweet data using Twitter API                                      |
|KeywordBasedMixedSentimentAnalysis.ipynb|Classify sentiment seperately for each subject(person) from tweet dataset|


#### Let's get started!

