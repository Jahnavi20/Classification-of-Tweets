# Classification-of-Tweets
## Introduction
## Methodology
## Word Cloud
## Model Architectures
## Model Comparisons
### RMSE
  ![image](https://user-images.githubusercontent.com/48169929/226206316-73b7dcc5-1dcc-435b-8f4d-54fd89d148ee.png)
### MAE
  ![image](https://user-images.githubusercontent.com/48169929/226206336-f83f867b-1044-42e9-bc88-7e8f5a82b28a.png)
* We have observed that for the Negative score, CountVectorizer() or TfidfVectorizer() are performing better that other models.
* We have observed that for the Neutral score, CountVectorizer() is performing better than other models.
* We have observed that for the Positive score, CountVectorizer() or TfidfVectorizer() are performing better that other models.
* We have observed that for the Compound score, CountVectorizer() is 
performing better than other models.
* We also observed that MAE for Positive and Negative Scores is less when compared to the MAE values for the Neutral and Compound scores.
## Conclusion
* From the RMSE and MAE values for the test data we can see that CountVectorizer() and TfidfVectorizer() have almost same values. 
* And also CountVectorizer() and TfidfVectorizer() are best models out of the 4 models as they have less RMSE and MAE values with good R squared values.
* Also these models are predicting Negative Score and Positive score more accurately than Neutral and compound Scores.
* Changing the hyper parameters also helped slightly but not to our expectations.
* Coming to the architecture, we have seen some improvements as we changed it.
* As we increase the number of layers, the performance has increased but not so high.
* Adding dropouts after NN layers helped to increase the R squared but not as expected. Still it is overfitting, but it helped.
* Reducing the patience value, batch size and limiting the batch size also helped in the improvement.
* Since, the data is very small, adding SimpleRNN layers to the model architecture gave slight improvement.
* The primary problem here is that the data we have is very small. It is only 4k tweets. But, the model is sightly better when the data size is increased from 2k to 4k tweets.
* So, increasing the data largely would improve the model performance in capturing the sentiments. 
* We can say that Deep learning models are able to steal the logic of the nltk SentimentIntensityAnalyzer() for atleast positive and negative scores.
* Rule-based models blindly follows more advanced rules. Deep-learning models doesn’t blindly tag keywords or ‘rules’. It infers meaning based on patterns between words and the wider context of the sentence and paragraph they sit within. 
* Deep learning models require more data as compared to rule-based models. Rule-based models can operate with simple basic information and data. However, deep learning models require full demographic data details.
