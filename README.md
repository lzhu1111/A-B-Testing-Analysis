# Customer Acquisition A/B Test Analysis

Disclaimer: “No similarity to actual persons or companies is intended or should be inferred.”

GameFun, world’s top developer of mobile games, conducted a display banners experiment with the goal of testing whether display banners increase sales on gaming subscription packages. Based on the data collected, I have conducted an analysis of the effectiveness of this social media campaign and evaluated results to recommend future test target customers with highest purchase rate and expected revenue. 

## Questions to consider
1. Most importantly, double check whether the A/B test is set up correctly (before running it)?
There must be no statistically significant differences between the control and test group. For example, use t-test to see statistical significance in income differences.
```
t1,p1 = stats.ttest_ind(control_group['income'],test_group['income'])

```
2. How "big" is the data? If the number of samples is extremely large, consider using effect size instead of p-value. 
3. Evaluate the average purchase rates in the test and control for different demographics. For exmaple, male vs. female, gamer vs. non-gamer.
4. Assess the expected revenue in the test and control for different demographics.
5. What is your recommendation to management? Should Game-Fun run this promotion again in the future? If yes, should Game-Fun offer it to all customers or a targeted segment. 

My take: The expected revenue from female gamers almost doubles that from all customers. Therefore, GameFun should run this promotion again in the future. However, rather than offering to all customers, the company should offer it only to a targeted segment with largest return, the female gamer population.


