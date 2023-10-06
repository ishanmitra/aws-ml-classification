# Deploy and monitor a machine learning workflow for Image Classification #
An image-classification project for Udacity's AWS Machine Learning Nanodegree.

## Table of Contents ##
1. [Overview](#overview)
2. [File Contents](#file_contents)
3. [Step Function](#step_function)
4. [Inferences](#inferences)


## Overview<a name="overview"></a> ##
This is a project in Udacity’s AWS Machine Learning Engineer Nanodegree geared towards building an ML workflow.

The project uses a sample dataset called CIFAR to simulate an image classification model. The machine learning workflow for Image Classification is deployed using AWS resources such as, `sagemaker` and `boto3` SDKs, image-classification built-in algorithm, Lambda functions and Step Function Workflow, and SageMaker model monitor and endpoint.  

The CIFAR dataset is open source and can be downloaded at: https://www.cs.toronto.edu/~kriz/cifar-100-python.tar.gz  

The goal of this project is to:  
1. Build an image classification model that differentiates between bicycles and motorcycles.
2. Deploy the model for inference using AWS Lambda functions and AWS Step functions.

## File Contents<a name="file_contents"></a> ##
* 'starter.ipynb': Jupyter notebook with solution and visualisations

* 'lambda.py': All three Amazon Lambda functions later invoked in Step Functions

* 'StepFunction.json': Exported JSON for Step Function flowchart

* 'stepfunction/': Image directory

## Step Function<a name="step_function"></a> ##
![step_function](https://raw.githubusercontent.com/ishanmitra/aws-ml-classification/main/StepFunction.png)  

## Inferences<a name="inferences"></a> ##
The best image classification model has a test accuracy of 0.848958.  

The visual below shows whether the images are inferred as a motorbike or a bicycle with their probability scores. Text is red if it is below the confidence threshold of 0.93.  

![viz](https://raw.githubusercontent.com/ishanmitra/aws-ml-classification/main/stepfunction/viz.png)
