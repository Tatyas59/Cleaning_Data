#Variables

testData - table contents of test/X_test.txt
trainData - table contents of train/X_train.txt
X - Measurement data. Combined data set of the two above variables
testSub - table contents of test/subject_test.txt
trainSub - table contents of test/subject_train.txt
S - Subjects. Combined data set of the two above variables
testLabel - table contents of test/y_test.txt
trainLabel - table contents of train/y_train.txt
Y - Data Labels. Combined data set of the two above variables.
featuresList - table contents of features.txt
features - Names of for data columns derived from featuresList
keepColumns - logical vector of which features to use in tidy data set
activities - table contents of activity_labels.txt. Human readable
tidyData - subsetted, human-readable data ready for output according to project description.
uS - unique subjects from S
nS - number of unique subjects
nA - number of activities
nC - number of columns in tidyData
td - second tiny data set with average of each variable for each activity and subject

#Output

tidydata.txt
tidydata.txt is a 180x68 data frame.

The tidy data set a set of variables for each activity and each subject. 10299 instances are split into 180 groups (30 subjects and 6 activities) and 66 mean and standard deviation features are averaged for each group

The output represents the average of each variable for each activity and each subject. It is a table ; each variable is represented by a column, and each activity / subject is represented by a row. The columns names are slightly modified from the "features.txt" input file content: all parenthesis are removed. The row names merge the subject and the activity. For instance, the row "1_LAYING" describes the means of the subject 1 for the LAYING activity.
