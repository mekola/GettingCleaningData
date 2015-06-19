#CodeBook for the tidy dataset
The objective of this project is to create a tidy dataset from raw data, so that further analysis can be performed on the data.

###Data Source 
The raw data is obtained from the follwoing link:

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 

A description of the data collection can be viewed at: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones 

###Synopsis of the experiment to obtain the data
The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data. 
The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain. See 'features_info.txt' for more details. 

###Details of Variables 
The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. 
These prefix 't' singnals were captured at a constant rate of 50 Hz. 
The signals were filtered to remove noise. 
The acceleration signals were separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ).
Therafter, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). 
The magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag). 
Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to indicate frequency domain signals). 
For a more complete list refer to the files features_info and features.txt contained in the data download .zip file.

###Selection / Renaming of Variables.
I have selected features, for this assignment, based on "2.Extracts only the measurements on the mean and standard deviation for each measurement."
To be on the safe-side I have selected all features variables that have anything to do with mean and sd.
The follwing is a list of signals that were used to estimate variables of the feature vector for each pattern:  
'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.

tBodyAcc-XYZ

tGravityAcc-XYZ

tBodyAccJerk-XYZ

tBodyGyro-XYZ

tBodyGyroJerk-XYZ

tBodyAccMag

tGravityAccMag

tBodyAccJerkMag

tBodyGyroMag

tBodyGyroJerkMag

fBodyAcc-XYZ

fBodyAccJerk-XYZ

fBodyGyro-XYZ

fBodyAccMag

fBodyAccJerkMag

fBodyGyroMag

fBodyGyroJerkMag

The set of variables that were estimated (and kept for this assignment) from these signals are: 

•mean(): Mean value

•std(): Standard deviation

Additional vectors obtained by averaging the signals in a signal window sample. These are used on the angle() variable:

•gravityMean

•tBodyAccMean

•tBodyAccJerkMean

•tBodyGyroMean

•tBodyGyroJerkMean

Features are normalized and bounded within [-1,1].

As a result of the script run, the variable names have the word "mean" or "std" added to them and look like this: 

tbodyaccmeanx = the mean of tBodyaccx 

tbodyaccstdx = the standard deviation of ttbodyaccx

...and so on for Y and Z.

Two columns "activity" and "subject" have been added to the dataset as required. The dataset has been ordered.

###Conclusion
Running the script will result in a tidy dataset, in the directory listed in the readme.md file.
Please refer to this readme.md file for background and other details.
Every effort has been made to eliminate errors.  
If there are errors please report them for fixes.


