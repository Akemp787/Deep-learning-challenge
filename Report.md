# Report on the Performance of the Deep Learning Model for Alphabet Soup

## Overview of the Analysis:
The purpose of this analysis is to develop a deep learning model that predicts the success of charity donations for Alphabet Soup, a philanthropic organization. By utilizing a dataset containing various features related to charity applications, we aim to create a model that accurately classifies whether a donation will be successful or not. This classification can help Alphabet Soup optimize their resources and focus their efforts on the most promising donation opportunities.

## Results:

### Data Preprocessing:
- **Target Variable:** The target variable for our model is 'IS_SUCCESSFUL', which indicates whether a donation was successful or not.
- **Feature Variables:** The feature variables for our model include all columns except 'IS_SUCCESSFUL' as well as non-beneficial ID columns such as 'EIN', 'NAME', 'STATUS', 'SPECIAL_CONSIDERATIONS', and 'ASK_AMT'.
- **Removed Variables:** The non-beneficial ID columns ('EIN', 'NAME', 'STATUS', 'SPECIAL_CONSIDERATIONS') and the 'ASK_AMT' column were removed from the input data as they do not provide meaningful information for predicting donation success.

### Compiling, Training, and Evaluating the Model:
- **Neurons, Layers, and Activation Functions:** We experimented with different configurations in each attempt. In the first attempt, we used two hidden layers with 8 and 5 neurons respectively, both with ReLU activation functions. In subsequent attempts, we adjusted the number of neurons and activation functions to explore their impact on model performance. We chose these configurations to create a relatively simple yet effective model architecture.
- **Achievement of Target Performance:** The target model performance was not fully achieved, as the accuracy remained around 73% across all attempts.
- **Steps to Increase Model Performance:** We attempted various strategies to improve model performance, including adjusting the number of neurons and layers, trying different activation functions, and scaling the input data using StandardScaler. Despite these efforts, the model accuracy remained relatively constant.


![Attempt_1](https://github.com/Akemp787/Deep-learning-challenge/assets/146573396/d43d5cc6-107a-4188-aff5-4cfb1e773853)
![Attempt_2](https://github.com/Akemp787/Deep-learning-challenge/assets/146573396/ae08f4a6-56a1-4a8b-9142-166335916206)
![Attempt_3](https://github.com/Akemp787/Deep-learning-challenge/assets/146573396/a56cb0c4-5366-44a3-a0b5-6fbbe5aa1855)




## Summary:
In summary, our deep learning model achieved moderate performance in predicting the success of charity donations for Alphabet Soup, with an accuracy of approximately 73%. While this accuracy is decent, there is still room for improvement. To further enhance the model's performance, we recommend exploring more complex architectures, experimenting with different hyperparameters, and incorporating advanced techniques such as regularization and ensemble learning.

Additionally, considering the nature of the problem as a binary classification task, other models such as Random Forest, Gradient Boosting, or Support Vector Machines (SVM) could be considered as alternatives. These models might provide better performance, especially when dealing with complex, high-dimensional datasets like the one we have. Furthermore, ensembling techniques, such as combining predictions from multiple models, could potentially yield even higher accuracy and robustness in prediction. Therefore, further exploration of alternative models and ensemble techniques could lead to better outcomes for predicting donation success for Alphabet Soup.
