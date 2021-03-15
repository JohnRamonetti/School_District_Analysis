# School_District_Analysis

## Overview

### The objective of the current analysis was to review and assess the total standardized test data for the 15 schools comprising a city school district.  Test scores (math and reading) were received for all students in the district and organized by school.  The data was reviewed, cleaned, and organized in a logical format.  Summaries were prepared for for the district and each school, then the data was manipulated to see patterns that may relate to student success in taking the standardized tests.

### Additionally, there was an issue exposed regarding potentially compromised test scores, specifically involving the 9th grade at Thomas High School (THS).  This data had to be considered and dealt with appropriately.  The data was removed from the dataset and the district-wide analysis was repeated without the scores in question.  In other words, the entire set of scores for 9th graders at Thomas High School was not considered.

## Resources
- Data Source: [schools_complete.csv](resources/schools_complete.csv), [students_complete.csv](Resources/students_complete.csv)
- Software: Python 3.7.7, Anaconda, Jupyter Notebook 6.1.4

## Results
- The [district summary](Resources/SCREENSHOTS/District_Summary.png) shows that the district comprises 15 schools with a Total Budget of almost $25M.  There were 39,170 students receiving scores for the standardized math and reading exams. Passing percentages were 75% and 86% for math and reading respectively. The overall passing rate for the district (i.e., students who passed both math and reading exams) was 64.9%, after disqualifying the questionable test scores.  Excluding the THS scores had a very minor negative effect on this total, since the THS score average was slightly higher than the district average.  However, the 461 compromised scores only represent approximately one (1) percent of the total scores, so the impact was not dramatice on this metric.
- The next tabulation is the (School Summary)[]. This table shows the diversity of average scores and passing rates in the district.  The compromised scores affected only Thomas High School, where the 9th grade "questionable" averages were similar to the 10th, 11th, and 12th grade averages, so again the impact of dropping the questioned scores was not very significant.
- Across the district, the (highest and lowest performing schools)[] are evident.  Despite the compromised test scores at THS, Thomas HS appears in the number 2 spot for top-performing schools, with an overall passing rate of almost 91%.
- Additionally:
   - (Average Math and reading)[] scores are shown in the attached DataFrames.  Again, since the 9th grade average scores, based on questionable score data, for (math)[] and (reading)[] were very similar to the respective THS school averages, the overall impact on Thomas High School average scores was not significant.
   - Schools were grouped by the average spending per student to see if there was any correlation between spending and student success.  In fact, there was a very strong negative correlation, clearly showing a relationship between higher per student spending and lowere passing rates!
   - (School size)[] also showed a strong correlation with student success.  The largest schools (2000 to 5000 student population), on average, had much lower overall passing rates on standardized exams (average 58%) versus small (average 91%) or medium (average 90%) schools.
   - (Type of school)[] (district vs. charter) was also examined. Charter schools averaged overall passing rates of 90%, while district schools averaged only 54% overall passing on standardized tests.
        
## Summary

### While we are naturally concerned about the compromised test scores at Thomas High School, the reality is that the greatest impact of those compromised tests was on the 9th graders at THS.  The 9th grade at THS represents only approximately 1% of the total district student population, so dropping those scores affected the overall district-wide passing average, but only very slightly.  
### More importantly, we have shown here several correlations that can be considered when discussing how to make improvements in the district regarding student success.  Firstly, and perhaps counter-intuitively, there appears to be a negative correlation between average per student spending and student success.  The schools with the highest average student spending had the lowest average passing percentages.  Secondly, while small and medium-sized schools had similar passing rates, large schools had significantly lower passing rates.  Thirdly, the type of school matters - charter schools examined her had much higher success rates than district schools (90% versus 54%).  Finally, it is important to note that the top schools in the district, based on testing scores, were all charter schools, and the worst schools in the district, based on testing scores, were all district schools.

