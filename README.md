# COSC 426 Final Project:
This repository contains our:
- **sample data**
- **config files** for models to execute steps
- **bash scripts** for submitting jobs to turing

This README contains instructions for running our experiment on sample data. For the purpose of our proposal, these steps are all run on the same data set. In our final project, we will have separate datasets for our training, validation, and evaluation. We also provide config files and bash scripts to run our experiment with a single model, however we will be performing this using more than one in our final product.

## Step 1: Train models using the train and validation data set

Submit training job to Turing. Run the train config file using this command:
```
qsub bashscript_finalproject_train.pbs
```
This command will run this pbs file that executes our main.py function with the "train" config file. This will give us the fine-tuned model in the path specified in the config file.

## Step 2: Use TextClassification models on the evaluation data set

Run the train config file using this command:
```
qsub bashscript_finalproject_evaluate.pbs
```
This command will run this pbs file that executes our main.py function with the "evaluate" config file. This will generate a predictions file that we will use in **Step 3**

## Step 3: Analyze output from model evaluation
Run the train config file using this command:
```
qsub bashscript_finalproject_evaluate.pbs
```

After this step, we should have our results data that is ready for our own analysis


