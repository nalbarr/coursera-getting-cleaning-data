# Coursera - Getting and Cleaning Data
# Week 4 - Project
## Student:  Narciso Albarracin

### Overview
This project is the intended to synthesize and validate skills acquired during this course including collecting, working with and cleaning data sets.  Specifically, we will be manipulating a data set related to human activity tracking from smart phone sensors and finally creating *tidy* data sets.  

Coursera has made this data available at:  [https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip] with background and original research context at:  [http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones].

Analysis and processing this human activity tracking data set requires application of both course instructors' teaching (Leek, Peng, Caffo) and interpretation of Hadley Wickham's *tidy data* principles as described in:  [https://www.jstatsoft.org/article/view/v059i10]

Tidy datasets are easy to manipulate, model and visualize... have a specific structure: each variable is a column, each observation is a row, and each type of observational unit is a table).

I attempt to apply these principles with R programming but also in applying proper semantic by documenting my approach via a code book that accompanies a data analysis script.

Additionally, where possible I apply as much of Wickhams's convenience packags such as data.table, dplyr and attempt to use a more functional coding style by using R collections and declarative lapply, etc. processing where possible.

### Objectives

This project demonstrated data analysis by an R script called run_analysis.R that does the following.

- Merges the training and the test sets to create one data set.
- Extracts only the measurements on the mean and standard deviation for each measurement.
- Uses descriptive activity names to name the activities in the data set
- Appropriately labels the data set with descriptive variable names.
- From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

### Artifacts

Artifact | Description | File name
-------- | ----------- | ---------
README source   | Project overview document | README.md (this file)
README | (generated) | README.html
Code book source | Describes all data set semantics | CodeBook.md
Code book | (generated) | CodeBook.html
R script | Input file processing, manipulation and final tidy data set creation | run_analysis.R
Final data set | Tidy data set| tidy_output.txt

### Assumptions

#### Inputs
Input UCI Human Activity Recognition (HAR) data set has been downloaded to your current working directory expanded to a local folder named:  "UCI HAR Dataset".  For convenience, this has been included in the repository

For convenience the input data files have been included pre downloaded as original .zip file and already expanded in Git repository.

#### Outputs
- README.html
- CodeBook.html
- tidy_ouput.txt

#### Environment and Dependencies

##### Environment
This project assumes the following design and run time execution environment.  
RStudio installed with the specified versions below:

- R Studio, version 0.99.893 or later
- R version 3.2.4 (2016-03-16) or later

R packages include:
- base
- data.table
- dpylr
- knit

##### Operating System (OS)
This project was designed and tested on the following specific environment:
- Hardware:  Intel - 64 bit machine
- OS: Windows 10

##### Data
This project assumes you have input files downloaded from [...] and placed in the current directory of where you have cloned the Git repository.  

#### Project Criteria

- The submitted data set is tidy. - COMPLETED
- The Github repo contains the required scripts. - COMPLETED
- GitHub contains a code book that modifies and updates the available codebooks with the data to indicate all the variables and summaries - COMPLETED calculated, along with units, and any other relevant information. - COMPLETED
- The README that explains the analysis files is clear and understandable. - COMPLETED
- The work submitted for this project is the work of the student who submitted it. - COMPLETED

#### How to evaluate this project

- Check assumptions (i.e. dataset available locally)
- Open RStudio or commandline prompt with Rscript in environmet PATH
- Read READM.html and CodeBook.html documentation
- Run analyis run_analysis.R
- Check for output file
- Review analysis file as needed for context
 