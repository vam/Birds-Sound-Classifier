Introduction
The Birds-Sound classifier App aims to classify five different bird species based on their distinct vocalizations. This report outlines the methodology, implementation, and results of the project.

Dataset
The dataset consists of 30-second audio samples featuring the following bird species:

White-breasted Wood-Wren
House Sparrow
Red Crossbill
Chestnut-crowned Antpitta
Azara's Spinetail


1) Preprocessing:
Loaded the dataset using pandas.
Preprocessed the data by filtering out irrelevant entries and assigning numerical labels to the bird species.

2)Feature Extraction:
Utilized YAMNet, a pretrained audio event classifier, to extract embeddings from audio samples.

3)Model Architecture:
Designed a neural network model consisting of dense layers for classification.
Used dropout and batch normalization to prevent overfitting.

4)Training:
Created TensorFlow datasets for training and testing.
Compiled and trained the model using the Adam optimizer and sparse categorical crossentropy loss function.

5)Evaluation:
Evaluated the model's performance on the test dataset in terms of loss and accuracy.

Results
Achieved a final accuracy of 37% on the test dataset.
Saved the trained model as "b_bird_model.h5" for future use.
