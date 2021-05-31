
# Recommendations_with_IBM
This project is related to creation a recommendation system for IBM Watson Studio platform. It analyzes the interactions that users have with articles on the IBM Watson Studio platform, and make recommendations to them about new articles you think they will like. It involves recommender system using FunkSVD & SVD techniques.

Below mentioned graph depicts the corelation between number of Latent features and test data accuracy of the model.

![image](https://user-images.githubusercontent.com/77229486/119861526-1fa4d480-bf35-11eb-9af9-41d8184efe2d.png)

# Summary:

1) There is very less data points (only 20 users) for testing.

2) The accuracy of train data increases with number of latent features.

3) The accuracy of test data decreases with increasing the number of latent features, could be due to less data points.

4) Latent features close to 100 seems to be the critical point where rate of accuracy (slope) changes.

5) The accuracy may not be a good parameter to judge about the effectiveness of this recommender model due to typical dataset where only 20 user IDs are common between training and test dataset which is hardly 0.4% of the total unique users.

6) Additionally We can try Content based and collaborative based recommender models for testing the accuracy.

7) A/B testing method can be used to test the effectiveness of the recommendation engine in practice.The two groups can be separated based on cookies enabled diversions for equal splits. Group 'A' can be provided with only the rank based recommendations while the 'B' group would see only the user-item matrix as recommendation.

8) For evalution matrix, We can record rate of clicks (ratio of Total no. of clicks & Total no. of cookies in group B) on the recommended articles from the recommendation section or time spent rate on article after click while running our experiment.

9) In an ideal case, both the clicks rate and time spent rate should increase with the new recommender ; a statistically significant negative change should be a sign to not deploy the change. However, if only one of our metrics shows a statistically significant positive change we should be happy enough to deploy the new recommender model.
