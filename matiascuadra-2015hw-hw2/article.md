
### What polls can really tell us about election results

For most politicians polls are the best thermometer for electoral temperature, but how precise are they in reality? Can we rely on them as the best predictor for final election results? The answer to these questions, as many other important answers in life, is relative. After analyzing a comprehensive data base of US polls, we discovered a set of interesting features about polls for our country. The first interesting is that even when polls contain useful information, they should be taken with care. For example, if we simulate the 2014 senate elections and predict result based solely on polls this is what we get:

<img src= Hist1RepExpctSeats.png>

As we can see, our purely poll based projections are not accurate. The median number of seats that republicans get in our simulation is 20, and the probability of getting the real outcome, 23 seats for republicans, is around 2%.

**Why polls are a poor predictor?**

What the press tells us about the results of a poll are mainly averages, but within the construction of the average there is a great degree of uncertainty, which depends on variables related to the design of the survey, such as the number of people who was interviewed and/or the type of questions that were asked. One of the popular measures that statisticians use to account for part of the uncertainty is the margin of error. Other very important factor that could affect the predictive power of a poll is how old it is, people tends to change opinions frequently and during campaign period voters' behavior can be highly dynamic. Then, what happens if we correct the information in polls by these two concepts? Well, results improve a little bit but not that much, our median outcome will be 21 seats for the republican party, and the probability of the real outcome will be around 6%, it is an improvement but predictions are still poor.

**If polls are not very good predictors, how can we improve?**

First we should inspect how polls results look against the real outcome and see if we can detect any anomaly. For example when we compare 2014 senate polls against actual results, we detect a clear anomaly:

<img src=spread1.png>

Polls tend to under estimate results. In the graph above we can see that, generally, wining spreads are bigger than what polls estimated, maybe adjusting for this fact could improve polls’ predictive power. Another way to improve would be to incorporate more ingredients to our recipe, for example, not only use polls to predict but add additional features. After a few analyses on the data, we realize that there is maybe a feature that could help to improve our predictions, this feature is incumbency. After the 60’s, incumbency started to grow in terms of predictive for the next election, seems that there is a trend in which incumbent candidates have higher chances to get reelected.

<img src=pValuesIncumb.png>

Blue dots getting down the red line mean that through time the certainty of an incumbent effect has been increasing. So, maybe if we incorporate the idea of incumbency in our projections we can improve. Besides incumbency, we decided to add two more features in order to improve predictions: the results in the previous election and if the party in power at the time of the election was republican or democrat. So, do our predictions improve after these additional features?

<img src=Hist2RepExpctSeats.png>

Yes, they improve! Now our median simulated outcome is 22, and the probability of getting the real outcome is above 10%. But we would still like to have a median simulated outcome of 23, and a probability for this outcome as high as possible.

**How can we improve further?**

A nice experiment would be to add relevant demographic features to our predictions. Maybe, republicans and democrats could have better chances depending on the demographic characteristics of each state.

As we can see, polls can give us useful information to predict results. But we should not take this information literally, some adjustments to it need to be made, also, we can improve our predictions by using not only polls’ information but also some additional features, such as incumbency, previous results and the political party in power at the time of the election. Finally, our predictions could improve even further if we use some state demographic variables