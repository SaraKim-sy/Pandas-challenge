# Pandas-challenge - PyCity Schools

## Table of contents
  * [Introduction](#introduction)
  * [Observable Trends Based on the Data](#trends)
  * [Final Report](#final-report)
    * [District Summary](#district-summary)
    * [School Summary](#school-summary)
    * [Top Performing Schools (By % Overall Passing)](#top-performing-schools)
    * [Bottom Performing Schools (By % Overall Passing)](#bottom-performing-schools)
    * [Math Scores by Grade](#math-scores-by-grade)
    * [Reading Scores by Grade](#reading-scores-by-grade)
    * [Scores by School Spending](#scores-by-school-spending)
    * [Scores by School Size](#scores-by-school-size)
    * [Scores by School Type](#scores-by-school-type)
  * [Technologies](#technologies)
  
## <a name="introduction"></a> Introduction
This project is to analyze the district-wide standardized test results using python and pandas to help the school board and mayor make strategic decisions regarding future school budgets and priorities. The dataset will include every student's math and reading scores, as well as various information on the schools they attend. The purpose of this project is to aggregate the data to and showcase obvious trends in school performance. 
* Inside a PyCitySchools folder, you will find the following:
  * A jupyter notebook file called [**school_test_results_analysis.ipynb**](./PyCitySchools/school_test_results_analysis.ipynb), which is the main script to run for analyzing the district-wide standardized test results.
  * A "Resources" folder that contains two CSV files used; one is called [**schools_complete.csv**](./PyCitySchools/Resources/schools_complete.csv). This dataset is composed of five columns: `School ID`,	`school_name`,	`type`,	`size`,	`budget`. The other dataset is called [**students_complete.csv**](./PyCitySchools/Resources/students_complete.csv). This dataset is composed of seven columns: `Student ID`,	`student_name`,	`gender`, `grade`, `school_name`,	`reading_score`,	`math_score`. I imported and merged these two datasets using the pandas library and Jupyter Notebook to analyze test results and draw observable trends based on the data. 
* The [**final report**](#final-report) includes District Summary, School Summary, Top Performing Schools (By % Overall Passing), Bottom Performing Schools (By % Overall Passing), Math Scores by Grade, Reading Scores by Grade, Scores by School Spending, Scores by School Size, and Scores by School Type. 

## <a name="trends"></a> Observable Trends Based on the Data
1. Seeing the Scores by School Spending, the lowest spending ranges per student (less than $584) schools group has the highest average math scores, average reading scores, percentage of students passed math, percent of students passed reading, and percentage of students passed both. The higher budget spent per student, the lower average math scores, average reading scores, percent of students passed math, the percentage of students passed reading, and the percentage of students passed both.

2. Looking at the Scores by School Size, the small-sized schools' group (<1000) has the highest average math score and average reading score. Also, the medium-sized schools' group(1000-2000) has the highest percentage of students passed math, percent of students passed reading, and percent of students passed both. However, all the gaps between small and medium schools are not big; all the results were very similar. 
* However, the large-sized schools' group(2000-5000) has quite lower results than small/medium-sized schools. For example, the percentage of students who passed math in large-sized schools was about 23.6% lower than that of small-sized schools, and the percentage of students who passed reading in large-sized schools was about 31.6% lower than that of small-sized schools. 
* From these results, we can assume that students in small/medium-sized schools tend to perform better in tests than those who go to large-sized schools with many students. 

3. From the Scores by School Type, we can notice that charter schools have higher average math scores, average reading scores, percentage of students passed math, percent of students passed reading, and percentage of students passed both than those of district schools. Moreover, according to the Top Performing Schools (By % Overall Passing), all the top 5 performing schools were charter schools. On the other hand, all the bottom 5 performing schools were large district schools with 2000-5000 students.

4. Observing Math Scores by Grade and Reading Scores by Grade, we can see that math and reading scores between different grades in each school are very close. We can say that students' performance levels are very similar within the same schools, regardless of their grades(9th to 12th). 

## <a name="final-report"></a> Final Report
The notebook displays the whole test results analysis is available in this link: [Final Report](https://nbviewer.jupyter.org/github/SaraKim-sy/Pandas-challenge/blob/main/PyCitySchools/.ipynb_checkpoints/school_test_results_analysis-checkpoint.ipynb) 

### <a name="district-summary"></a> District Summary
* A high level snapshot (in table form) of the district's key metrics, including:
  * Total Schools
  * Total Students
  * Total Budget
  * Average Math Score
  * Average Reading Score
  * % Passing Math (The percentage of students that passed math.)
  * % Passing Reading (The percentage of students that passed reading.)
  * % Overall Passing (The percentage of students that passed math and reading.)

### <a name="school-summary"></a> School Summary
* An overview table that summarizes key metrics about each school, including:
  * School Name
  * School Type
  * Total Students
  * Total School Budget
  * Per Student Budget
  * Average Math Score
  * Average Reading Score
  * % Passing Math (The percentage of students that passed math.)
  * % Passing Reading (The percentage of students that passed reading.)
  * % Overall Passing (The percentage of students that passed math and reading.)

### <a name="top-performing-schools"></a> Top Performing Schools (By % Overall Passing)
* A table that highlights the top 5 performing schools based on % Overall Passing. Include:
  * School Name
  * School Type
  * Total Students
  * Total School Budget
  * Per Student Budget
  * Average Math Score
  * Average Reading Score
  * % Passing Math (The percentage of students that passed math.)
  * % Passing Reading (The percentage of students that passed reading.)
  * % Overall Passing (The percentage of students that passed math and reading.)

### <a name="bottom-performing-schools"></a> Bottom Performing Schools (By % Overall Passing)
* A table that highlights the bottom 5 performing schools based on % Overall Passing. Include:
  * School Name
  * School Type
  * Total Students
  * Total School Budget
  * Per Student Budget
  * Average Math Score
  * Average Reading Score
  * % Passing Math (The percentage of students that passed math.)
  * % Passing Reading (The percentage of students that passed reading.)
  * % Overall Passing (The percentage of students that passed math and reading.)


### <a name="math-scores-by-grade"></a> Math Scores by Grade
* A  table that lists the average Math Score for students of each grade level (9th, 10th, 11th, 12th) at each school.

### <a name="reading-scores-by-grade"></a> Reading Scores by Grade
* A table that lists the average Reading Score for students of each grade level (9th, 10th, 11th, 12th) at each school.

### <a name="scores-by-school-spending"></a> Scores by School Spending
* A table that breaks down school performances based on average Spending Ranges (Per Student). Include in the table each of the following:
  * Average Math Score
  * Average Reading Score
  * % Passing Math (The percentage of students that passed math.)
  * % Passing Reading (The percentage of students that passed reading.)
  * % Overall Passing (The percentage of students that passed math and reading.)

### <a name="scores-by-school-size"></a> Scores by School Size
* A table that breaks down school performances based on reasonable approximation of school size (Small, Medium, Large). Include in the table each of the following:
  * Average Math Score
  * Average Reading Score
  * % Passing Math (The percentage of students that passed math.)
  * % Passing Reading (The percentage of students that passed reading.)
  * % Overall Passing (The percentage of students that passed math and reading.)


### <a name="scores-by-school-type"></a> Scores by School Type
* A table that breaks down school performances based on school type (Charter vs. District). Include in the table each of the following:
  * Average Math Score
  * Average Reading Score
  * % Passing Math (The percentage of students that passed math.)
  * % Passing Reading (The percentage of students that passed reading.)
  * % Overall Passing (The percentage of students that passed math and reading.)

## <a name="technologies"></a> Technologies
Project is created with:
* Python 3.8
* Jupyter Notebook
* Pandas
