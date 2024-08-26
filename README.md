# Amazon SageMaker

Build, train, and deploy machine learning (ML) models for any use case with fully managed infrastructure, tools, and workflows.

### Support for the leading ML frameworks, toolkits, and programming languages

![aws sagemaker](image.png)

Amazon SageMaker is a fully managed service that brings together a broad set of tools to enable high-performance, low-cost machine learning (ML) for any use case.

With SageMaker, you can build, train and deploy ML models at scale using tools like notebooks, debuggers, profilers, pipelines, MLOps, and more – all in one integrated development environment (IDE).

SageMaker supports governance requirements with simplified access control and transparency over your ML projects. In addition, you can build your own FMs, large models that were trained on massive datasets, with purpose-built tools to fine-tune, experiment, retrain, and deploy FMs.

SageMaker offers access to hundreds of pretrained models, including publicly available FMs, that you can deploy with just a few clicks.

### A high-level overview of ML workflows in SageMaker

Doing machine learning in SageMaker is slightly different than doing it on your local machine. We’ve already covered the first steps:

- Creating an `AWS account`.
- Creating a `notebook instance`.
- Creating an `S3 bucket` for the project.

They are companions for popular ML libraries such as `scikit-learn`, `XGBoost`, `TensorFlow`, `PyTorch`, etc. Using these estimators, SageMaker builds Docker containers around your script, deploying it as an endpoint to serve it at scale.

### Setting up the notebook instance for SageMaker

Let’s start by importing the necessary libraries inside the sagemaker-test notebook you created earlier:

```python
import boto3
import numpy as np
import pandas as pd
import sagemaker
from sagemaker import get_execution_role
from sklearn.model_selection import train_test_split
```
