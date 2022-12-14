# School District Analysis

## Overview of the school district analysis

After creating an initial analysis of standardized tests for the City School District, the school board uncovered evidence of academic dishonesty for the reading and math scores for Thomas High School ninth graders. Because of this, I have been asked to replace the math and reading scores for Thomas High School ninth grader with NaNs while keeping the rest of the data intact. Based on the new results, I will show how each of the seven school district metrics were affected by this change in data.

## Results

### 1. How is the district summary affected?

Original District Summary:

![original_district_summary](Resources/original_district_summary.png)

New District Summary:

![new_district_summary](Resources/new_district_summary.png)

Changes:
There are no significant changes from the original to the new analysis of the district summary. The total schools, students, and budget have not been affected by this change in data; However, there are minor changes to the data in the average math and reading score that result in less than .10. As well as changes in percentages of math, reading, and overall passing. These result in less than a 1% change in data. 

### 2. How is the school summary affected?

Original School Summary:

![original_school_summary](Resources/original_school_summary.png)

New School Summary:

![new_school_summary](Resources/new_school_summary.png)

Changes:
In the new school summary we see significant changes in the math, reading, and overall passing percentages for Thomas High School. while keeping the total number of students (including 9th graders w/ NaNs), we can see a dramatic drop in their passing percentages:

    - % Passing Math: 26% drop
    - % Passing Reading: 27% drop
    - % Overall Passing: 26% drop

### 3. How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

Original School Ranking:

![original_ranking](Resources/original_ranking.png)

New School Ranking:

![new_ranking](Resources/new_ranking.png)

Changes: In the original analysis, Thomas High School ranked 2nd overall amongst the 15 schools. In the new analysis, Thomas High School droppd in rank from 2nd to 8th. 

### 4. How have math and reading scores by grade been affected?

Original Math Scores:

![original_math_scores](Resources/original_math_scores.png)

New Math Scores:

![new_math_scores](Resources/new_math_scores.png)

Original Reading Scores:

![original_reading_scores](Resources/original_reading_scores.png)

New Reading Scores:

![new_reading_scores](Resources/new_reading_scores.png)

Changes:
The new math and reading scores show the change in data for Thomas High School 9th graders. Their scores have been replaced with NaN. All other data has remained intact. 

### 5: How have scores by school spending been affected?

Original Spending Summary:

![original_spending](Resources/original_spending.png)

New Spending Summary:

![new_spending](Resources/new_spending.png)

Changes:
Thomas High School falls into $631-645 spending range. The changes in scores and percentages are very minor.

### 6. How have scores by school size been affected?

Original School Size Data Frame:

![original_school_size](Resources/original_school_size.png)

New School Size Data Frame:

![new_school_size](Resources/new_school_size.png)

Changes:
Thomas High Schools fall into the Medium school size category. Again, there are only minor changes in score and percentages.

### 7. How have scores by school type been affected?

Original School Type Data Frame:

![original_school_type](Resources/original_school_type.png)

New School Type Data Frame:

![new_school_type](Resources/new_school_type.png)

Changes:
Thomas High School is a Charter school so only the data within that row have been affected. Again, the changes are minor. 

## Summary (4 Changes)

1. Thomas High School's percentages for math, reading, and overall passing have dropped over 20%.

2. With the drop in overall passing %, Thomas High School has also decreased in rank from 2nd to 8th amongst the 15 school represented.

3. The data scores by: school spending, school size, and school type, show very little change. The data needed to be formatted to the hundredths place in order to see the change. It is interesting to note that once the 9th, 10th, and 11th grade scores where counted, totaled, and averaged the data remained similar to the original data. It may be interesting to see how data would be affected when the total count of students is recalculated excluding the 9th grade class from Thomas High School.

4. Overall, whether minor or major, the data shows that when the 9th grader's scores were replaced with NaN, the scores and percentages were lowered. Depending on the data frame index property the change affected whichever catergory Thomas High School was placed in. In this case, the $631-645 spending range category, the Medium school size category, and the Charter school type category. This in turn not only affects Thomas High School individual rank, but also lowers other schools who fall into similar categories. 