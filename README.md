# Getting and Cleaning Data Course Project
## README

This repository contains R code for downloading and tidying the Human Activity Recognition Using Smartphones Data Set.

## Contents

* run_analysis.R: This is the script the produces a tidy dataset with mean and std from the raw data
* codebook.Rmd: Contains descriptions of the steps performed in run_analysis.R, as well as the list of produced fields of the tidy data set.


1. The included R script, run_analysis.R, conducts the following:
2. Download the dataset from web if it does not already exist in the working directory.
3. Read both the train and test datasets and merge them into x(measurements), y(activity) and subject, respectively.
4. Load the data(x's) feature, activity info and extract columns named 'mean'(-mean) and 'standard'(-std). Also, modify column names to descriptive. 
5. Extract data by selected columns(from step 3), and merge x, y(activity) and subject data. Also, replace y(activity) column to it's name by refering activity label (loaded step 3).
6. Generate 'TidyDataset' that consists of the average (mean) of each variable for each subject and each activity. The result is shown in the file tidy_dataset.txt.