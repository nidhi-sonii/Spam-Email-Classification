# Spam-Email-Classification
The Spam Email Classification system is the implementation of a machine learning based model, specifically using the Naive Bayes classifier, that allows us to categorize input mail as either spam or not spam. The training has been performed on a dataset provided, and implemented using NLTK with Python

# Dataset description. 
The dataset used to train the model is the Email Spam Classification Dataset CSV from Kaggle. The dataset contains 5172 rows, with 3002 columns The first column indicates Email name, and the last column has the labels for prediction : 1 for spam, 0 for not spam. The remaining 3000 columns are the 3000 most common words in all the emails, after excluding the non-alphabetical characters/words

# Training the Model
The model is trained using Naive bayes classifier, it works by categorizing an email being spam or not by calculating the likelihood of its words appearing in spam or non-spam emails, and assumes all words contribute independently to the classification.
Since the dataset provided to us is of a moderate size, it is assumed that Naive Bayes will perform well because it assumes feature independence, which often works well for text data (like words in an email).
After training the model, it is used to make predictions. These predictions can be evaluated using the following metrics:

# Evaluation Metrics:
Accuracy: This is the number of correctly classified samples out of the total samples, showing overall model performance.
Confusion Matrix: This summarizes the true positives, true negatives, false positives, and false negatives of a model's predictions to evaluate performance, that is, precision, recall and f1 score.
F1 Score: Balances between precision and recall, to show the effectiveness of the model.

# Using NLTK to preprocess the input email.
In this step, stop words are removed, and stemming is performed with the use of stemmer to preprocess the input email. After this, the email is broken down into tokens which are then passed into the model for prediction.

After passing the tokens through the trained model, it will be able to predict whether the tokens passed into it are spam or not
