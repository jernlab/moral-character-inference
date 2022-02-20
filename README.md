# Moral Character Inference Project

In this project, we seek to evaluate the correctness of a proposed hierarchical model of moral concepts supposedly used when making inferences. We use a Bayesian model and compare the results of an experiment, conducted as an online survey, to the model's prediction to evaluate the model's accuracy. 

## File Structure

The 3 folders for this project are as follows:
- old: This folder contains prior work for this project, conducted by another student in the 2020-21 school year. 
- code: This folder contains all the code files (written in Python in Jupyter Notebooks) for the project. All files are commented.
- data: This folder contains all the experiment data files, including datasets of questions used in the experiment; raw survey data from Formr; and processed survey data from all participants. 

Finally, the raw Formr spreadsheets used for the experiment (as CSV files) are included in the main folder of the project. 

## Description of Data Files

The data files in this project are listed below, and their purpose explained:
- experiment_data_F: This file contains all the specific examples of moral violations by category for a female subject.
- experiment_data_M: This file contains all the specific examples of moral violations by category for a male subject.
- formr_one_example: This file is the raw Formr input for the 1-example premise case. 
- formr_three_example: This file is the raw Formr input for the 3-example premise case. 
- SingleInferenceTask_data: This is the raw output from the Formr experiment for the 1-example premise case. 
- InferenceTask_data: This is the raw output from the Formr experiment for the 3-example premise case. 
- InferenceTask_data_incomplete, SingleInferenceTask_data_incomplete: This is the data from the incomplete Formr surveys (i.e. surveys that the participants did not complete).
- InferenceTask_data_processed, SingleInferenceTask_data_processed: This is the processed filtered survey data from Formr. 
- final_data: This file contains the combined information from the processed data for both 1-example and 3-example premise cases. 

## Description of Code Files

The code files in this project are listed, roughly in the order that they must be run. 
- model_implementation: This script contains an implementation of the Bayesian model that takes in a list of premise categories and outputs the model's predictions for each of the 7 conclusions given the premise(s). 
- formr_generator: This script takes in the data on specific experiment questions/situations, and produces the fully randomized Formr CSV files for the 1 and 3 premise cases with a specified number of unique surveys. 
- premise_category_extraction: This script includes some additional data processing stages which takes the condition information from the prompts in the Formr spreadsheet and appends it to CSV data files for the one and three premise cases. 
- processing_1_example_data, processing_3_example_data: Data processing scripts for the 1-example and 3-example premise cases, respectively. 
- plotting_data: This scripts takes the processed data from both 1 and 3 example cases, and completes the final data visualization and analysis work.  
