1. Purpose of the Code.
The code is part of the final project in Data Science Speciallization 3: Getting and Cleaning Data to merge, clean and extract from the raw data to provide a tidy data set based on specific requirement.

2. Original data.
The raw data are collected from the accelerometers from the Samsung Galaxy S smartphone. Description of the data are in below link: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

3. Outcome of the code.
a combined and tidy data set from merging the raw data and taking the mean and standard deviation of each acitivities, and a new tidy data set with the average of each variable for each activity and each subject. 

4. Description of variables.
  1. Subject: integer lists the index of tested subjects, from 1 to 30.
  2. Activities: text lists activities of the tested subject, including laying, sitting, standing, walking, walking upstairs, walking downstairs.
  3-68: features as signals generates from the smartphone. 
    The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals timeAcc-XYZ and timeGyro-XYZ. These time domain signals were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (timeBodyAcc-XYZ and timeGravityAcc-XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz. 

    Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (timeBodyAccJerk-XYZ and timeBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (timeBodyAccMag, timeGravityAccMag, timeBodyAccJerkMag, timeBodyGyroMag, timeBodyGyroJerkMag). 

    Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing frequencyBodyAcc-XYZ, frequencyBodyAccJerk-XYZ, frequencyBodyGyro-XYZ, frequencyBodyAccJerkMag, frequencyBodyGyroMag, frequencyBodyGyroJerkMag.  
        
    These signals were used to estimate variables of the feature vector for each pattern: '-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.
    timeBodyAcc-XYZ
    timeGravityAcc-XYZ
    timeBodyAccJerk-XYZ
    timeBodyGyro-XYZ
    timeBodyGyroJerk-XYZ
    timeBodyAccMag
    timeGravityAccMag
    timeBodyAccJerkMag
    timeBodyGyroMag
    timeBodyGyroJerkMag
    frequencyBodyAcc-XYZ
    frequencyBodyAccJerk-XYZ
    frequencyBodyGyro-XYZ
    frequencyBodyAccMag
    frequencyBodyAccJerkMag
    frequencyBodyGyroMag
    frequencyBodyGyroJerkMag

    The set of variables that were estimated from these signals are: 

    mean(): Mean value
    std(): Standard deviation
    mad(): Median absolute deviation 
    max(): Largest value in array
    min(): Smallest value in array
    sma(): Signal magnitude area
    energy(): Energy measure. Sum of the squares divided by the number of values. 
    iqr(): Interquartile range 
    entropy(): Signal entropy
    arCoeff(): Autorregresion coefficients with Burg order equal to 4
    correlation(): correlation coefficient between two signals
    maxInds(): index of the frequency component with largest magnitude
    meanFreq(): Weighted average of the frequency components to obtain a mean frequency
    skewness(): skewness of the frequency domain signal 
    kurtosis(): kurtosis of the frequency domain signal 
    bandsEnergy(): Energy of a frequency interval within the 64 bins of the FFT of each window.
    angle(): Angle between to vectors.

    Additional vectors obtained by averaging the signals in a signal window sample. These are used on the angle() variable:

    gravityMean
    timeBodyAccMean
    timeBodyAccJerkMean
    timeBodyGyroMean
    timeBodyGyroJerkMean
