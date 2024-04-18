# Azure-Machine-Learning-Deployment-for-Diabetes-Prediction
This project demonstrates the deployment of a machine learning model for diabetes prediction using Azure Machine Learning services.


## Features:

Leverages the Azure Machine Learning SDK for workspace creation, model registration, and web service deployment.
Utilizes a Conda environment to manage dependencies (e.g., scikit-learn) for the deployed model.
Defines an inference configuration specifying the entry script for processing predictions.
Configures deployment on Azure Container Instances (ACI) with allocated CPU cores and memory.
Provides sample code for sending predictions requests to the deployed web service.

## Overall Workflow:

### Configuration and Setup:

Installs the Azure Machine Learning SDK.
Reads configuration details (subscription ID, resource group, etc.) from a JSON file.
Creates an Azure Machine Learning workspace.

### Model Registration:

Registers a pre-trained diabetes prediction model (assumed to be saved as Diabetes_Pipeline.pkl) in the workspace.

### Deployment Configuration:

Defines a Conda environment with scikit-learn dependencies.
Creates an inference configuration specifying the entry script (score.py) for handling predictions.
Sets up deployment configuration for Azure Container Instances.

### Web Service Deployment:

Deploys the registered model as a web service using Azure Machine Learning.
Retrieves the scoring URI of the deployed service, which is used for sending prediction requests.

### Sample Prediction (Optional):

Includes sample code (commented out) that demonstrates sending a prediction request to the deployed service with sample input data.

## Target Audience:

Data scientists and developers interested in deploying machine learning models on Azure Machine Learning.
Individuals seeking to understand the process of deploying a diabetes prediction model as a web service.

## Please Note:

This project requires an existing Azure Machine Learning subscription and a pre-trained diabetes prediction model.
The provided sample code demonstrates the deployment process but might require adjustments based on your specific model and scoring script.
