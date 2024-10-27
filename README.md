# Lung-sound-multiclass-classification

# KINDLY REFER TO THE NOTEBOOK AND OBSERVE THE DATASET USING THE LINK TO GET IN-DEPTH IN-SIGHTS REGARDING THE ABOVE EXPLAINATION AND SOLUTION OF THE PROBLEM STATEMENT.

A multiclass classification using Computer Vision concepts implemented on OpenCV to classify things on basis of lung sounds.


This project uses machine learning library ***OpenCV*** and is a implementation of ***Computer-Vision*** concepts to classify the diseasesd and normal persons in the terms of presence of pulmonary diseases. The model takes the lung sound of the patients as input recorded, and uses extracted spectrogram to extract feature vectors using feature-label paradigm.

Link :- https://www.kaggle.com/code/rudhirmahalik/cv-project-final/input

# Q. Classify the Diseased[COPD, PNEUMONIA] and normal lung sounds from the lung sounds in the dataset

***we have used following steps to implement the project:***
  1. Data loading and cleaning
  2. Generating the spectrogram using the data for visualization
  3. Adding labels to the dataset by appending another column
  4. Merging all classes of data to a single dataframe and randomizing the order of distribution
  5. Training the model and testing

     5.1. USING MACHINE LEARNING MODELS
       -After preparing the dataframe the dataframe is flattened to be used by ML models in the feature-label paradigm where combination of coloumn apart from the feature coloumn is taken into consideration, to make the model learn intermitten combinations for certain type of label.     
       - the dataframe is splitted into train and test data and then the train data is fed to the model and trained using it.
       - the accuracy of the model is calculated using cross validation and prediction to actual ratio %.

       
     5.2 USING DEEP LEARNING MODELS
       - In case of Deep Learning models the dataframe need not to be flattend. As flattening the dataframe can loose the correlation data can be extracted by neighbour elements by the CNN models.
       - the dataframe is splitted into test and train and validation split
       - the CNN architecture is initialized where the number of filters and layers are statically initiallized
       - the train and validation data is provided to the model to train the model
       - then the performance of the model is calculated by checking the test accuracy of the cross validation  method.
    
       - in furthur steps the model is initialized by keras tuner to get let the model decided the best parameters for himself.
       - we have to specify the range of every paramemter to the tuner before instantiating it to run.
       - then the dataframe is passed into him to learn and test the performance of the model which would give us the best model.
    
  7. Result visualization
     - the results of the model was visualized using certain tools and libraries like matplotlib where the confusion matrix and graphs are ploted for the cross validation results and accuracy to visualize the performance of the model throughout the convergence process of the accuracy; and this helps to visualize the error levels of the models also.
  
   



