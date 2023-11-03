# A-B-Testing and ML
# Project objective
This aids an e-commerce business in determining which version is more well-liked by consumers and also reveals the relationships between each variable, helping them decide whether to roll out the new page, stick with the old page, or maybe extend the trial. This project aims to teach you how to use machine learning and A/B testing techniques.
* Methodology Approach:

  - Calculated Probability: 
    1. Calculate the proportion of users converted.
    2. Group the dataset with treatment into with/without new_version.
    3. Check if there is a duplicated and then drop it.
    4. Compute the probabilities for each assigned group.
  
  - A/B Testing: 
    1. Calculate required probabilities for A/B testing.
    2. Visualize the results with histogram plot for easy understanding.
    3. Compute the p-value and interpret the results into business words.
    4. Apply A/B testing with statistics package to know the testing results. 
  
  - Modeling Approach: 
    1. Utilize **Logistic Regression** methodology for a **categorical** based dataset.
    2. Summarize the Logistic Regression model.
    3. Merge with countries data and then summarize the model again.
    4. Test with more factors and interpret the results into business words.
### Conclusion:

  - From the results of **Calculated Probability**, there are more than 50% of users willing to land new_pages which makes the model more convincing and meaningful. Although only around 11.96% of users are willing to convert to the new_pages version, the result is still acceptable in the business world. Furthermore, the probability of an individual received the new page in either "control" or "treatment" groups are around 12% which means not only the size of both groups are similar but the conversion rates are close. Therefore, I can distinguish the design of this experimental model is **strong and persuasive**.
  
  - From the results of **A/B Testing**, p-value is around 9.6% which is higher than Type I error(5%); therefore, I should **fail to reject the null (H0)**. In addition, I can tell the actual p-value of control group is higher than the treatment group during the calculation which means **no overfitting**. On the other hand, since old verison has higher p-value than the new one, **I should keep the old version and do not change to the new version**. Meanwhile, since the probabilities of using new_pages and old_pages are the same, there is **no bias** here..
  
  - From the results of **Modeling Approach**, **Logisitc Regression** is an excellent choice in this case because the response variables are **Categorical Variables**. Moreover, the result will be stronger and more convincing with new variables added such as **'timestamp'**. More specifically, I can classify this factor into **'morning', 'afternoon'** and **'evening'**. Also I can classify them as **'weekday'** and **'weekend'** for better performance. On the other hand, it will make regression model more complex and I need to check it carefully to see if variables are dependable with each other. If yes, I need to add **higher order term** to get the better prediction results. Otherwise, the results should be trustworthy.
