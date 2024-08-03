# medical-minds-llm

## About
This repo contains code for my team's submission for the final project of the course Advanced Natural Language Processing (CS 685) under the guidance of Professor Mohit Iyyer at UMass Amherst in the Spring '24 semester. 

In the project, we combined experts LLM's using techniques such as Ensembling and Mixture of Experts and finetuned the combined as well as the base models to gain an increase in performance. We used Mistral 7B models as our base LLM models and finetuned them using QLora. 

## Proposal and Final Report
[Final Report](https://github.com/ojasraundale/medical-minds-llm/blob/main/Final%20Report.pdf) and [Project Proposal](https://github.com/ojasraundale/medical-minds-llm/blob/main/Project%20Proposal.pdf) can be found the repo. 


## File Structure
Below is the description of the folders and files in our code zip.

Data & Preprocessing:
    This folder contains all the files used in data preprocessing and dividing the data into train eval and test sets.

Base Experts
    This folder contains the .py files which creates the baseline experts. The experts were developed using Unsloth (we refered to https://github.com/unslothai/unsloth).

Baseline Models
    This folder contains notebooks used to obtain baseline accuracies of our base models and experts.

MoE
    This folder contains notebooks used to train the MoE model.

Ensembling Models
    This folder contains notebooks used to train the Ensembling Models

Evaluation
    This folder contains notebooks used to obtain the analysis graphs and evaluation metrics

fast_lora.py
    This file is from the unsloth library. This was the one that caused issue with data type mismatch during back-propogation. We rectified the error and it needs to be used to change the code in lib/unsloth/fast_lora.py folder.


## Recreating all the experiments:

To recreate our outputs, the files need to be run in the below order:
    1. Data & Preprocessing
    2. Base Experts - helps in creating the experts which will be used in MoE and Ensembling files.
    3. MoE
    4. Ensembling techniques
    5. Evaluation.
    6. Baseline Models - The codes in this folder can be run after creating the datasets and base experts.


Thank You!!!!
