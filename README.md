# School_District_Analysis
## Summary
- School data along with student data was provided to make an analysis of the school districts.
- Data provided on school file included school name, type, size and budget.
- Data provided on student file included student name, gender, grade, school name, reading and math scores.
- The analysis requires to get a school summary after merging the files provided.

## Analysis
- 1. Use pandas dependency. 
- 2. Verify the data does not contain blank spaces or NaN values.
- 3. Remove prefixes and suffixes from student names.
- 4. Merge the school data with student data.
- 5. Provide the following summaries:
    - Distric Summary (Includes passing math and reading scores >= 70).
    - Bottom and Top schools (sorting by %Overall Passing).
    - Reading scores by grade.
    - Math scores by grade.
    - Spending summary (Provide average of the math and reading scores and %passing by spending ranges per student).
    - Size summary (Provide average of the math and reading scores and %passing by school size ranges(number of students per school)).
    - School Summary (contains the average of the data by school name).
    - Type Summary (Provide average of the math and reading scores and %passing by school type).
    
## Files for Module Exercise:
- PyCitySchools.ipynb (jupyter notebook)
- Resources (folder with files for the module exercise and challenge)
- output_org_code (folder for results)
    
# Challenge Module 4
## Goals
- Replace the ninth-grade math and reading scores from Thomas High School with NaN and keep intact the rest of the data. 
    - Using loc, the reading and math scores for Thomas HS for 9th graders were replaced by NaN.  See Jupyter Notebook file: PyCitySchools Challenge.ipyn
- Explain how the analysis changes.

## Analysis
- How is the district summary affected?
    - The Distric Summary was made from the 39,170 students and displays the average of the data for the total of the students.  The data from ninth-grade math and reading scores from Thomas High School that has changed was for 461 students.  461 students is 1,18% of the total students (39,170).  On the table below the percentages only are changing 1% on the %passing for math and reading and %overall passing columns.  
    ![District Summary Table](https://github.com/DahianaMC/School_District_Analysis/blob/master/School_District_Analysis_Summary_Tables/District%20Summary%20Table.png)

- How is the school summary affected?
    - The School Summary was affected only for Thomas High School and has a high impact on the % passing math and reading and % overall passing, because the calculations are made counting how many students have math and reading scores higher than 70, then is divided by the total of students per school.  The total of students per school is calculated counting the student name per school and does not reflect the data that is NaN in reading and math scores.
    ![School Summary Table](https://github.com/DahianaMC/School_District_Analysis/blob/master/School_District_Analysis_Summary_Tables/School%20Summary%20Table.png)

- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance, relative to the other schools?
    - The performance of the Thomas High School was seriously affected by replacing the reading and math scores from the 9th graders for NaN becuase the way the calculation is made in the code.  The school went from the 2nd place for the Charter type to the last one.
    ![Top and Bottom Schools Table](https://github.com/DahianaMC/School_District_Analysis/blob/master/School_District_Analysis_Summary_Tables/Top%20and%20Bottom%20Schools%20Table.png)

- How does replacing the ninth-grade scores affect the following?
    - Math and Reading Scores by Grade:
        - The math and reading scores are only NaN values now for Thomas HS for 9th graders.  The summary tables show the actual (challenge) values for Thomas HS, 9th graders are NaN values, the rest of the graders and schools keep the original scores:
    ![Math Scores for 9th graders](https://github.com/DahianaMC/School_District_Analysis/blob/master/School_District_Analysis_Summary_Tables/Math%20Scores%20for%209th%20graders.png)
    ![Reading Scores for 9th graders](https://github.com/DahianaMC/School_District_Analysis/blob/master/School_District_Analysis_Summary_Tables/Reading%20Scores%20for%209th%20graders.png)
    
    - Scores by School Spending:
        - Looking the School Summary table, the spending range for Thomas High School was $630-644.  The spending summary table shows the %Passing for math and reading and %Overall passing are decreasing, because the issue with the calculation to get the % passing for math and reading scores.
    ![Spending Summary Table](https://github.com/DahianaMC/School_District_Analysis/blob/master/School_District_Analysis_Summary_Tables/Spending%20Summary%20Table.png)
    
    - Scores by School Size:
        - Looking the School Summary table, the school size for Thomas HS was Medium (1000-2000).  The size summary table shows the %Passing for math and reading and %Overall passing are decreasing as well.
    ![Size Summary Table](https://github.com/DahianaMC/School_District_Analysis/blob/master/School_District_Analysis_Summary_Tables/Size%20Summary%20Table.png)
    
    - Scores by School Type:
        - Since the Thomas HS was a Charter school type, the %Passing for math and reading and %Overall passing are decreasing for Charter school type on Type Summary table.
    ![Type Summary Table](https://github.com/DahianaMC/School_District_Analysis/blob/master/School_District_Analysis_Summary_Tables/Type%20Summary%20Table.png)
    
- In general make the reading and math scores NaN for the Thomas HS, 9th graders, affects the calculations for %Passing math and reading scores and the %Overall Passing, becuase the %passing for math and reading are computed counting the reading or math scores higher than 70, then divide it by the total students per school, the issue with the formula is the total students per school is calculated counting the student names and does not reflect the scores that are NaN.

## Files for Challenge:
- PyCitySchools Challenge.ipynb (jupyter notebook)
- Resources (folder with files for the module exercise and challenge)
- output (folder for challenge results)
- School_District_Analysis_Summary_Tables (Folder with summary tables)
