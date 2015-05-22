##Getting and Clean Data Course Project
#Feature Selection 
=================
The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain signals (prefix 't' to denote time) were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz. 

Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag). 

Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to indicate frequency domain signals). 
These signals were used to estimate variables of the feature vector for each pattern:  
'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.

* tBodyAcc-XYZ
* tGravityAcc-XYZ
* tBodyAccJerk-XYZ
* tBodyGyro-XYZ
* tBodyGyroJerk-XYZ
* tBodyAccMag
* tGravityAccMag
* tBodyAccJerkMag
* tBodyGyroMag
* tBodyGyroJerkMag
* fBodyAcc-XYZ
* fBodyAccJerk-XYZ
* fBodyGyro-XYZ
* fBodyAccMag
* fBodyAccJerkMag
* fBodyGyroMag
* fBodyGyroJerkMag

The set of variables that were estimated from these signals are: 
* mean()	Mean value
* std()	Standard deviation
* mad()	Median absolute deviation 
* max()	Largest value in array
* min()	Smallest value in array
* sma()	Signal magnitude area
* energy()	Energy measure. Sum of the squares divided by the number of values. 
* iqr()	 Interquartile range 
* entropy()	Signal entropy
* arCoeff()	Autorregresion coefficients with Burg order equal to 4
* correlation()	correlation coefficient between two signals
* maxInds()	index of the frequency component with largest magnitude
* meanFreq()	Weighted average of the frequency components to obtain a mean frequency
* skewness()	skewness of the frequency domain signal 
* kurtosis()	kurtosis of the frequency domain signal 
* bandsEnergy()	Energy of a frequency interval within the 64 bins of the FFT of each window.
* angle()	Angle between to vectors.

The fitness measurements were combined and subsetted select mean() and std() measurements only.  Finally for each activity and subject, we took the mean of the mean() and std() values and output the results into the data set containing 30 subjects for each activity or 180 observations and 68 columns (activity, subject, 33 mean of means, 33 mean of stds).

- activityDesc (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING)
- subject	Subject number (1-30)
- mean.tBodyAcc.mean.X	
- mean.tBodyAcc.mean.Y	
- mean.tBodyAcc.mean.Z	
- mean.tGravityAcc.mean.X	
- mean.tGravityAcc.mean.Y	
- mean.tGravityAcc.mean.Z	
- mean.tBodyAccJerk.mean.X	
- mean.tBodyAccJerk.mean.Y	
- mean.tBodyAccJerk.mean.Z	
- mean.tBodyGyro.mean.X	
- mean.tBodyGyro.mean.Y	
- mean.tBodyGyro.mean.Z	
- mean.tBodyGyroJerk.mean.X	
- mean.tBodyGyroJerk.mean.Y	
- mean.tBodyGyroJerk.mean.Z	
- mean.tBodyAccMag.mean	
- mean.tGravityAccMag.mean	
- mean.tBodyAccJerkMag.mean	
- mean.tBodyGyroMag.mean	
- mean.tBodyGyroJerkMag.mean	
- mean.fBodyAcc.mean.X	
- mean.fBodyAcc.mean.Y	
- mean.fBodyAcc.mean.Z	
- mean.fBodyAccJerk.mean.X	
- mean.fBodyAccJerk.mean.Y	
- mean.fBodyAccJerk.mean.Z	
- mean.fBodyGyro.mean.X	
- mean.fBodyGyro.mean.Y	
- mean.fBodyGyro.mean.Z	
- mean.fBodyAccMag.mean	
- mean.fBodyBodyAccJerkMag.mean	
- mean.fBodyBodyGyroMag.mean	
- mean.fBodyBodyGyroJerkMag.mean	
- mean.tBodyAcc.std.X	
- mean.tBodyAcc.std.Y	
- mean.tBodyAcc.std.Z	
- mean.tGravityAcc.std.X	
- mean.tGravityAcc.std.Y	
- mean.tGravityAcc.std.Z	
- mean.tBodyAccJerk.std.X	
- mean.tBodyAccJerk.std.Y	
- mean.tBodyAccJerk.std.Z	
- mean.tBodyGyro.std.X	
- mean.tBodyGyro.std.Y	
- mean.tBodyGyro.std.Z	
- mean.tBodyGyroJerk.std.X	
- mean.tBodyGyroJerk.std.Y	
- mean.tBodyGyroJerk.std.Z	
- mean.tBodyAccMag.std	
- mean.tGravityAccMag.std	
- mean.tBodyAccJerkMag.std	
- mean.tBodyGyroMag.std	
- mean.tBodyGyroJerkMag.std	
- mean.fBodyAcc.std.X	
- mean.fBodyAcc.std.Y	
- mean.fBodyAcc.std.Z	
- mean.fBodyAccJerk.std.X	
- mean.fBodyAccJerk.std.Y	
- mean.fBodyAccJerk.std.Z	
- mean.fBodyGyro.std.X	
- mean.fBodyGyro.std.Y	
- mean.fBodyGyro.std.Z	
- mean.fBodyAccMag.std	
- mean.fBodyBodyAccJerkMag.std	
- mean.fBodyBodyGyroMag.std	
- mean.fBodyBodyGyroJerkMag.std	
