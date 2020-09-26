In this project my goal was to analyze A/B test results to help the company understand if they should implement new page, keep the old page, or perhaps run the experiment longer to make their decision.

### Approaches:
Part I 
- Probability of receiving the new page and converting

Part II - A/B Test 
- Setting up hypothesis and test conversion rate
- Performing the sampling distribution and ztest

Part III - Regression 
- Performing Logistic Regression to predict the conversion (based on the country and interaction between pages and country)

### Conclusion
In the first section of Part II, we assumed under the null hypothesis, 𝑝𝑛𝑒𝑤 and 𝑝𝑜𝑙𝑑 both have "true" success rates equal to the converted success rate regardless of page. For determining if the null is possible, we built sampling distribution and found confidence interval. The p-value was approximately 0.9. Based on the data, we fail to reject the Null hypothesis.

In the second section of Part II, we used the test for proportions based on the normal (z) test. Our computed p-value was 0.905 and z-score -1.31. Based on these results, we fail to reject our null hypothesis.

In Part III, as we wanted to predict only two possible outcomes, we used Logistic regression. We fit the regression model to see if there is a significant difference in conversion based on which page a user receives.

We included in our model another metric - countries where users live to see whether a country might affect the conversion rate. According to our results, we can say the country doesn't have a significant impact on the conversion of users.

According to these results, we can say that launching a new page would not be lucrative for the company. It is possible that the test has been cut off early, and therefore the results are skewed. On the other hand, it's very debatable that if the test were running for a longer time, the results would be different.

Perhaps the company should reconsider the design of the new page and implement new changes that would be more attractive and interesting for users, then rerun the test.
