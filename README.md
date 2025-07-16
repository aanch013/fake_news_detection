# Fake News Detection

In this project, I developed a machine learning-based Fake News Detector that classifies news articles as FAKE or REAL based on their textual content. The goal was to address the growing problem of misinformation by building a tool that is able to automatically assess article credibility.

Using the Fake and Real News dataset from Kaggle, which contains labeled news articles with titles and full text, I performed end-to-end NLP processing, including data cleaning, exploratory data analysis, feature extraction with TF-IDF vectorization, and classification modeling.

I started by exploring and cleaning the dataset by observing class balance, checking for missing values and examining the articles' characteristics. The class distribution was somewhat balanced between fake and real news articles. I also engineered features such as word counts and character counts to get a better understanding of the structure of articles and identify potential trends and differences between the classes. This analysis revealed that fake news articles and real news articles had similar distributions in terms of text length, suggesting that textual content rather than length would be more informative for classification.

I applied TF-IDF vectorization for feature engineering to transform the article texts into numerical features, capturing the importance of words while reducing the impact of commonly used terms. Using these features, I trained a Logistic Regression classifier as a baseline model. I chose Logistic Regression because of its interpretability, efficiency, and strong performance in text classification tasks with high-dimensional sparse data.

The model achieved an overall accuracy of 92% on the test set. Precision and recall were both high and balanced across classes, with precision of 93% and recall of 90% for real news, and precision of 90% and recall of 93% for fake news. The ROC AUC score was approximately 0.916, indicating excellent discriminatory ability. These results demonstrate that the model effectively distinguishes between fake and real news, with a low rate of false positives and false negatives.

<img width="481" height="183" alt="Screen Shot 2025-07-16 at 3 06 57 PM" src="https://github.com/user-attachments/assets/1199e598-936e-40c2-9e2d-c4da86192513" />
