# Overview
The rise of platforms like Airbnb has transformed how people book accommodations, offering diverse options to suit various preferences and budgets. However, both hosts and guests face uncertainty regarding the future availability of listings. To address this, NLP techniques were implemented to predict whether an Airbnb property will be removed from the platform in the next quarter.

# Models and Techniques
The preprocessing steps involved cleaning and standardizing the text data, removing irrelevant elements, and lemmatizing words to their root forms. I also used Hugging Face's Transformers library's nlptown/bert-base-multilingual-uncased-sentiment model for sentiment analysis to gain insights from the comments, given that this model supports several languages. Then, I used techniques like Bag of Words (BoW), TF-IDF, GloVe, LaBSE, and XLM-R to transform the text data into meaningful features. These features were combined with numerical data for model training.
Various classification models were used both with undersampling and oversampling techniques to address class imbalance:
- Logistic Regression
- Multi-Layer Perceptron
- K-Nearest Neighbours
- Support Vector Machines
- Random Forest
- Gradient Boost Machines
- AdaBoost
- XGBoost
- LightGBM
- CatBoost

# Evaluation Metrics
In this project to predict Airbnb property unlisting, I faced the challenge of working with an unbalanced dataset, where the number of properties that get unlisted is significantly smaller compared to those that remain listed. To effectively evaluate the performance of the predictive models, I employed several metrics tailored to handle this imbalance and ensure accurate predictions.

### F1 Score
The F1 score is a critical metric for evaluating our models, particularly given the class imbalance in our dataset. Since the number of unlisted properties (positive class) is much lower than the listed properties (negative class), focusing solely on accuracy could be misleading.


