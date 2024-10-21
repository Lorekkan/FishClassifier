# Sequential Fish Classifier
A sequential neural network fish classifier. There are 9 kinds of fish with each having 1000 samples in this project. All images used are gorund truth images so that color of the fish has no effect on memorization. The model is trained only by shape. Images were also rotated in order to reduce overfitting. 70% of the images are used as the training data and the remaining data is split equally between test and validation. Model's implementation details are further explained in the Kaggle notebook which is provided at the bottom of this README file.

# Results
With 10 epoch and 126 batch size, the model reached 74.38% training accuracy and 66.89% validation accuracy. When prediction is done on test data, it is observed that it has 67.70% accuracy which is very close to validation accuracy and moderately lower than the training accuracy. Therefore, the model might have some overfitting issues because of the difference in training and test accuracies. Altough, the amount of overfitting shouldn't be that much considering validation and test accuracies are very close to each other. When loss and accuracy graphs are observed, it can be concluded that 6 or 7 could be good stopping point for epoch because of two factors: 1) Training and validation accuracies are similar for those instances. 2) After epoch 7, validation loss and accuracy doesn't seem to change much. But messing around with the variables more could be a better approach since the accuracy score is also a bit low. With the amount of work I have done, this was the best results obtained.

# Kaggle Link to the Notebook
[https://www.kaggle.com/code/cengizhanterziolu/sequential-fish-classifier](https://www.kaggle.com/code/cengizhanterziolu/sequential-fish-classifier)

Author: Cengizhan Terzioğlu
