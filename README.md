# Algorithm_Trading
# Challenge 14 Machine Learning Trading Bot

# Data

![svm_report]("../Images/svm_report.PNG")
![svm_graph]("../Images/svm_graph.PNG)

Training data offset changed to 9 months.
```
# Select the ending period for the training data with an offset of 9 months
training_end = X.index.min() + DateOffset(months=9)
```
![training_report](Images/training_report.PNG)
![training_graph](Images/training_graph.PNG)

SMA adjusted to be much longer than the original.
``` 
# Set the short window and long window
short_window = 50
long_window = 200
```
![sma_report](Images/sma_report.PNG)
![sma_graph](Images/sma_graph.PNG)

Using Logistic Regression as our new classifier.
```
# Import a new classifier from SKLearn
from sklearn.linear_model import LogisticRegression

# Initiate the model instance
lr_model = LogisticRegression()
```
![lr_report](Images/lr_report.PNG)
![lr_graph](Images/lr_graph.PNG)
