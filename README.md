# Coursera-Azure-AI-900-Corrections
# Azure Bike Rental Prediction and Diabetes Dataset Correction

This repository contains a Python script that interacts with an Azure Machine Learning model to predict bike rentals based on a five-day weather forecast. More specifically, the bicycle code in "Microsoft Azure Machine Learning" Course, "Module 1", "Exercise Part 5: Deploying a Model as a Service".

Additionally, it includes a corrected CSV file for a diabetes dataset used in "Module 3", "Exercise Part 3: Exploration Data".

# 1. Azure Bike Rental Prediction

This repository contains a Python script that interacts with an Azure Machine Learning model to predict bike rentals based on a five-day weather forecast. This code runs on Azure Cloud.

## Key Fixes

The original code had several issues that prevented it from working correctly:

1. Data Structure: The input data was provided as a 2D list, which was incompatible with the model's expected format. I corrected this by restructuring the data as a list of dictionaries, with each dictionary representing a day's weather features.
   
2. JSON Format: The original JSON payload didn't match the model's expected input format. I wrapped the input data inside an `Inputs` key, which resolved the issue.

3. Response Handling: The original code checked for a `result` key in the response, but the correct key is `Results`. This change ensures the predictions are retrieved correctly.

# 2. Diabetes Dataset

The `diabetes_datasets_correct.csv` file has been uploaded to replace the now-invalid URL for the Diabetes Dataset used in Module 3, Exercise Part 3: Exploration Data. This file is essential for completing the exercise as intended.
