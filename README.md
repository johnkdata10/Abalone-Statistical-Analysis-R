# R Data Analysis Overview:

Two data analysis projects using abalone data are completed in this repository. The first data analysis project entails exploratory data analysis. The second data analysis project involves statistical inference using analysis of variance and linear regression. Binary decision rules will be evaluated and a Receiver Operating Characteristic (ROC) curve developed.

## Overall Background:
We are bombarded daily with statements or claims arising from surveys and studies that use data to generate statistics. In a world where data are becoming more abundant every day, as an educated consumer, it is essential to think critically about the information we receive and the decisions that will be made based on that information. Part of this involves considering the source of the data, how it was collected, how it was analyzed and whatever limitations there may be to the conclusions reached and claims being made.
As analysts we must be prepared to apply sound statistical and critical thinking to a wide variety of situations. Being able to do so is the mark of an accomplished analyst. This project assignment is one example.

## Project Background:
Abalones are an economic and recreational resource that is threatened by a variety of factors which include: pollution, disease, loss of habitat, predation, commercial harvesting, sport fishing and illegal harvesting. Environmental variation and the availability of nutrients affect the growth and maturation rate of abalones. Over the last 20+ years it is estimated the commercial catch of abalone worldwide has declined in the neighborhood of 40%. Abalones are easily over harvested because of slow growth rates and variable reproductive success. Being able to quickly determine the age composition of a regional abalone population would be an important capability. The information so derived could be used to manage harvesting requirements.

#### Supplemental information may be obtained from the following sources:
http://www.fishtech.com/facts.html http://www.marinebio.net/marinescience/06future/abintro.htm

## Background information concerning the assignment data:
The assignment data are derived from an observational study of abalones. The intent of the investigators was to predict the age of abalone from physical measurements thus avoiding the necessity of counting growth rings for aging. Ideally, a growth ring is produced each year of age. Currently, age is determined by drilling the shell and counting the number of shell rings using a microscope. This is a difficult and time consuming process. Ring clarity can be an issue. At the completion of the breeding season sexing abalone can be difficult. Similar difficulties are experienced when trying to determine the sex of immature abalone.
The study was not successful. The investigators concluded additional information would be required such as weather patterns and location which affect food availability.

## R_data_analysis_1
Exploratory data analysis to determine plausible reasons why the original study was unsuccessful in predicting abalone age based on physical characteristics.

## R_data_analysis_2
Involves development of a regression model; and, also address development of binary decision rules and a Receiver Operating Characteristic (ROC) curve.

## Data set:
abalones.csv

## Data Description:
This data file is derived from study of abalones in Tasmania. There are 1036 observations and eight variables. The CLASS variable has been added for these projects.

#### Note: When data sets are made available for public use, the original owners may obscure variable names or scale the data differently from original measurements. There are different reasons for this. This is the case with these data and will be ignored for this assignment. Basic facts remain.

1. SEX=M(male), F (female), I (infant)
2. LENGTH= Longest shell length in cm
3. DIAM = Diameter perpendicular to length in cm
4. HEIGHT = Height perpendicular to length and diameter in cm
5. WHOLE = Whole weight of abalone in grams
6. SHUCK = Shucked weight of meat in grams
7. RINGS = Age (+1.5 gives the age in years)
8. CLASS = Age classification based on RINGS (A1= youngest,., A6=oldest)

### Additional Features:
Additional features that are relevant to answer the questions can be created. In this case, there are 2 additional features that seem relevant. (i) I calculated a new variable VOLUME by multiplying LENGTH, DIAM and HEIGHT together. VOLUME is related to the overall size of an abalone. (ii) I calculated a new variable called RATIO by dividing SHUCK by VOLUME. RATIO is related to the proportion of meat in an abalone.

### Exploratory data analysis
EDA is a process of detective work which may lead to important insights. EDA by its nature tends to be visual. When starting to analyze data, a few good plots may save you hours of pouring over tables and summary statistics. This assignment will use important EDA methods to display aspects of these data such as:
1. The center or location of distributions.
2. The variation in different variables.
3. The shape of various distributions.
4. The presence of outliers.
5. The differences in data characteristics between abalone classifications.

These projects involve development of a regression model; and, also address development of binary decision rules and a Receiver Operating Characteristic (ROC) curve for harvesting abalones. Use the abalones.csv file to follow along.

Real data are usually not perfect and that is the case here. This work suggests hypotheses that need confirmatory testing, and it identifies difficulties with the data that need to be addressed in subsequent analyses or future studies of abalones. R_data_analysis_2 builds upon what is found in R_data_analysis_1.
