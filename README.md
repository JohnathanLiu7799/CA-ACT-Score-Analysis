
# ACT Test Scores and the Effects of Socioeconomic Status

A look into the relationships between standardized test performance and factors outside the academic reach.

## Problem Statement

With many colleges cutting standardized tests from their applications <sup>[1](#footnote1)</sup> , the question of the efficacy and necessity of these tests such as the ACT have come into question again. While the creators, ACT Inc., have claimed that these tests are a measure of college preparedness, many others claim that they are far more indicitave of other factors beyond college prepardness<sup>[2](#footnote2)</sup> such as socioeconomic status<sup>[3](#footnote3)</sup>, school district quality, and more. 

How are students from districts or schools with lesser income, faculty, and school resources being impacted when it comes to standardized tests like the ACT?

Citations:

<a name="myfootnote1">1</a>: https://www.nytimes.com/article/sat-act-test-optional-colleges-coronavirus.html

<a name="myfootnote2">2</a>: https://www.ascd.org/el/articles/why-standardized-tests-dont-measure-educational-quality

<a name="myfootnote3">3</a>: https://www.cnbc.com/2019/10/03/rich-students-get-better-sat-scores-heres-why.html


## Data Dictionary

### Data Dictionary

| Field                    	| Description                                    	| Data Type 	|
|--------------------------	|------------------------------------------------	|-----------	|
| num_over_21_score        	| Number of Test Takers that Scored Over 21      	| int64     	|
| percent_over_21_Score    	| Percent of Test Takers that Scored Over 21     	| float64   	|
| per_capita_income        	| Income Per Capita by County                    	| float64   	|
| edp_365                  	| Total School Expenses                          	| float64   	|
| current_expenses_ada     	| Average Daily Attendence with Current Expenses 	| float64   	|
| current_expenses_per_ada 	| Expenses per Average Daily Attendence          	| float64   	|
| teachers                 	| Number of Teachers for 2018-2019               	| float64   	|
| avg_teacher_salary_18_19 	| Average Teacher Salary for 2018-2019           	| float64   	|

## Analysis Summary

Although intially there seems to be a significant negative correlation between school expense factors such as
total school budget, average daily attendence, and current expense per average daily attendence to
standardized test results, these correlation coefficients were the result of Los Angeles Unified acting as an
extreme outlier with incredibly high school expenses as well as average daily attendence, but incredibly low test performance.

After removing Los Angeles Unified from the data, the correlations were far weaker and weren't strong enough to draw any 
meaningful conclusions from.
## Conclusion

With the current data, we can establish no meaningful insights into the relationship
between socioecnomic status or school status as a factor in ACT test scores.

Some steps going forward would include:

1. Getting more specific data that matches in scope. Examples would include individual test scores,
per capita income by school district, individual teacher salary by school, and more.

2. Exploration of the unique situation of Los Angeles Unified to better understand factors that may contribute
to their poor performance.


## Acknowledgements

 - [Awesome Readme Templates](https://awesomeopensource.com/project/elangosundar/awesome-README-templates)
 - [Awesome README](https://github.com/matiassingers/awesome-readme)
 - [How to write a Good readme](https://bulldogjob.com/news/449-how-to-write-a-good-readme-for-your-github-project)
 - [Average Teacher Pay for CA School Districts](https://www.sacbee.com/news/databases/article239621598.html)
 - [California Department of Education](https://www.cde.ca.gov/) 
 - [Census.gov Quickfacts](https://www.census.gov/quickfacts/fact/table/CA/INC110219)
 - [CA ACT Results 2019](https://www.cde.ca.gov/ds/sp/ai/)
 
