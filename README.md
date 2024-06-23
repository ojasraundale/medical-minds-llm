# medical-minds-llm

This repo contains code for my team's submission for the final project of the course Advanced Natural Language Processing (CS 685) under the guidance of professor Mohit Iyyer at UMass Amherst in the Spring '24 semester. 


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


Additioanlly, all our codes and notebooks are maintained in the below drive folder. This can be accessed using UMass Gmail accounts.:
    https://drive.google.com/drive/folders/1GQ5I7VfgICV32bIM4Z7QUelLypdw6Mro?usp=sharing

To recreate our outputs, the files need to be run in the below order:
    1. Data & Preprocessing
    2. Base Experts - helps in creating the experts which will be used in MoE and Ensembling files.
    3. MoE
    4. Ensembling techniques
    5. Evaluation.
    6. Baseline Models - The codes in this folder can be run after creating the datasets and base experts.


Thank You!!!!