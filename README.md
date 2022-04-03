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


 


