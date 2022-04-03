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




 


