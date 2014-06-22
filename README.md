# R script to convert the *Human Activity Recognition* data to a tidy data set for the course project.

This Readme document is written to explain the R script run_analysis.R, an R script for the course project. Comments have also been included in the script itself.

## The run.analysis script

### Objective
The objective of the script is to read in given data from the *Human Activity Recognition using Smartphones Dataset Version 1.0*, and to output a tidy dataset that gives the average of each of the mean/std variables for activity for each subject (Refer to the Codebook for definitions).

### The steps taken to create the tidy data set

1.Read in all the given data files. For this the "read.table"" function was used.

2.Next the train and test data sets were merged using "rbind". The column names were also given the appropriately descriptive names for example the column for the different activities like walking, sitting etc was names "activity".
The initial column names for all the variables were replaced with the names provided in the "features.txt" data file.

3.Then the columns with the mean and standard deviation measurements were extracted using the "grep" function. These were then merged to create one data set.

4.The "activity" column was only numerically represented e.g 1 for WALKING, 5 for STANDING, etc. These numbers were replaced descriptively by the six measured activities.

5.The final step was to :

*first create a skinny dataframe with "activity" and "subject" as the IDs, and the mean/std variables as the variables. For this the "melt" function from the "reshape2" package was used. The dataframe was 813,621 rows long.

*From the skinny dataframe, use dcast to create the tidy dataframe. with the average of each variable for each activity and each subject.

### The result
A tidy data set with the average of each variable for each activity and each subject.

















