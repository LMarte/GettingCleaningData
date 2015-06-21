## Getting and Cleaning Data - Project

Source dataset https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 

* You should create one R script called run_analysis.R that does the following. 
* Merges the training and the test sets to create one data set.
* Extracts only the measurements on the mean and standard deviation for each measurement. 
* Uses descriptive activity names to name the activities in the data set
* Appropriately labels the data set with descriptive variable names. 
* From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

## Notes

*  Only variables containing mean() & std() are used.
*  Requires the plyr & reshape2 packages.
*  Assumes that the dataset is unzipped in the working directory.

Constructed using the following:

```R
> version
platform       x86_64-w64-mingw32          
arch           x86_64                      
os             mingw32                     
system         x86_64, mingw32             
status                                     
major          3                           
minor          1.3                         
year           2015                        
month          03                          
day            09                          
svn rev        67962                       
language       R                           
version.string R version 3.1.3 (2015-03-09)
nickname       Smooth Sidewalk  
```

##  Running

```bash
$ Rscript run_analysis.R
```

Yields tidy.txt & tidy.mean.txt.
