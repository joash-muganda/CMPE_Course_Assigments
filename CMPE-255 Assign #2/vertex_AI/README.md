# Customer Propensity to Purchase Model

## Overview
This model was trained on customer purchase data to predict their propensity to purchase. We leveraged Google's Vertex AI to explore the capabilities of AutoML, streamlining the model development process. The model is designed to provide insights into customer behaviors and help in tailoring marketing strategies to enhance sales and customer engagement.

## Model Details
- **Model Name:** customer_propensity_to_buy
- **Version:** 1
- **Creation Date:** Sep 10, 2023, 4:45:53 PM
- **Training Completion:** Sep 10, 2023, 6:58:37 PM
- **Status:** Finished
- **Model ID:** 2621699714524905472
- **Budget:** 1 node hour
- **Training Duration:** 2 hr 8 min
- **Region:** us-central1
- **Encryption:** Google-managed
- **Dataset Name:** customer_propensity_to_buy
- **Dataset ID:** 6423224883676708864
- **Target Column:** ordered
- **Data Split Method:** Randomly assigned (80/10/10 split)

## Evaluation Metrics
- **PR AUC:** 1
- **ROC AUC:** 1
- **Log Loss:** 0.02
- **F1 Score:** 0.992989
- **Micro-F1:** 0.992989
- **Macro-F1:** 0.9582419
- **Precision:** 99.3%
- **Recall:** 99.3%

## Interpretation
The model's performance, based on the given metrics, is exceptional. Both the ROC AUC and PR AUC being 1 (or very close to 1) suggests that the model can distinguish between the classes very well. The F1 score, precision, and recall are also extremely high, indicating that the model is making accurate predictions with very few false positives and false negatives. However, it's crucial to ensure there isn't any data leakage or overfitting when models have almost perfect scores. Always validate the model in a real-world scenario to confirm its effectiveness.

## Hyperparameters & Algorithm
- **Algorithm:** AutoML
- **Objective:** Tabular classification
- **Source:** AutoML training
- **Optimization Goal:** Log loss
- **Feature Attribution Method:** Sampled shapley
- **Path Count:** 10

## Model Deployment and Testing
- **Export Option:** The model can be exported as a TF Saved Model for deployment on Docker containers
- **Endpoints:** These make machine learning models available for online prediction and are designed for real-time predictions catering to multiple users
- **Batch Predictions:** This feature allows for multiple prediction requests at once and stores the results in a designated location. It's ideal for scenarios where immediate responses aren't necessary
- **Note:** Currently, there are no active endpoints containing this model. To test the model, it first needs to be deployed

## Visuals and Experience
Screenshots of the visuals and user experience with the Vertex AI platform can be found in the `vertex_screenshots` folder.
