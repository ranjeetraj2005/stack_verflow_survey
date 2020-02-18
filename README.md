Readme:
Project Motivation and Details:

This is step into to explore Stack Overflow Developer Survey, 2017.
Every year, Stack Overflow conducts a massive survey of people on the site, covering all sorts of information like programming languages, salary, code style and various other information. 
This year, they amassed more than 64,000 responses fielded from 213 countries.

My work:
A look into the lives of over 64,000 Stack Overflow developers.
I tried to solve 3 Business Understanding questions Related to business or real-world applications of how the data could be used to solve.

Q1 : What are the most popular programming languages among developers?

Q2 : How do different programming languages stands in terms of job satisfaction?

Q3 : Base programming language to start professional career?

Dataset:

We will use the data of StackOverflow's Developer Survey for year 2017. 
#download dataset URL : https://www.kaggle.com/stackoverflow/so-survey-2017

Libraries used:
Numpy, Pandas, matplotlib

Files used in the project:
stack_overflow_survey_2017_data.ipynb - complete model file for overall problem solution addressed in project motivation

Summary of the results:

Solution 1: What are the most popular programming languages among developers?

Data Understanding:

check the proportion of missing values in "HaveWorkedLanguage" columns.
Result : 28% found missind data in column

Prepare Data:
i Rertieve programming languages in particular year and Get common programming languages in data.
I clean up language columns based on a list of strings you want to search for in each row.
So finally i got all the proportion of languages.

![alt text](https://github.com/ranjeetraj2005/stack_verflow_survey/blob/master/result/so_survey_plot1_prog_lang_result.png)

So finally i got rankings of common languages by merging the data with all dictionary data.


![alt text](https://github.com/ranjeetraj2005/stack_verflow_survey/blob/master/result/so_survey_q1_prog_lang_result.png)

So finally i could conclude , "Javascript" is most popular programming languages among developers

Solution 2 : How do different programming languages stands in terms of job satisfaction?
Prepare Data:
Because each year survey has a different job satisfaction level, we have to re-encode those fine scales into the same rough scale before comparison and column "JobSatisfaction_encoded" re-encoded column for the purose.

So i write a function "total_count_job_sat()" to count total job count by satistfaction level.
then "clean_job_sat()" to remove unwatnted listing

Finally to merge the "job_sat_mean" column to get result.

![alt text](https://github.com/ranjeetraj2005/stack_verflow_survey/blob/master/result/so_survey_q2_prog_lang_result.png)

So finally i conclude "typescript" is most satified language in terms of job satisfaction

Solution 3 : Base programming language to start professional career?
I tried to figure out the proportion of years of code of each language in each year. and found Assempbly language is basic starting language for early career choice.

![alt text](https://github.com/ranjeetraj2005/stack_verflow_survey/blob/master/result/so_survey_plot2_prog_lang_result.png)

when i figure out 'matlab' proportion is 0.7 of new-comers of and get highest rankings of common languages.

![alt text](https://github.com/ranjeetraj2005/stack_verflow_survey/blob/master/result/so_survey_q3_prog_lang_result.png)

i conclude "Matlab" is most basic language that every developer start learning in their professional career.

Acknowledgements:
Like so many projects, this effort has roots in many places. thanks to https://www.kaggle.com/stackoverflow/so-survey-2017 page that has dataset and many previous task done in past related to conclude my project motivation.
