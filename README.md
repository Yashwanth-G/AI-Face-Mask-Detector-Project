# AI Face Mast Detector - COMP 6721 Winter 2022 Project

# Assignment 1 (Due by 23rd March 2022)

You have to develop an AI that can analyze face images and detect whether a person is wearing a face mask or not, as well as the type of mask that is being worn:

Towards this end, you have to develop a Deep Learning Convolutional Neural Network (CNN) using PyTorch and train it to recognize five different classes: 
(1) Person without a face mask 
(2) Person with a “community” (cloth) face mask 
(3) Person with a “surgical” (procedural) mask
(4) Person with a “FFP2/N95/KN95”-type mask (you do not have to distinguish between them)
(5) Person with a FFP2/N95/KN95 mask that has a valve. You do not have to consider other mask types (e.g., FFP3), face shields, full/half-face respirators, PPEs, or images that do not show a single face (e.g., groups of people). 

You will have to collect suitable training data and evaluate the performance of your system as follows:

# Training Data: 
Create datasets for training and testing your AI. You have to provide provenance information, i.e., where you obtained each image in your dataset. You can re-use existing datasets, but again please make sure you properly reference the source of the image datasets (name, author, source, license of the dataset). It is expected that you have a minimum of 1500 training images and 500 testing images (across all classes). 

Make sure that both your training and testing data sets are balanced, i.e., have roughly the same number of images per class. Note that you will have to perform suitable pre-processing (such as size-normalization) on your datasets. Also, please take note of the additional evaluation task that will follow in Part II of the project, mentioned below, when setting up your dataset. For images showing a face, you can limit your dataset to single persons (i.e., you do not have to consider groups of people). You must use real training data, i.e., using synthetic, generated data is not permitted. 

# Deep Learning: 
Create a suitable Convolutional Neural Network (CNN) architecture, implement it in PyTorch, and train it using your dataset. You must implement the complete workflow in your CNN, that is, you cannot use any external libraries, except for the ones mentioned below. 

# Evaluation: 
Evaluate your model, creating a table of results showing the accuracy, precision, recall and F1-measure, as well as a confusion matrix. You must automate the training/test-split in your project (e.g., do not use two separate, manually split datasets). You can use scikit-learn (including skorch7) for your evaluation process.

# Team Member Specialization: 

While all team members have to contribute equally to the project, you must designate one person who is mainly responsible for each of the following three sub-tasks in the project: A 

(I) Data Specialist, responsible for creating, pre-processing, loading & analyzing the datasets.

(II) Training Specialist, responsible for setting up and training the CNN.

(III) Evaluation Specialist, responsible for analyzing, evaluating, and applying the generated model. 

Each specialist has to write the corresponding part in the project report, detailed below. Note: this does not mean the designated person has to do all the work for the given task, but rather is mainly responsible for this work and can define and distribute sub-tasks to the other team members. 

# Report:
You have to write a report on your work with the following information: 

Title page: showing your group information (team name, team members, ID numbers, team member specialization). Length: 1 page

Dataset: Describe how you built your dataset and where you collected images (provide details on each image’s source in a file). Provide statistics on the size and structure of your dataset, i.e., how many images you have in each class. Length: ca. 1 page

CNN Architecture: Describe the architecture of your CNN and provide details on the training process
(how many epochs you trained, etc.). Length: ca. 1 page (excluding images/diagrams)

Evaluation: Evaluate your model and provide the tables mentioned above. Discuss the results and explain how and where you want improve during the second phase of the project (also see PhaseII details below). Length: ca. 1 page See https://github.com/skorch-dev/skorch

Reference Section: containing citations to all relevant resources that you have consulted (books, Web sites, . . . ), even if it was just to inspire you. Failure to properly cite your references constitutes plagiarism and will be reported.

# Project Phases I and II:
The goal of this first phase of the project is to set up the complete AI learning & evaluation process and gather first results. You can improve the design and collect further training data for the final submission. In other words, do not overly worry about the performance at this step, rather focus on a proper design of your datasets and evaluation process, so that you can further improve it in the second phase of the project.

# Phase II Preview: 
In Part II of the project, you are expected to further improve the performance of your system. A new task will be an extended evaluation of your AI, where you have to determine if your model exhibits any kind of bias, i.e., whether it performs differently for faces depending on age, gender, or race; and subsequently remove the bias from your system.

# Deliverables. Your submission must include the following deliverables within a single .zip or .tgz archive:

Python code: All the Python code that you developed for this project. You must have a complete CNN implemented using PyTorch.

Dataset: Information on the datasets you collected, as well as a file detailing the source of each dataset/image. For external, publicly available dataset, only include a  reference to the source with the details mentioned above. Include images you created yourself, as well as any manually created metadata for the Phase II bias evaluation.

Trained Model: The trained model that you used in your evaluation, together with some sample data  (ca. 100 images) and instructions on how to run your system on the provided data. 

README: A readme.txt (or readme.md) file that lists all submitted files with an explanation of their content. It also must describe how to run your code for (a) training and (b) testing (including generating the evaluation results provided in the report). If your instructions are incomplete and your code cannot be run you might not receive any marks for your work. 

Report: The project report, as detailed above, in PDF format.

