# Amazon-Sentiment-Analysis-NLP
We will train a Naive Bayes classifier to predict sentiment from thousands of Amazon Reviews. This project could be practically used by any company with social media presence to automatically predict customer's sentiment (i.e.: whether their customers are happy or not).

Description:

This project performs sentiment analysis on Amazon customer reviews to predict customer feedback. It uses Python, pandas, numpy, seaborn, matplotlib, and scikit-learn to process and analyze the text data.

Actions:

Data Loading and Exploration:
Loads the dataset (amazon_reviews.csv) into a pandas DataFrame.

Explores the data by displaying the first few rows, checking data types, and generating descriptive statistics.

Handles missing values (if any) using a heatmap to visualize nullity.

Data Cleaning and Preprocessing:
Removes the rating column as it is not needed for the analysis.
Calculates the length of each review and stores it in a new column.
проводит предварительную обработку текста, включая удаление знаков препинания, стоп-слов и преобразование в нижний регистр.
Exploratory Data Analysis (EDA):
Visualizes the distribution of review lengths using a histogram.
Examines the balance of positive and negative feedback using a count plot.
Generates word clouds to visualize the most frequent words in both positive and negative reviews.
Model Training and Evaluation:
Splits the data into training and testing sets.
Converts the text data into a numerical format using CountVectorizer.
Trains a Multinomial Naive Bayes classifier on the training data.
Predicts the sentiment on the test data.
Evaluates the model's performance using a confusion matrix and a classification report.
Model Metrics and Conclusion:

The Multinomial Naive Bayes model achieved the following performance on the test set:

Accuracy: 94%
Precision:
Negative feedback: 68%
Positive feedback: 95%
Recall:
Negative feedback: 39%
Positive feedback: 98%
F1-score:
Negative feedback: 49%
Positive feedback: 97%
The model performs very well at predicting positive feedback but has a lower precision and recall for negative feedback, which suggests it has more difficulty in correctly identifying negative reviews.    

