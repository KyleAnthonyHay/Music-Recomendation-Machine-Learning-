# Music-Recomendation-Machine-Learning-

This is a small project where I learn how to implement the decision tree model from "skllearn" to predict the music genre of users.

Libraries: pandas, sklearn, joblib

## Folders

### Intro

An introduction to using the **pandas** and **sklearn** libraries in order to train a model from a data set. "train_test_split" is used to seperate the data set into two caegories: **input** and **output**. The model is then trained to predict what the output is based on the combinations of input.

"model.fit" is the command used to train the model on the selected input(X_train, y_train). 

"accuracy_score" stores the accuracy(0.0-1.0) in variable "score"

### Music_Recomender

This program stores the trained model as a .joblib file. The line below traines the model and aves the fie. This line is commented out in the program.
`joblib.dump(model, 'music-recommender.joblib')`

This below line loads the saved model.joblib file.
`model = joblib.load('music-recommender.joblib')`

The model is then tested.

### Music_Projection

This program loads a pre-trained Decision Tree Classifier model called 'music-recommender.joblib'. It then uses the model to make predictions on the input data [[21, 1]] using the predict method.  
