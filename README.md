## Twitter Sentiment Analysis of Apple and Google Products Using Natural Language Processing

# Business Understanding
In the fast-paced consumer technology market, corporate giants like Apple and Google receive thousands of social media mentions daily. For brand managers, product development teams, and public relations specialists, manually monitoring this volume is impossible.
This project develops a machine learning-driven sentiment analysis engine that automatically sifts through public tweets and classifies them into three distinct behavioral categories:

Positive Emotion: Highlighting consumer satisfaction, feature appreciation, or product excitement.

Neutral Emotion (No Emotion): Standard feature inquiries, objective tech news sharing, or non-emotional commentary.

Negative Emotion: Outlining software glitches, hardware complaints, or customer service frustrations.

By deploying this pipeline, brand management teams can instantly bypass general noise and focus their human engineering efforts exactly where public relations or operational interventions are needed most.

# Stakeholders

These are the people who will use or benefit from the results of this model:
Brand Managers (Apple & Google) – Monitor public perception and brand reputation.
Product Teams – Identify product issues, bugs, or feature feedback from users.
Customer Success / Support Teams – Understand customer complaints and improve response strategies.
Marketing Teams – Identify positive sentiment to amplify successful campaigns.
Business Executives – Use insights for strategic decision-making.
# Business Questions
What is the overall sentiment (positive, negative, or neutral) expressed in Tweets about Apple and Google products on Twitter?
Can a machine learning model accurately identify negative tweets to ensure that critical customer issues are quickly detected and addressed?
Which Apple and Google products or features generate the most positive and negative customer feedback?

# Project Objectives
# General Objectives
To develop a Natural Language Processing (NLP) model that automatically classifies Tweets about Apple and Google products into sentiment categories (positive, negative, and neutral) to support customer insight and decision-making.
# Specific Objectives
To clean and preprocess Twitter text data for sentiment analysis.
To explore and understand the distribution of sentiments in the dataset.
To transform text data into numerical features using NLP techniques such as TF-IDF.
To build a machine learning model that classifies Tweets into positive, negative, and neutral sentiment.
To evaluate the performance of the model using appropriate metrics such as F1-score, precision, and recall.
To identify and analyze negative Tweets for early detection of customer issues.
To generate insights on which Apple and Google products or features drive positive and negative sentiment.

# Methodology
# 1. Data Cleaning
The following preprocessing steps were performed:
Removal of missing tweet records
Removal of duplicate tweets
Conversion to lowercase
URL removal
Username and hashtag cleaning
Removal of punctuation and special characters
Whitespace normalization

# 2. Feature Engineering
Additional features were explored during analysis:
Tweet length
Character count
Word count

# 3. Exploratory Data Analysis (EDA)
The analysis included:
Sentiment distribution visualization
Tweet length versus sentiment analysis
Brand and product breakdowns
Class imbalance assessment
# 4. Text Vectorization
Tweets were transformed into numerical representations using:
TF-IDF (Term Frequency–Inverse Document Frequency)
This approach emphasizes important words while reducing the influence of commonly occurring terms.

# Machine Learning Models
The following classification algorithms were trained and evaluated:
Logistic Regression
Multinomial Naive Bayes
Random Forest Classifier
Linear Support Vector Classifier (Linear SVC)

# Model Evaluation
Models were evaluated using:
Accuracy
Precision
Recall
F1-Score

# Confusion Matrix
The workflow involved:
Train-Test Split (80/20)
TF-IDF Transformation
Model Training
Prediction

# Performance Evaluation
Model Deployment
The final trained model and vectorizer were saved using Joblib:
joblib.dump(model, "sentiment_model.pkl")
joblib.dump(tfidf, "tfidf_vectorizer.pkl")
A prediction function was also created to classify new tweets.

# Key Findings

Social media sentiment can be effectively classified using NLP techniques.
TF-IDF provides strong baseline text representations for sentiment analysis.
Traditional machine learning models remain effective for short-text classification tasks.
Negative tweets can serve as early indicators of customer dissatisfaction and product issues.

# Technologies Used
Python
Pandas
NumPy
Scikit-learn
NLTK
Matplotlib
Seaborn
Joblib
Jupyter Notebook

# Github link
https://github.com/simiyuclare26-source/Phase-4-Project.git

# Author
Nanjala Simiyu