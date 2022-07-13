# school_district_analysis
## Overview & Scope of School Metrics Analysis
### Initial Analysis: Comprehensive Analysis
This project was undertaken to provide a comprehensive school district analysis across metrics for reading, math and overall success measured against school size, type and budget per student to the School District Board. The analysis will help reinforce statistics derived from math and reading scores across all grades for 15 district high schools and the results will help the school board drive decisions about predictors for success. 

After analysis was complete, the school board became aware of compromised data: specifically the reading and math scores for 9th graders at Thomas High School (THS) needed to be nulled because of evidence of dishonesty in the reporting. The implications of omitting the polluted data are discussed in the results section as a comparison of before and after voiding the 9th grade scores of Thomas High School.

### Secondary Comparative Analysis: Excluding Compromised Data
A full analysis of the schools districts was delivered to the school board for review. Please see PyCitySchool_Challenge.ipynb in the resources folder for the full scipt run on the data. The second signifact deliverable to the school board was a comparative analysis of the success metrics including the statistics from the 9th graders at Thomas High School and the analysis excluding the compromised data. The school board was intent on knowing how much the polluted data impacted the results. Replacing the ninth graders' math and reading scores with "NaN" to void the scores resulted in the following changes:


## Results: Relative Impact Before & After Compromised Data Removal

### Thomas High School Summary Results

![school_summary_after](https://user-images.githubusercontent.com/107326987/178740422-24aa3744-7dd9-4137-9206-1a6e33fd2849.png)

THS overall school wide average scores were impacted by voiding the 9th grades scores. Before ommitting the compromised data, the % Passing Math, % Passing Reading and % Overall Passing were 93.2%, 97.3% and 90.9% respectively. The new data points for the same metrics now read at 93.2% 97.0% and 90.6% respectively. The greatest variance from before and after omission is +/-0.03%.

### Relative Performance Change of Thomas High School

![thomas_relative_performance_no9](https://user-images.githubusercontent.com/107326987/178741364-31929544-f03a-4d89-af36-66c41f162eb7.png)

The districut summary statistics were ranked in descending order of overall success based on the "% Overall Passing" metric - a measurement of the averages of % passing reading and math totals. THS % Overall Passing metric dropped 0.3% - THS's relative performance was unchanged, they continue to be ranked second. 

### District Wide Summary Results

![district_summary_after](https://user-images.githubusercontent.com/107326987/178743548-1a76b7f2-be09-4c8e-9cb1-f020f3cfc313.png)

The impact of the polluted data was prescribed exclusively to THS's singular performance. The impact to their performance was minimual enough that it did not move the needle on any of the metrics for the district.

### Math & Reading Scores by Grade

![math_by_school_after](https://user-images.githubusercontent.com/107326987/178744616-e2318d87-dc84-4b7f-b987-20dc5a242ee8.png)
![reading_by_school_after](https://user-images.githubusercontent.com/107326987/178744633-79a9370e-ce0b-4063-9a2a-8ae113b57d91.png)

The math and reading scores by grade, above images 1 and 2 respectively, remain unchanged aftering voiding the 9th grades scores at THS.

### Scores by School Spending

![school_spending_after](https://user-images.githubusercontent.com/107326987/178745106-9f82d8f0-6ced-49b8-8555-b59e2aece927.png)

The scores by school spending remain unchanged aftering voiding the 9th grades scores at THS. We can draw some conclusions based on patterns we represented in the data. We can see intrestingly that as you increase the spending per student, we see a inverse affect on grades. This might be antithetical to general assumptions about spending and budget impacts on student performance and is an important revelation in the data analysis for the school board.

### Scores by School Size

![scores_by_size_before](https://user-images.githubusercontent.com/107326987/178745149-e6bea754-7963-4984-9f35-798130ce01ed.png)

The scores by school size remain unchanged aftering voiding the 9th grades scores at THS. We can see a relationship between the size of the school and school performance; as the school size increase performance averages tend to decrease. We suggest further analysis for the school board to plot the relationship between spending per student and school size that would help tell the full story of the data.

### Scores by School Type

![scores_by_type_after](https://user-images.githubusercontent.com/107326987/178745174-e99ccd81-970d-41a8-b20a-a771f0b94e55.png)

The scores by school type remain unchanged aftering voiding the 9th grades scores at THS. We can see however that there is a marked difference in the average perforamnces of district schools versus charter schools. At the minimum there is a 6 point difference across the Average Math Score in favor of Charter schools. At most, we see a remarkable 36 point difference across the Overall Passing scores in favor of Charter Schools. This is the most distinct realization in the data across any of the metrics we measured against. 

## Summary: 
In order to maintain the integrity of the school district data and make it comparable and compatible with larger datasets, it was critical to remove all compromised data. We can deduce, however, that while they're may have been dishonesty in the reporting of the 9th grade scores for THS, the data was consistent with the overall set. The voided scores were not artificially impacting the larger set and while removing data points is not ideal - the school board can use this data with confidence as a true representation of the per school metrics and district wide metrics of success. The negligiable change

## Resources
Resources: All raw data files used in the analysis can be found inside of the resources folder.

Software: Python 3.7, Anaconda, Jupyter Notebook
