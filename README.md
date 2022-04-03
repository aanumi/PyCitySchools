# WRITTEN ANALYSIS - PYCITYSCHOOLS

## OVERVIEW OF ANALYSIS
The school board has identified key issues relating to academic dishonesty regarding the reading and math grades for Thomas High School. The purpose of this analysis is to help the school board uphold state testing standards by replacing the inconsistent datasets for the 9th Grade Thomas High School with NaNs, keeping the unaffected data intact, and re-conducting the school district analysis with updated data.


## ANALYSIS RESULTS

### How is the district summary affected?
•	When the 9th grade scores for math and reading for students at Thomas High School are removed, the total number of schools, students and budget stay the same. The percentages passing math, reading and passing overall are however reduced as a result of replacing a portion of the data with NaNs. The changes however are not too substantial as both the old and new analysis may likely round to the same whole numbers. An image of the updated adjusted analysis is seen below:
<img width="881" alt="Screen Shot 2022-04-03 at 9 28 56 AM" src="https://user-images.githubusercontent.com/100884241/161430451-45b64376-b9fc-487f-90dc-e5d8946c2b9a.png">

### How is the school summary affected?
•	While the total students, total school budget, and per student budget data remain the same, the average math score, average reading score, % passing math, % passing reading, and % overall passing reduce as a result of replacing some scores with NaNs. A significant impact is the reduction in the original analysis % overall passing from 90.9% to 65.07% in the re-computed analysis. The reason for this significant reduction is the replacement of math and reading scores with NaNs while using the same overall total denominator of students. The school summary data frame also changes only in regard to Thomas High School. An image of the updated analysis showing the reduced passing math, reading, and overall scores is seen below:
![School_summary affected](https://user-images.githubusercontent.com/100884241/161430668-d2c6d7c9-ebef-4acc-aafd-06f56ba17494.png)

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to other schools?
•	In the original analysis, Thomas High School ranked in the top 5 schools by overall passing % relative to other schools. When the incorrect 9th grade scores are removed and replaced with NaNs in the dataset, Thomas High School falls below to the 8th position, with a % overall passing score of 65.07. This approximate reduction of about 30 is anticipated as a portion of the data has been removed and replaced with NaNs. Of course, this doesn’t represent the most accurate picture of events as the corrupted scores weren’t replaced with similar averaged numbers, but replaced with NaNs instead. Replacing the corrupt scores with other metrics (averages or interpolations) may be helpful in ranking and evaluating Thomas High School’s (as accurate as possible) performance. An updated snapshot of Thomas High School’s position relative to other schools is seen below:
 <img width="1090" alt="Screen Shot 2022-04-03 at 9 40 41 AM" src="https://user-images.githubusercontent.com/100884241/161430831-d19ff105-844b-499a-89ee-675b39010a5d.png">

### How does replacing the ninth grade scores affect Math and Reading scores by grade?
•	The math and reading scores by grade for all other schools are not affected when the 9th grade Thomas High School scores are removed. Having replaced the Thomas High School 9th grade scores with null values, we see ‘nan’ in the 9th grade columns for Math and Reading Scores. Snapshots of new math and reading scores showing the ‘nan’ after the replacement can be seen below:
 ![New math scores by grade](https://user-images.githubusercontent.com/100884241/161430883-95a79372-c359-452c-821f-f2434c2a29e5.png) ![New reading scores by grade](https://user-images.githubusercontent.com/100884241/161430892-2e471278-1a15-443d-b10f-7d3831cc832f.png)
 
 ### How does replacing the ninth-grade scores affect scores by school spending?
•	The only affected bin as anticipated is the bin containing Thomas High School. The spending range for Thomas High School is $638, so Thomas High School falls in the $630 - $644 bin. While the average math and reading scores remain the same, the % passing math, reading, and overall are reduced since a portion of the dataset is replaced with NaNs, while the overall denominator with the pool of all students stays the same. The new percentages are 73.46 for Math, 84.32 for reading, and 62.47 overall. A snapshot of the replaced scores can be seen below:

![Affected by school spending](https://user-images.githubusercontent.com/100884241/161431007-0ea8a6bb-6d2a-4b63-9bae-8ff8e8fe096e.png)

 ### How does replacing the ninth-grade scores affect scores by school size?
•	Since Thomas High School has 1635 students, it falls in the medium school size. Due to the replacement of the affected scores with the NaNs, the % passing math, reading, and overall are decreased from (Math) 93.6 to 93.58, (Reading) 96.79 to 96.73, and (Overall 90.62 to 90.56). An image of the adjusted analysis impacting school size is pasted below:
![Affected by school size](https://user-images.githubusercontent.com/100884241/161431052-0dbe9b29-8d8b-4d6e-ae65-1b6216f7c1eb.png)

 ### How does replacing the ninth-grade scores affect scores by school type?
•	Thomas High School is categorized as a Charter school. This means that the numbers for the other school type (District) are unaffected as the change affects Charter schools after adjusting the analysis. While average math and reading scores stay the same between both school types, the percentages reduce in the charter schools  from 94 to 90 (% passing match), 97 to 93 (% passing reading), and 90 to 87 (% overall passing). This is roughly a 4 point decrease in the first two items, with a 3 point drop in the overall. An image of the adjusted analysis impacting school type (Charter schools) is pasted below:
![Affected by school type](https://user-images.githubusercontent.com/100884241/161431085-60d1f8a7-af4e-41ba-84c8-fe3f41fec4f4.png)


## SUMMARY
Four key changes noted in the updated school district analysis after reading and math scores for the ninth grade students at Thomas High School were replaced with NaNs are discussed below:

1.	Using NaNs to replace incorrect data is a good way to resolve inconsistencies without skewing the results to a large extent. Using zeroes for example, in place of the NaNs would likely skew the data to a larger extent as zero is numeric and could have a bigger impact.
	
2.	Even after replacing the inconsistent data with NaNs, the performance of Charter schools is still considerably stronger than that of District schools. The replacement of Thomas High School (Charter) 9th grade scores was not significant enough to change the dynamic and highlight district schools as performing better.
	
3.	A significant reduction is noticed in Thomas High School’s overall metrics as replacing the tampered data reduced its overall from 90.9% to 65.07% in the re-computed analysis.
	
4.	The changes that occurred in the scores by school size category are minimal, as they decreased by less than 0.1% in all cases. This did not significantly affect schools in the overall medium size category.
 


