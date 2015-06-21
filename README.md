Getting-and-Cleaning-Data-Course-Project
========================================
By  Marcelo Ferreira.

This file describes how run_analysis.R script works.

* First, unzip the data from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip  a
	- After download, uncompress the file getdata-projectfiles-UCI HAR Dataset.zip
	- rename the folder "UCI HAR Dataset" to "data".
	- Make sure the folder "data" and the run_analysis.R script file are both in the current working directory.
* Second, use source("run_analysis.R") command in RStudio. 
* Third, you will find two output files are generated in the current working directory:
  - merged_data.txt: it contains a data frame called cleanedData with 10299*68 dimension.
  - data_with_means.txt: it contains a data frame called result with 180*68 dimension.
* Finally, use data <- read.table("data_with_means.txt") command in RStudio to read the file. Since we are required to get the average of each variable for each activity and each subject, and there are 6 activities in total and 30 subjects in total, we have 180 rows with all combinations for each of the 66 features. 
