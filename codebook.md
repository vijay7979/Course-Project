#Codebook for *Human Activity Recognition* course project.
========================================================

##Introduction

The required output has dimensions of 180 rows and 81 columns.
The columns comprise of 79 columns which measure the average of the means or standard deviations of that particular variable.
The first tow columns are the activity and the subject who is carrying out the activity.

## Code Description

*_activity_is the specific type of activity.
        WALKING
        WALKING_UPSTAIRS
        WALKING_DOWNSTAIRS
        SITTING
        STANDING
        LAYING
        
*_subject_is the individual carrying out the activities.
        Ranges from 1 to 30
        
### The remaining 79 variables are measurements of the triaxial acceleration or triaxial angular velocity. So each measurement will have three components i.e. x, y and z. Each measurement has been normalized and is bounded between -1 and 1.

Those variables ending with ...mean... are averages of measurements of means, and those ending with ...std... are averages of measurements of standard deviations.

Examples of mean average:
*_tBodyAcc-mean()-X_is average of mean measurement in x direction                   
*_tBodyAcc-mean()-Y_is average of mean measurement in y direction                  
*_tBodyAcc-mean()-Z_is average of mean measurement in z direction 

Examples of standard deviation average:
*_tGravityAcc-std()-X_is average of standard deviation in x direction                 
*_tGravityAcc-std()-Y_is average of standard deviation in y direction                
*_tGravityAcc-std()-Z_is average of standard deviation in z direction 



