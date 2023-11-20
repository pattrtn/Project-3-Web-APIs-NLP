# Project-3-Web-APIs-NLP-

#### Problem Statement:
Marketing student who want to develop NLP for analyzing the competitive dynamics between Samsung and Apple to understand market trends and the factors influencing consumer preferences in the global electronics industry.


#### Background: 
The rivalry between Samsung and Apple is a longstanding and prominent competition in the consumer electronics industry.

#### Objectives:
To develop NLP model that can automatically classify post into Samsung and Apple categories and see if can develop into another funtion that help gathering more data like classify customer sentiments for sentiment analysis or identifying emerging trends and topics in the discussions related to Samsung and Apple for market trend identification that would help with marketing research in the future.


---

#### Datasets:

* [Subreddit: r/samsung](https://www.reddit.com/r/samsung/)
* [Subreddit: r/apple](https://www.reddit.com/r/apple/)

---

#### Data Cleaning:
* Step 1 : Check duplicated data and null value : None
* Step 2 : labeling data by topic ‘Samsung’ & ‘Apple’
* Step 3 : Concat 2 dataframe , reset index ,create new column for year and month of the post and drop column ‘date’
* Step 4 : Check data balance & random drop data in apple 40%
* Step 5 : Text Cleaning
  - Remove HTML tags
  - Remove non-alphanumeric characters
  - Remove extra white spaces
  - Make all text lowercase
* Step 6 : Create new column for post length & word count
* Step 7 : Tokenizing
* Step 8 : Lemmatizing
* Step 9 : Stop Word Removal


---
#### Modelling
Model 1 : Logistic Regression
- Train Accuracy : 0.98313
- Test Accuracy : 0.90134
- Precision : 0.90020
- Recall : 0.90572
- F1 Score : 0.90295


Model 2 : Naive Bayes
- Train Accuracy : 0.87000
- Test Accuracy : 0.85696
- Precision : 0.85696
- Recall : 0.82866
- F1 Score : 0.85822

Model 3 : Random Forests
- Train Accuracy : 0.99405
- Test Accuracy : 0.88670
- Precision : 0.89351
- Recall : 0.88908
- F1 Score : 0.89129


#### Chose Model 1 For better score compare to others model
---

#### Conclusions
* NLP model have ability to classify post into the categories of Samsung and Apple with acceptable in a prediction model accuracy.So it can develop to classify more detail in future , for next step should be develop with similar data like categorize brand mentions for Samsung and Apple and classify customer sentiments expressed in reviews and social media comments.

---

#### Recommendations

Exploring more additional features, such as competitor mentions to identify and extract mentions of competitors in the text. Understanding how Samsung and Apple are discussed in comparison to each other and to other competitors can be informative.

