# COSC 426 Final Project:
This repository contains our:
- **sample data**
- **config files** for models to execute steps
- **bash scripts** for submitting jobs to turing

This README contains instructions for running our experiment on sample data. For the purpose of our proposal, these steps are all run on the same data set. In our final project, we will have separate datasets for our training, validation, and evaluation. We also provide config files and bash scripts to run our experiment with a single model, however we will be performing this using more than one in our final product.

## Step 1: Train models using the train and validation data set
In main.py, change the config file name at the end of the path to
```
config_finalproject_sample_train.yaml
```
Submit training job to Turing. Run the train config file using this command:
```
qsub ___ bashscript_finalproject_train.pbs
```

This will give us the fine-tuned model in the path specified in the config file

## Step 2: Use TextClassification models on the evaluation data set

Follow the same steps used in **Step 1**, except replace "train" in file path names in both commands with "evaluate"

## Step 3: Analyze output from model evaluation
Follow the same steps used in **Step 1**, except replace "analyze" in file path names in both commands with "analyze"
