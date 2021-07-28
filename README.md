# Panda_analysis
Module 4 - PyCitySchools with Pandas

## Project Overview

The school board has notified Maria that the database used shows evidence of academic dishonesty. Specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. The school district analysis that was previously done needs to be updated once these changes might affect the overall analysis. 

Deliverable 1
- [x] 1. Replace reading and math scores from Thomas High School with NaNs

Deliverable 2
- [x] 2. The district summary DataFrame
- [x] 3. The school summary DataFrame 
- [x] 4. The top 5 performing schools, based on the overall passing rate 
- [x] 5. The bottom 5 performing schools, based on the overall passing rate
- [x] 6. The average math score for each grade level from each school 
- [x] 7. The average reading score for each grade level from each school
- [x] 8. The scores by school spending per student 
- [x] 9. The scores by school size
- [x] 10. The scores by school type

Deliverable 3
- [x] 11. Analyze the updated data

Jupyter Notebook with updated analysis: [School District Analysis](https://github.com/GabrielaTuma/Panda_analysis/blob/8e97f44600a3eb1e01055bb7e979debdb63c61a8/School_District_Analysis/PyCitySchools_Challenge.ipynb)

## Resources 

- Data Source (by School): [schools_complete.csv](https://github.com/GabrielaTuma/Panda_analysis/blob/8e97f44600a3eb1e01055bb7e979debdb63c61a8/School_District_Analysis/Resources/schools_complete.csv)
- Data Source (by Student): [students_complete.csv](https://github.com/GabrielaTuma/Panda_analysis/blob/8e97f44600a3eb1e01055bb7e979debdb63c61a8/School_District_Analysis/Resources/students_complete.csv)
- Software: Python 3.7.6, Visual Studio Code 1.58.1, Jupyter Notebook 6.3.0

## Summary 

### The district summary DataFrame

Updated district summary 
![District Summary](https://github.com/GabrielaTuma/Panda_analysis/blob/c98a28f83b6b9dcd78f25c01d152c2c4d29dc3ef/School_District_Analysis/Resources/District%20Summary%20DataFrame.png)

Looking at the averages and percentages with one decimal point we can notice a slight difference compared to the original file. Specially when it comes to the math results the scores of the ninth grade students from Thomas High School definitely affected the overall results. The averages and percentages are greater when all the grades are counted, which contributes with the supposition of academic dishonesty. 

Original file - all scores counted
![Original Summary](https://github.com/GabrielaTuma/Panda_analysis/blob/9359b6bdd8b0e0b2d1aba7d1def45576c089d957/School_District_Analysis/Resources/Original%20district%20summary.png%20.png)


### The school summary DataFrame 

![School Summary](https://github.com/GabrielaTuma/Panda_analysis/blob/c98a28f83b6b9dcd78f25c01d152c2c4d29dc3ef/School_District_Analysis/Resources/School%20Summary%20DataFrame.png)

Looking at the Thomas High School row we can observe that the average for math and reading don't ready add up with the passing percentages. The logical sequences to calculate average don't count NaN values, but the percentages depend on the student count number to be calculated, which means that the results for Thomas High School are misleading.  

The percentages for Thomas High School are recalculated and a new DataFrame is generated:

![Adjusted Summary](https://github.com/GabrielaTuma/Panda_analysis/blob/ac5e9bd9f8f9453f0bdc64ec851757fc87bd6f6c/School_District_Analysis/Resources/School%20summary%20adjusted.png)


### The top 5 and bottom performing schools, based on the overall passing rate 

The numbers for Thomas High School are slightly different than before, but the position in the top 5 schools remains. The school is still in second place based on the overall passing rate.  

Top 5 performing schools 

![Top Schools](https://github.com/GabrielaTuma/Panda_analysis/blob/5502b8b49ef2218600224c1403e58ea1e85fa91f/School_District_Analysis/Resources/Top%20Schools.png)

Bottom 5 performing schools 

![Bottom Schools](https://github.com/GabrielaTuma/Panda_analysis/blob/5502b8b49ef2218600224c1403e58ea1e85fa91f/School_District_Analysis/Resources/Bottom%20Schools.png)


### The average math and reading score for each grade level from each school 

No difference is noted in this analysis, except the NaN values that represent the supposition of academic dishonesty.

Average math score for each grade level

![Math by grade](https://github.com/GabrielaTuma/Panda_analysis/blob/c98a28f83b6b9dcd78f25c01d152c2c4d29dc3ef/School_District_Analysis/Resources/Math%20scores%20by%20grade.png)

Average reading score for each grade level

![Reading by grade](https://github.com/GabrielaTuma/Panda_analysis/blob/c98a28f83b6b9dcd78f25c01d152c2c4d29dc3ef/School_District_Analysis/Resources/Reading%20scores%20by%20grade.png)


### The scores by school spending per student

![Score by spending](https://github.com/GabrielaTuma/Panda_analysis/blob/c98a28f83b6b9dcd78f25c01d152c2c4d29dc3ef/School_District_Analysis/Resources/Scores%20by%20spending%20per%20student.png)


### The scores by school size

![Score by size](https://github.com/GabrielaTuma/Panda_analysis/blob/c98a28f83b6b9dcd78f25c01d152c2c4d29dc3ef/School_District_Analysis/Resources/Scores%20by%20size.png)


### The scores by school type

![Score by type](https://github.com/GabrielaTuma/Panda_analysis/blob/c98a28f83b6b9dcd78f25c01d152c2c4d29dc3ef/School_District_Analysis/Resources/Scores%20by%20type.png)


When we look at the scores by school size, type and spending per student no difference is noted comparing with the original files counting the reading and math scores for the ninth grade at Thomas High School. These students represent less than 1,5% of the total, we can see slight changes in the more detailed tables, but when we categorize the data in broader groups it's hard to see the difference in the final results. 

Other conclusions can be taken by looking at these tables. Schools with high investments show poor score results, the smaller the value spent per student, the greater is the performance. Same goes to large instituions, medium and small schools have an overall passing percentage of 90%, but when it comes to large ones, this number drops to 58%. Also, Charter type schools have a notorious advatages against District type schools comparing passing percentages. 




