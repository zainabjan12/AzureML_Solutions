# Project Overview

This repository contains the code and resources for a real-time diabetes prediction solution using Azure Machine Learning (AML).

## Prerequisites:
- An [Azure account](https://azure.microsoft.com/en-us/free/machine-learning/) with an active subscription. [Create an account for free.](https://azure.microsoft.com/en-us/free/machine-learning/)

## Setting up Azure Machine Learning Workspace:

1. **Create Workspace:**
   - Sign in to Azure Machine Learning studio.
   - Click on "Create workspace."
   - Provide a unique workspace name, select subscription, choose or create a resource group, and pick a region.
   - Click "Create" to set up the workspace.

2. **Create Compute Instance:**
   - Navigate to Notebooks and choose "Create compute" in the middle of the page.
   - Provide a name, keep defaults on the first page, and click "Create."

These steps establish a workspace and a compute instance for running Jupyter notebooks and Python scripts in subsequent tutorials.


## Repository Structure

- **training_folder:**
  - `lr_training_script.py`: Script to train a logistic regression model and create a pickle file.
  - `score_diabetes.py`: Script used in real-time inference pipeline.
  - `batch_score_diabetes.py`: Script used in batch processing.

- **notebooks:**
  - `Real_Time_Inferencing_Service.ipynb`: Notebook orchestrating the end-to-end process, from connecting to AML workspace to deploying and conducting real-time predictions. It calls scripts from the training_folder.

- **environment.yml:**
  - Contains dependencies for the environment.

- **diabetes-data:**
  - Contains the dataset used for training and inference.

## Steps Completed:

1. **Azure ML Workspace Setup:**
   - Created an Azure ML workspace, set up a compute cluster, and connected to it.

2. **Data Preparation and Model Training:**
   - Utilized scripts in `training_folder` to train a logistic regression model and create a pickle file.

3. **Real-Time Inference:**
   - Developed a real-time inference pipeline using `Real_Time_Inferencing_Service.ipynb` that orchestrates the entire process, from model deployment to conducting real-time predictions.

4. **Batch Processing:**
   - Configured a script (`batch_score_diabetes.py`) for batch processing.

5. **Environment Configuration:**
   - Defined dependencies in `environment.yml`.

6. **Outputs:**
   - Model outputs, such as the pickle file, are stored in the `outputs` folder.

