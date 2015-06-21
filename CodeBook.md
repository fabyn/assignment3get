#Code Book

##The data set

The Data set: 
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 

A full description of the data set: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones 

## Transformations performed
Transformations performed to clean up the data:

1. Merges the training and the test sets to create one data set;
2. Extracts only the measurements on the mean and standard deviation for each measurement;
3. Uses descriptive activity names to name the activities in the data set;
4. Appropriately labels the data set with descriptive variable names;
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

##Variables

* Load activity labels:
activity_labels

* Load data column names:
features

* Extract the measurements on the mean and standard deviation for each measurement: 
extract_features, 
X_test

* Load and process X_test & y_test data:
X_test, 
y_test,
subject_test

* Bind data:
test_data, 
train_data

* Load and process X_train and y_train data: 
X_train,
y_train,
subject_train

* Merge test and train data: 
data,
id_labels,
data_labels, 
melt_data

* Apply mean function to data set using dcast function:
tidy_data

* Create file with the tidy data: 
write.table
