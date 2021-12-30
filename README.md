# Hate-Speech-Detection

## Dataset
The dataset used is accessed from the SemEval 2019: Task 5. 
For downloading the dataset please register in the [contest](https://competitions.codalab.org/competitions/19935) and request the dataset.

## Data Preprocessing
* Remove Mentions : Example - @john is substituted with USER.
* Remove URLs : URLs are replaced with the keyword “URL”.
* Removing special characters.
* Converting emoji to text.
* Lowercase text.

### GloVe Embeddings
Link - https://huggingface.co/stanfordnlp/glove/resolve/main/glove.6B.zip


## Results

|                         Model                        |     Test F1-score (Macro)    |     Test Accuracy score    |
|:----------------------------------------------------:|:----------------------------:|:--------------------------:|
|                      Naive Bayes                     |              0.42            |             0.48           |
|             Support Vector   Machine (SVM)           |              0.48            |             0.51           |
|     SVM + Universal   Encoder Sentence Embeddings    |          **0.53**            |             **0.54**           |
|                   LSTM + GloVe(300d)                 |              0.50            |             0.53           |
|                   GRU + GloVe(300d)                  |              0.51            |             0.53           |
|                          Bert                        |              0.47            |             0.52           |
