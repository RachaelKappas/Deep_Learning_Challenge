# Deep_Learning_Challenge
Module 21 Challenge


# Overview of the Analysis
The purpose of this analysis is to develop a deep learning model to predict the success of funding applications for Alphabet Soup. The goal is to use a neural network to classify whether an applicant will be successful based on various features provided in the dataset. This analysis includes preprocessing the data, building and training a neural network model, and evaluating its performance.

# Results
## Data Preprocessing
* Target Variable:
  * IS_SUCCESSFUL: This is the binary target variable indicating whether the funding was used effectively (1 for successful, 0 for unsuccessful).
      
* Feature Variables:
  * All columns except EIN, NAME, and IS_SUCCESSFUL are used as features. This includes APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, and SPECIAL_CONSIDERATIONS.
    
* Variables to Remove:
  * EIN: Identification column, not useful for predictions.
  * NAME: Identification column, not useful for predictions.
These columns were dropped during preprocessing to focus on the features relevant to predicting the success of funding applications.

# Compiling, Training, and Evaluating the Model
* Neurons, Layers, and Activation Functions:
  * Input Layer: The number of neurons corresponds to the number of features in the dataset (8).
  * Hidden Layers:
    * First Hidden Layer: 8 neurons with ReLU activation function.
    * Second Hidden Layer: 8 neurons with ReLU activation function.
  * Output Layer: 1 neuron with a sigmoid activation function to output a probability for binary classification.
   
### Why This Configuration:
* The number of neurons and layers was chosen to provide enough capacity to learn from the data while avoiding overfitting. The ReLU activation function introduces non-linearity, which is essential for learning complex patterns. The sigmoid activation function is appropriate for binary classification tasks.
  
* Model Performance:
 * Loss: 0.5577
 * Accuracy: 72.36%
 * The target model performance was not achieved, as the accuracy fell short of the 75% target.
* Steps Taken to Increase Model Performance:
  * Adjusted the number of hidden layers and neurons.
  * Used different activation functions.
  * Experimented with the number of epochs and batch size during training.

   
# Summary
The deep learning model built for predicting the success of funding applications achieved an accuracy of 72.36%, which is below the desired 75% target. The model structure included two hidden layers with 8 neurons each and used ReLU and sigmoid activation functions.
