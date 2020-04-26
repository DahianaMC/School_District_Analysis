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
- How is the school summary affected?
    - The School Summary was affected only for Thomas High School and has a high impact on the % passing math and reading and % overall passing.  Looks like the ninth grades were having scores higher than 70% from the original data.

    

