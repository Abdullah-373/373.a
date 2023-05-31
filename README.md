## Team members:
 --Abdullah Hasan
 --Haroun Alhassan 
 --Yllka ostergllava




## Introduction

In this project, our goal is to assist a social media department in analyzing the success of their communication strategies. Specifically, we aim to develop a sophisticated tool that can accurately predict the number of shares on social media platforms based on the content and the supposed publication time. To achieve this, we have been provided with a comprehensive dataset that will serve as the foundation for our machine learning analysis.

## Methods

To tackle this challenge, we employed a diverse set of models, including a Neural Network Regression model implemented in Keras, an XGboost Regression model, and a Random Forest Regressor. These models were selected for their ability to capture complex relationships within the data and make accurate predictions. For each model, we followed a systematic approach that involved several key steps:

We began by conducting an Exploratory Data Analysis (EDA) to gain a deep understanding of the dataset's characteristics, uncover potential patterns or anomalies, and identify any data preprocessing requirements. Through visualizations and statistical analysis, we gained valuable insights into the distribution of variables, correlations, and potential issues that needed to be addressed.

To ensure robust model evaluation and performance estimation, we divided the dataset into distinct training and test sets. The training set was utilized to train the models, while the test set was reserved for evaluating the final performance of each model.

Preprocessing the dataset was an essential step in preparing the data for modeling. We employed various techniques such as outlier detection and removal, as well as encoding categorical features using one-hot encoding or other suitable methods. By standardizing and transforming the data appropriately, we ensured that our models could effectively learn from the dataset.

To optimize the performance of each model, we implemented a thorough hyperparameter tuning process. We created a validation set from the training data to assess the model's behavior with default hyperparameters. Subsequently, we employed advanced techniques like 10-fold cross-validation to explore different combinations of hyperparameters and identify the best set of values for each model. This process aimed to find the optimal balance between model complexity and generalization.

Once the hyperparameters were fine-tuned, we selected the best architecture for each model based on the evaluation metrics specific to the task. These metrics included Mean Squared Error (MSE), Mean Absolute Error (MAE), and R2 score. We carefully evaluated each model's performance and selected the one that exhibited the highest predictive power.

Finally, we computed the performance of each model on the test set, providing a reliable assessment of their predictive capabilities. This allowed us to compare and contrast the models' performance and identify the most effective model for predicting the number of shares on social media.

Hyperparameter Tuning

To achieve optimal model performance, we employed Random Search for hyperparameter tuning in our models. This technique efficiently explored a wide range of hyperparameter values and allowed us to find the best combination of settings for each model.

## Experimental Design

To validate the effectiveness of our approach, we conducted a series of experiments for each model. These experiments aimed to assess the model's predictive power and generalization capabilities. We utilized evaluation metrics such as Mean Squared Error (MSE), Mean Absolute Error (MAE), and R2 score to quantitatively measure the performance of each model. By comparing the results obtained from different models, we could make informed decisions about their relative strengths and weaknesses.

## Results

Before dropping variables and using Linear Regression, the initial performance scores for each model were as follows:

Model Used	R2
Neural Network Regressor	0.03
Random Forest Regressor	-0.27
XGboost Regressor	-0.53
However, after dropping variables and implementing Linear Regression, the performance scores for each model improved significantly:

Model Used	R2
Neural Network Regressor	0.07
Random Forest Regressor	0.05
XGboost Regressor	0.08
These results indicated that the XGboost Regressor outperformed the other models, demonstrating the highest predictive performance for the number of shares on social media.

## Conclusions

In conclusion, our project's main finding was that the XGboost Regressor exhibited the best prediction performance among the three models considered. However, it is worth noting that the overall performance of all three models was not particularly strong, as evidenced by the relatively low R2 scores. This suggests that there may be other important factors influencing the number of shares on social media that were not accounted for in our analysis.

Moving forward, there are several potential avenues for future work in this domain. One possibility is to explore different feature engineering techniques to extract more meaningful information from the available data. Additionally, considering additional data sources, such as user demographics or contextual information, could potentially enhance the predictive power of our models. Moreover, experimenting with alternative machine learning algorithms beyond the ones we employed may offer further insights and potentially yield improved predictions for the number of shares on social media. By continuously refining our approach and incorporating new insights, we can unlock even more accurate predictions and contribute to the field of social media analytics.
