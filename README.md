# School_District_Analysis

## PROJECT BACKGROUND
The Chief Data Scientist for the PyCity School District has requested assistance with analyzing student standardized test scores and student funding for the PyCity High school District. Due to a recent discovery of potential alteration to the reading and math score for Thomas High School, the district has requested change to the "PyCitySchool" project we've previously created for the district. 

In the "PyCitySchools" project we leveraged python programming, utilizing the python library "panda' along with the Jupyter notebook to read raw data from the CVS file and transform the data into a format that can easily be utilized to create reports for school district officials. 

## PURPOSE: 
The purpose of this '"PyCitySchool Challenge" project is to documents the refracting process of the original code from "PyCitySchool". We will use the Pandas Numpy module to replace Thomas High School's reading and math score with NaN. 

## GOAL
After replacing Thomas high Schools' reading and math scores, a new analysis will be performed based on those changes. The changes will provide the school district with new insight into the following metrics 

- District summary 
- School summary
- Top 5 performing schools, based on the overall passing rate 
- Bottom 5 performing schools, based on the overall passing rate 
- Average math score for each grade level from each school 
- Average reading score for each grade level from each school 
- Scores by school spending per student 
- Scores by school size 
- Scores by school type 

#### DELIVERABLES 
1. Replace ninth-grade reading and math scores
2. Repeat the school district analysis
3. School district analysis report

## RESOURCES

## LOGICAL WORKFLOW

**Step 1. Get the number of students that are in ninth grade at Thomas High School. These students have no grades. 

 **Get the total student count** 
student_count = school_data_complete_df["Student ID"].count()

**Step 2. Subtract the number of students that are in ninth grade at Thomas High School from the total student count to get the new total student count.**

**Step 3. Calculate the passing percentages with the new total student count.

**Calculate the students who passed both reading and math.**
passing_math_reading = school_data_complete_df[(school_data_complete_df["math_score"] >= 70)
                                               & (school_data_complete_df["reading_score"] >= 70)]
**Calculate the number of students that passed both reading and math.**
overall_passing_math_reading_count = passing_math_reading["student_name"].count()

**Step 4.Calculate the overall passing percentage with new total student count.**

**Step 5.  Get the number of 10th-12th graders from Thomas High School (THS).**
**Step 6. Get all the students passing math from THS**
**Step 7. Get all the students passing reading from THS**
**Step 8. Get all the students passing math and reading from THS**
**Step 9. Calculate the # Step 10. Calculate the percentage of 10th-12th grade students passing reading from Thomas High School. of 10th-12th grade students passing math from Thomas High School.** 
**Step 11. Calculate the overall passing percentage of 10th-12th grade from Thomas High School.**
**Step 12. Replace the passing math percent for Thomas High School in the per_school_summary_df.**
**Step 13. Replace the passing reading percentage for Thomas High School in the per_school_summary_df.**
**Step 14. Replace the overall passing percentage for Thomas High School in the per_school_summary_df.**

##### High and Low Performing Schools ** # per_school_summary_df
**Sort and show top five schools.**
**Sort and show top five schools.**

#### Math and Reading Scores by Grad
**Create a Series of scores by grade levels using conditionals.
**Group each school Series by the school name for the average math score.
**Group each school Series by the school name for the average reading score.


#### Math and Reading Scores by Grade
**Combine each Series for average math scores by school into single data frame.**
**Combine each Series for average reading scores by school into single data frame.**
**Format each grade column.**
**Remove the index.**
**Display the data frame**
**Remove the index.**


#### Scores by School Spending
**Establish the spending bins and group names.**
**Categorize spending based on the bins.**
**Calculate averages for the desired columns.** 
**Create the DataFrame**

#### Scores by School Size
**Establish the bins.**
**Categorize spending based on the bins.**
**Calculate averages for the desired columns.** 
**Assemble into DataFrame.** 

#### Scores by School Type
**Calculate averages for the desired columns.** 
**Assemble into DataFrame.**
**Format the DataFrame # Format the DataFrame**  
**Format the DataFrame** 
**Display the data frame**
