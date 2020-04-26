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
    
## Challenge Module 4
## Goals
- Replace the ninth-grade math and reading scores from Thomas High School with NaN and keep intact the rest of the data. 
- Explain how the analysis changes.

## Analysis
- How is the district summary affected?
    - The Distric Summary was made from the 39,170 students and it is displayed for total of the students.  The data from ninth-grade math and reading scores from Thomas High School that has changed was for 461 students.  The percentage of the students that has changed was 461/39,170x100=1.18%.  With this in mind the impact on the District summary was low.  On the table below the percentages only are changing 1% on the %passing for math and reading and %overall passing.  
    ![District Summary Table](https://github.com/DahianaMC/School_District_Analysis/blob/master/School_District_Analysis_Summary_Tables/District%20Summary%20Table.png)

- How is the school summary affected?
    - The School Summary was affected only for Thomas High School and has a high impact on the % passing math and reading and % overall passing.  Looks like the ninth graders were having reading and math scores higher than 70% from the original data.
    ![School Summary Table](https://github.com/DahianaMC/School_District_Analysis/blob/master/School_District_Analysis_Summary_Tables/School%20Summary%20Table.png)

- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance, relative to the other schools?
    - The performance of the Thomas High School was seriously affected by loosing the reading and math scores from the 9th graders.  The school went from the 2nd place for the Charter type to the last one.
    ![Top and Bottom Schools Table](https://github.com/DahianaMC/School_District_Analysis/blob/master/School_District_Analysis_Summary_Tables/Top%20and%20Bottom%20Schools%20Table.png)

- How does replacing the ninth-grade scores affect the following?
    - Math and Reading Scores by Grade:
        - The math are reading scores changed on the data, were the ones for Thomas High School for 9th graders.  The math and reading scores are only NaN values now.  The summary tables show the actual (challenge) values for Thomas HS, 9th graders are only NaN values:
    ![Math Scores for 9th graders](https://github.com/DahianaMC/School_District_Analysis/blob/master/School_District_Analysis_Summary_Tables/Math%20Scores%20for%209th%20graders.png)
    ![Reading Scores for 9th graders](https://github.com/DahianaMC/School_District_Analysis/blob/master/School_District_Analysis_Summary_Tables/Reading%20Scores%20for%209th%20graders.png)
    
    - Scores by School Spending:
        - Looking the School Summary table, the spending range for Thomas High School was $630-644.  The spending summary table shows the %Passing for math and reading and %Overall passing are decreasing, confirming a good number of values for math and reading for Thomas HS for 9th graders for the original data were higher than 70%.
    ![Spending Summary Table](https://github.com/DahianaMC/School_District_Analysis/blob/master/School_District_Analysis_Summary_Tables/Spending%20Summary%20Table.png)
    
    - Scores by School Size:
        - Looking the School Summary table, the school size for Thomas HS was Medium (1000-2000).  The size summary table shows the %Passing for math and reading and %Overall passing are decreasing.
    ![Size Summary Table](https://github.com/DahianaMC/School_District_Analysis/blob/master/School_District_Analysis_Summary_Tables/Size%20Summary%20Table.png)
    
    - Scores by School Type:
        - Since the Thomas HS was a Charter school type, the %Passing for math and reading and %Overall passing are decreasing for Charter school type on Type Summary table.
    ![Type Summary Table](https://github.com/DahianaMC/School_District_Analysis/blob/master/School_District_Analysis_Summary_Tables/Type%20Summary%20Table.png)
    

