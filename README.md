## Overview & Scope of School Metrics Analysis
### Initial Analysis: Distrcit Wide Statistical Analysis of Student Performance Metrics
This project was undertaken to provide a comprehensive school district analysis across metrics for reading, math and overall success measured against school size, school type and budget to be delivered to the School District Board. The analysis will help reinforce statistics derived from math and reading scores across all grades for 15 district high schools and the results will help drive informed decision making at the district level based on predictors for success. 

### Secondary Comparative Analysis: Excluding Compromised Data
A full analysis of the school district was delivered to the school board for review (please see PyCitySchool_Challenge.ipynb in the resources folder for the full scipt run on the data). After analysis was complete, the school board became aware of compromised data: evidence of dishonesty in the reporting was suspected in the reading and math scores for 9th graders at Thomas High School (THS). The School District Board requested a secondary analysis be run voiding all values for THS grade 9. The second signifact deliverable to the school board was a comparative analysis of the performance metrics including versus excluding the compromised data points. The school board was intent on knowing how much the polluted data impacted the district summary results. The implications of omitting the compromised data are discussed in the results section.

## Results: Relative Impact Before & After Compromised Data Removal

### Thomas High School Summary Results

![school_summary_after](https://user-images.githubusercontent.com/107326987/178740422-24aa3744-7dd9-4137-9206-1a6e33fd2849.png)

THS's overall school-wide average scores were impacted by voiding the 9th grade scores. Before ommitting the compromised data, the "% Passing Math", "% Passing Reading" and "% Overall Passing" values were 93.2%, 97.3% and 90.9% respectively. After eliminating the compromised data the new data points for the same metrics now read at 93.2%, 97.0% and 90.6% respectively. The greatest variance between before and after omission values is +/-0.03%. The data set is negligibly impacted by voiding and adjusting school-wide values for THS - we can conclude that the data provided for the 9th grade class was primarily consistent with the data for grades 10 - 12. 

### Relative Performance Change of Thomas High School

![thomas_relative_performance_no9](https://user-images.githubusercontent.com/107326987/178741364-31929544-f03a-4d89-af36-66c41f162eb7.png)

The district summary statistics ranked all district high schools in descending order based on the "% Overall Passing" metric - a measurement of the averages of school wide % passing reading and math totals. THS "% Overall Passing" metric dropped 0.3% once the 9th grade scores were voided - THS's relative performance was unchanged, they continue to be ranked second overall. 

### District Wide Summary Results

![district_summary_after](https://user-images.githubusercontent.com/107326987/178743548-1a76b7f2-be09-4c8e-9cb1-f020f3cfc313.png)

The impact of the polluted data was prescribed exclusively to THS's singular performance. The impact to their performance was minimual enough that it did not move the needle on any of the district wide metrics when measured to 0.0% accuracy.

### Math & Reading Scores by Grade

![math_by_school_after](https://user-images.githubusercontent.com/107326987/178744616-e2318d87-dc84-4b7f-b987-20dc5a242ee8.png)
![reading_by_school_after](https://user-images.githubusercontent.com/107326987/178744633-79a9370e-ce0b-4063-9a2a-8ae113b57d91.png)

The math and reading scores by grade, above images 1 and 2 respectively, remain unchanged aftering voiding the THS 9th grade scores.

### Scores by School Spending

![school_spending_after](https://user-images.githubusercontent.com/107326987/178745106-9f82d8f0-6ced-49b8-8555-b59e2aece927.png)

The scores by school spending remain unchanged aftering voiding the THS 9th grade scores. As a stand alone chart, we can draw conclusions based on patterns represented in the data. We can see intrestingly that as spending per student increases, there is an inverse relationship with average grade and passing rates. This relatinoship between budget per student and performance is antithetical to the general assumptions about budget impacts on student performance. It is an important revelation in the data analysis to deliver to the school board.

### Scores by School Size

![scores_by_size_before](https://user-images.githubusercontent.com/107326987/178745149-e6bea754-7963-4984-9f35-798130ce01ed.png)

The scores by school size remain unchanged aftering voiding the 9th grades scores at THS. We can see a relationship between the size of the school and school performance; as the school size increase performance averages tend to decrease. We suggest further analysis for the school board to plot the relationship between spending per student and school size that would help tell the full story of the data.

### Scores by School Type

![scores_by_type_after](https://user-images.githubusercontent.com/107326987/178745174-e99ccd81-970d-41a8-b20a-a771f0b94e55.png)

The scores by school type remain unchanged aftering voiding the THS 9th grades scores. We can see however that there is a marked difference in the average perforamnces of district schools versus charter schools. At the minimum there is a 6 point difference across the Average Math Score in favor of Charter schools. At most, we see a remarkable 36 point difference across the Overall Passing scores in favor of Charter Schools. This is the most distinct realization in the data across any of the metrics we measured. 

## Summary: 
In order to maintain the integrity of the school district data and make it comparable and compatible with larger datasets, it was critical to remove all compromised data. We can deduce, however, that while they're may have been dishonesty in the reporting of the 9th grade scores for THS, the data was consistent with the overall set. The voided scores were not artificially impacting the larger set and while removing data points is not ideal - the school board can use results from this analysis with confidence as a true representation of the per school performance metrics and district wide performance metrics. 

## Resources
Resources: All raw data files used in the analysis can be found inside of the resources folder.

Software: Python 3.7, Anaconda, Jupyter Notebook
