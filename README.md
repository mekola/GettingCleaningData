# GettingCleaningData
Course assignment for getting and cleaning data 

###Project Description
The purpose of this project is to demonstrate your ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis. You will be graded by your peers on a series of yes/no questions related to the project.

You are required to submit:

1.a tidy data set as described below

2.a link to a Github repository with your script for performing the analysis, and

3.a code book that describes the variables, the data, and any transformations or work that you performed to clean up the data called CodeBook.md. You should also include a README.md in the repo with your scripts. This file explains how all of the scripts work and how they are connected. 

One of the most exciting areas in all of data science right now is wearable computing. Companies like Fitbit, Nike, and Jawbone Up are racing to develop the most advanced algorithms to attract new users. The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. 
A full description is available at the site where the data was obtained: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

Here are the data for the project: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

You should create one R script called run_analysis.R that does the following.
•Merges the training and the test sets to create one data set.

•Extracts only the measurements on the mean and standard deviation for each measurement.

•Uses descriptive activity names to name the activities in the data set

•Appropriately labels the data set with descriptive activity names. 

•Creates a second, independent tidy data set with the average of each variable for each activity and each subject. 

###Reading the raw data
The raw data is in different .txt files.

1.x_test.txt: Contains 561 un-labeled features. 

2.y_test.txt: Contains the activity labels

3.subject_test.txt: Contains the test subjects

This is true for the files in the training set as well.
The R script analyzes these files.

###Project Completion
Contained in this repository are the following files which completes the project:

1.Read.md file - an overview of the project and instructions on how to create a tidy dataset

2.CodeBook.md  - a code book describes the variables, the data, and any transformations or work that I performed to clean up the data 

3.R script called run_analysis.R 

4.A file called tidy.txt which contains the output of the script above

###Instructions on creating the tidy dataset
Please follow the instructions listed below to create your own tidy dataset from the raw data. 
Assuming you are using a Windows computer:

1.Download zipped raw data files from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

2.Unzip the data files into a directory: C:\Users\[Your Name Here]\Documents\COURSERA\GETTING & CLEANING DATA\ASSIGNMENT\UCI HAR Dataset

3.Get the run_analysis.R file and save to same directory as above

4.Open a R console ( I have already set the working directory to the one specified above) and source run_analisys.R script

5.The result will be saved in tidy.txt file in the same directory as above
