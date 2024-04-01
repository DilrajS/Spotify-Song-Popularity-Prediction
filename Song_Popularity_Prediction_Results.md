## Predicting Song Popularity with Machine Learning: A Journey with Learnings

![Spotify Song Popularity Prediction Banner](images/sspBanner.gif)

This project explored the fascinating, yet challenging, task of predicting song popularity on Spotify using machine learning. The goal was to understand the relationship between a song's audio features and its popularity score.

**Approaching the Challenge: Data Exploration and Feature Selection**

![Distribution of Song Popularity](images/Distribution%20of%20Song%20Popularity.png)

The Spotify dataset provided a wealth of information about songs and their audio characteristics. To gain insights, I employed various data exploration techniques, including analyzing distributions, identifying missing values, and visualizing correlations between features.

![Correlation Matrix of Audio Features](images/Correlation%20Matrix%20of%20Audio%20Features.png)

A crucial step was feature selection. Correlation analysis revealed features like 'duration_ms' had minimal impact on popularity, so I removed them to streamline the model. Additionally, I addressed multicollinearity between 'loudness' and 'energy' by keeping 'loudness' as a representative feature.

**Building and Evaluating Machine Learning Models**

I implemented two machine learning models: a Decision Tree Regressor and a Neural Network. The Decision Tree provided a baseline understanding of the feature relationships. However, the Neural Network achieved a higher R-squared of 0.33 on the test data, indicating it captured a moderate portion of the variance in popularity. In comparison, the Decision Tree achieved an R-squared of 0.16.

**Key Learnings from Model Comparison**

The comparison between the Decision Tree and Neural Network models highlights the importance of model selection for complex prediction tasks. The Neural Network's superior performance (R-squared of 0.33 compared to the Decision Tree's 0.16) suggests it was better able to learn the underlying patterns in the data for predicting song popularity.

This finding emphasizes the strength of Neural Networks in capturing non-linear relationships between features, which might be present in audio data influencing song popularity.

**Learnings and Potential Improvements**

This project provided valuable insights into data exploration, feature engineering, and model selection for a complex prediction problem. One key learning was the importance of understanding the limitations of the data and the task itself.

Here are some areas for potential improvement:

- **Feature Engineering:** Crafting new features based on existing ones could potentially capture more nuanced relationships with popularity. For example, features combining elements of different audio characteristics might be more informative.
- **Hyperparameter Tuning:** The Neural Network architecture and hyperparameters weren't extensively tuned in this initial exploration. Techniques like GridSearchCV could be employed to identify a more optimal configuration for the specific dataset.
- **Exploring Different Model Architectures:** While the Neural Network showed promise, exploring other architectures like recurrent neural networks (RNNs) might be suitable for sequential data like music.

By delving deeper into these areas, the model's accuracy and ability to capture the nuances of song popularity could be further enhanced.

**Conclusion**

This project served as a springboard for exploring the challenges and opportunities in predicting song popularity with machine learning. The learnings gained about data exploration, feature selection, and model limitations are valuable takeaways that can be applied to future data science endeavors.
