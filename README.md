# Neural-Network-Analysis

## Analysis Overview

The purpose of this project is to use deep-learning neural networks with the TensorFlow platform in Python, to analyze and classify the success of charitable donations.
We use the following methods for the analysis:

- preprocessing the data for the neural network model,
- compile, train and evaluate the model,
- optimize the model.

## Results

### What variable(s) are considered as our target(s) for the model?

The variable that was our target was "IS_SUCCESSFUL". This was decided based on the fact that we are specifically looking into whether applicants will be successful if they receive funding. Variables and Features

### What variable(s) are considered to be our features for the model?

Our features were the rest of the variables in the dataset, as we believe they contribute to the success of the applicant.

### What variable(s) are neither targets nor features, and should be removed from the input data?

The variables that were removed were "EIN" and "NAME". We did not consider these variables necessary for the dataset, as the name or EIN of the would not be a factor for being successful.

### How many neurons, layers, and activation functions did we select for the neural network model?

For our base neural network model, we had 110 neurons, 2 hidden layers, and our activation function was relu.

### Were we able to achieve the target model performance?

We were unable to achieve the 75% accuracy target.

### What steps did we take to try and increase model performance?

We attempted by increasing the number of neurons to 140, adding a third hidden layer, and changing the activation function from "relu" to "tanh".

The results of our first optimization model: increasing the number of neurons to 140. 
![increased](https://github.com/bikachuuuuuu/Neural-Network-Analysis/blob/main/Resources/increased_neurons_summary.png)

The results of our second optimization model: including a third hidden layer. 

![third](https://github.com/bikachuuuuuu/Neural-Network-Analysis/blob/main/Resources/third_hidden_layer_summary.png)

The results of our third optimization model: replacing relu with tanh for the activation function.

![tanh](https://github.com/bikachuuuuuu/Neural-Network-Analysis/blob/main/Resources/tanh_model_summary.png)

## Summary

The deep learning neural network model did not reach the target of 75% accuracy. Considering that this target level is pretty average we could say that the model is not outperforming.

Since we are in a binary classification situation, we could use a supervised machine learning model such as the Random Forest Classifier to combine a multitude of decision trees to generate a classified output and evaluate its performance against our deep learning model.
