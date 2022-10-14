# Mini Project - Tweet Emotion Recognition
Defina Ambarwati : [Github](https://github.com/definaa2412)
***

## About
  In this project, we are going to create a recurrent neural network and train it on a tweet emotion dataset to to recognize emotions in tweets. This is a multi class classification problem. We will be using TensorFlow as our machine learning framework.
  
## Dataset
  The dataset is used from [Hugging Face](https://huggingface.co/datasets/emotion) containing English Twitter messages with six basic emotions: anger, fear, joy, love, sadness, and surprise. This data consists of three data set, such as train data, validation data and test data with each total data 16000, 2000, 2000 respectively.
  
## Summary
### Data Preprocessing
1. Word Tokenization

$\qquad$ Splitting a phrase, sentence, paragraph, or an entire text document into smaller units called token.

2. Padding and Truncation

$\qquad$ Make all the length sentences should be at the same size.

3. Preparing the Labels

$\qquad$ Convert the "string" label format to numeric format.

### Train the Model

Train the TensorFlow model for 20 epochs and the conditional callback with the accuracy and validation accuracy details for each epoch as follow:

<div align="center">

![Acc details](https://github.com/definaa2412/Tweet-Emotion-Detection/blob/main/images/Accuracy%20Detail.png)

</div>

Based on the output above, our model reaches 97% of accuracy and 89% of validation accuracy. It's not too bad for the simple model.

### Evaluate the Model

Evaluate the model in test data set with an accuracy 89%. It can be said that the model is good enough in classifying.

<div align="center">

![Acc eval](https://github.com/definaa2412/Tweet-Emotion-Detection/blob/main/images/Accuracy%20Evaluate.png)

</div>

### Confusion Matrix

<div align="center">

![cm](https://github.com/definaa2412/Tweet-Emotion-Detection/blob/main/images/cm.png)

</div>
 
  From confusion matrix above, mostly our model predict the correct result but it seems that the missclassification still occur between love and joy classes. It's probably caused by our data classes which are not too balance.
  
### Classification Report

<div align="center">

![cr](https://github.com/definaa2412/Tweet-Emotion-Detection/blob/main/images/cr.png)

</div>

  From the output above, mostly the metric value is pretty good. Although, the precision and recall for class 1 ("surprise") is a bit off good because it has less data when compared to other classes.






