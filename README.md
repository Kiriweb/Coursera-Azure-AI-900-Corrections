# Coursera-Azure-AI-900-Corrections
This repository contains revised and corrected code files that I encountered during my coursework on Coursera. 
More specifically, the bicycle code in "Microsoft Azure Machine Learning" Course, "Module 1", "Exercise Part 5: Deploying a Model as a Service"

# Azure Bike Rental Prediction

This repository contains a Python script that interacts with an Azure Machine Learning model to predict bike rentals based on a five-day weather forecast. This code runs on Azure Cloud.

## Key Fixes

The original code had several issues that prevented it from working correctly:

1. Data Structure: The input data was provided as a 2D list, which was incompatible with the model's expected format. I corrected this by restructuring the data as a list of dictionaries, with each dictionary representing a day's weather features.
   
2. JSON Format: The original JSON payload didn't match the model's expected input format. I wrapped the input data inside an `Inputs` key, which resolved the issue.

3. Response Handling: The original code checked for a `result` key in the response, but the correct key is `Results`. This change ensures the predictions are retrieved correctly.

