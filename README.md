# Twitter-Emoji-Prediction-Project

This project uses the Twitter Emoji Prediction dataset from Kaggle, which consists of tweets paired with emojis that reflect the context or sentiment of each post. Although the precise data collection method is not specified, the dataset was likely gathered using the Twitter API and preprocessed to emphasize the relationship between tweet text and emoji labels. It captures informal language, slang, and typical emoji usage found on social media.

### Files used:
- train.csv: for model training and validation
- test.csv: for final evaluation on unseen data
- Mapping.csv: provides the mapping between emoji symbols and their numeric labels

This dataset is well-suited for training deep learning models that predict the most appropriate emoji for a given tweet.

### Identifying a Deep Learning Problem
This task is a multi-class text classification problem: given a tweet, predict the correct emoji from a fixed set of labels. To address this, three distinct deep learning architectures are explored, each implemented in a separate Jupyter notebook:
- LSTM: Captures sequential structure and temporal dependencies in the tweet text.
- GRU: A simpler alternative to LSTM with faster training while still modeling sequences effectively.
- TextCNN: Uses convolutional layers to extract local n-gram features and position-invariant text patterns.

The objective is to compare these models in terms of prediction accuracy, training time, and ability to generalize. The comparison aims to identify which architecture is best suited for predicting emojis based on short, informal text inputs like tweets.
