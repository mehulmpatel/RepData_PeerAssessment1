Reproducible Research: Peer Assessment 1
===============================

This assignment is to analyze a set of data and document it. So that it is reproducible by others. 

The components of this repo are as follows:  

* A R markdown file of the data analysis. (PA1_template.Rmd)  
* Used data for analysis (downloaded csv). (steps_data.csv)  
* A html file corresponding to the rmd file.  (PA1_template.html)  
#######3* Plots in the document.  

Please find more details as mentioned below for this assignment, detailed breakdown of the various components.

## Introduction

There is a "quantified self" movement - a group of enthusiasts who take measurements about themselves regularly to improve their health, to find patterns in their behavior, or because they are tech geeks. But these data remain under-utilized both because the raw data are hard to obtain and there is a lack of statistical methods and software for processing and interpreting the data.

Tools such as Fitbit, Nike Fuelband, Jawbone Up has allowed for the collection of personal movement data. In the dataset we have data from these device. This device collects data at 5 minute intervals through out the day. The data consists of two months of data from an anonymousindividual collected during the months of October and November, 2012 and include the number of steps taken in 5 minute intervals each day.

We are going to use this data from a personal activity monitoring device for our assignment.


## Data

The data for this assignment can be downloaded from the course web site:

* Dataset: [Activity monitoring data](https://d396qusza40orc.cloudfront.net/repdata%2Fdata%2Factivity.zip)

The variables included in this dataset are:

* **steps**: Number of steps taking in a 5-minute interval (missing values are coded as `NA`)

* **date**: The date on which the measurement was taken in YYYY-MM-DD format

* **interval**: Identifier for the 5-minute interval in which measurement was taken

The dataset is stored in a comma-separated-value (CSV) file and there are a total of 17,568 observations in this dataset.


## Assignment Details:

### **Loading the data and preprocessing.**
  1. Loading data using read.csv().    
  2. Processing the data into a format fit for analysis.
  
### **What is the mean total number of steps taken per day?**
  1. (Ignoring NA values) calculate the total number of steps taken per day.  
  2. Make a histogram of the total number of steps taken per day.  
  3. Compute the mean and median of the total steps per day. 
  
### **What is the average daily activity pattern?**
  1. Make a time series plot (i.e. type = "l") of the 5-minute interval (x-axis) and the average number of steps taken, average across all days (y-axis).  
  2. Which 5-minute interval, on average across all the days in the dataset, contains the maximum number of steps?  
  
### **Imputing missing values -** Presence of NA days may introduce bias into some calculations or summaries of the data.  
  1. Calculate and report the total number of mising values in the data set (total number of rows in NA).  
  2. Devise a strategy for filling in all of the missing values in the data set. Example, the mean or median for the day could be used or the mean for the five minute interval.  
  3. Create a new dataset that is equal to the original dataset with the missing NA values filled in.  
  4. Make a histogram of the total number of steps taken each day, Calculate and report the median and mean total number of steps per day. How do these values compare to the cases where NA values were simply ignored? What is the impact of imputing missing data on the estimates of the total daily number of steps taken?
  
### **Are there differences in activity patterns between weekdays and weekends?** weekdays() function might be useful for this part. Use the data set with the filled in missing values.  
  1. Create a new factor variable in the dataset with the two levels - "weekdays" and "weekend".  
  2. Make a panel plot containing the time series plot (i.e. type = "l") of the five-minute interval and the average number of steps taken averaged across all weeday days and weekend days (y-axis).  
