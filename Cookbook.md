# Code Book

This code book includes information about the source data, the transformations performed after collecting the data and some information about the variables of the resulting data sets.

The source data was collected from the [UCI Machine Learning Repository](http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones) to complete an assignment.
The assignment involved working with the [data set](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip) and producing tidy data representation of the source data. 

Below is a list of the operations done to achieve the outputs.

1. Downloaded the data set
2. Loaded test and training data sets into data frames
3. Loaded source variable names for test and training data sets
4. Loaded activity labels
5. Combined test and training data frames using rbind
6. Paired down the data frames to only include the mean and standard deviation variables
7. Replaced activity IDs with the activity labels for readability
8. Combined the data frames to produce one data frame containing the subjects, measurements and activities
9. Produced "mergeddata.txt" with the combined data frame as the first expected output
10. Created another data set using the data.table library to easily group the clean data by subject and activity. Apply the mean and standard deviation calculations across the groups
and produced "cleandata.txt" as the second expected output

Please refer to [ReadMe.md] for implementation details.
