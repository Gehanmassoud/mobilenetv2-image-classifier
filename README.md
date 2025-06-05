# MobileNetV2 Image Classifier with Azure ML Deployment
CNN image classifier using TensorFlow and MobileNetV2 trained on custom data. Includes Azure ML deployment pipeline for scalable hosting, REST API inference, and reproducible environment setup. Modular design for easy adaptation to other image tasks.

This project demonstrates training a MobileNetV2 deep learning model using TensorFlow for image classification and deploying it as a scalable REST API using Azure Machine Learning.

## Project Structure
- `model_training.ipynb`: Training and evaluation of the model.
- `mobilenetv2_model/`: Saved model directory.
- `score.py`: Script to handle inference requests in Azure ML deployment.
- `conda_dependencies.yml`: Environment dependencies for Azure.
- `deploy.py`: Script to register and deploy the model on Azure ML.
- `test_endpoint.py`: Sample client to test the deployed endpoint.

## How to Deploy
1. Train and save your TensorFlow model.
2. Modify `deploy.py` with your Azure subscription and workspace details.
3. Run `deploy.py` to deploy the model to Azure.
4. Use `test_endpoint.py` to test your deployed model.

## Requirements
- Azure subscription with Azure Machine Learning workspace.
- Python 3.8+
- Azure ML SDK (`pip install azure-ai-ml azure-identity`)
