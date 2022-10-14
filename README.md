# Mini Project - Tweet Emotion Recognition
Defina Ambarwati : [Github](https://github.com/definaa2412)
***

## About
  In this project, we are going to create a recurrent neural network and train it on a tweet emotion dataset to to recognize emotions in tweets. This is a multi class classification problem. We will be using TensorFlow as our machine learning framework.
  
## Dataset
  The dataset is used from [Hugging Face](https://huggingface.co/datasets/emotion) containing English Twitter messages with six basic emotions: anger, fear, joy, love, sadness, and surprise.
  
## Summary
### Data Preprocessing
1. Word Tokenization

$\qquad$ Splitting a phrase, sentence, paragraph, or an entire text document into smaller units called token.

2. Padding and Truncation

$\qquad$ Make all the length sentences should be at the same size.

3. Preparing the Labels

$\qquad$ Convert the "string" label format to numeric format.

### Training the Model

Train the TensorFlow model for 20 epochs and the conditional callback with the detail accuracy each epoch as follow:




