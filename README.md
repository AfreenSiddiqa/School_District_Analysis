# School_District_Analysis

##Deliverable 2

##Overview of the school district analysis:

students_complete.csv file shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. 
We have to replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact
Using the Pandas loc method with conditional statements and comparison and logical operators, select the ninth-grade reading and math scores for Thomas High School. Then by  using the Pandas NumPy module to change the reading and math scores to NaN.

The loc method is used to select all the reading and math scores from the ninth grade at Thomas High School. Inside the loc method, the following are completed:

A comparison operator is used to retrieve all the rows with Thomas High School in the "school_name" column of the student_data_df 
A comparison operator is used to retrieve all the rows with the ninth grade in the "grade" column of the student_data_df
Logical and comparison operators are used to retrieve all the rows with the "reading_score" column for Thomas High School ninth graders from the student_data_df
Logical and comparison operators are used to retrieve all the rows with the "math_score" column for Thomas High School ninth graders from the student_data_df
The reading and math scores for the ninth graders in Thomas High school are replaced with NaNs

![First Deliverable](https://user-images.githubusercontent.com/93686963/144766485-34c1a238-3996-4f31-9fa5-e7f9f2a63273.PNG)

![First Deliverable_2](https://user-images.githubusercontent.com/93686963/144766494-183f974c-9ed7-423e-8358-78675d234dab.PNG)



Deliverable 2

The District summary:
Recalculated total student count by subtracting the number of ninth-grade students in Thomas High School from the total student count, then recalulated the passing math and passing reading percentages and overall passing percentage.

How is the school summary affected?
Using the same methods from previous examples I created a data frame, including the data metrics: School Type, total studemts, total school budget, per student budget, average math score, average reading score, passing math percentage, passing reading percentage and overall passing percentage. I formatted the school budget and per student budget to include the dollar sign and set the values to show to the hundreds place. You can see the data in the following screenshot. 
you’ll execute the code from this module that creates and formats the School Summary DataFrame, then update the school summary using the 10th-12th graders from Thomas High School as follows:

First, you’ll calculate the number of 10th-12th graders in Thomas High School.
Create three new DataFrames for the 10th-12th graders from Thomas High School: students who passed math, students who passed reading, and students who passed both math and reading.
Using these DataFrames, you'll recalculate the percentage of students who passed math, passed reading, and passed both math and reading for Thomas High School only.
Finally, you'll replace the % Passing Math, % Passing Reading, and % Overall Passing scores in the current School Summary DataFrame with the new passing percentages for Thomas High School.
 using the loc method with logical and comparison operators, retrieve the student count for Thomas High School ninth graders in the school_data_complete_df DataFrame.
 subtract the number of students retrieved from Step 1 from the total student count to get the new total student count.
 calculate the math and reading passing percentages based on the new total student count.
 calculate the overall passing percentage with the new total student count.
Before moving on, confirm that that your District Summary DataFrame looks like this image:

![District Summary](https://user-images.githubusercontent.com/93686963/144766696-86176acb-ec6d-421a-ad52-05db789569a3.PNG)



The top 5 and bottom 5 performing schools, based on the overall passing rate
top_schools = per_school_summary_df.sort_values(["% Overall Passing"], ascending=False)
top_schools.head()
![top_schools](https://user-images.githubusercontent.com/93686963/144766870-ba2bc7d5-841f-4291-8051-47310fc960df.PNG)

bottom_schools = per_school_summary_df.sort_values(["% Overall Passing"], ascending=True)
bottom_schools.head()
![bottom_schools](https://user-images.githubusercontent.com/93686963/144766912-2bdb9d64-de68-4145-b0cf-2c2ec9fdb05f.PNG)



The average math score for each grade level from each school

![image](https://user-images.githubusercontent.com/93686963/144766949-b5798a4f-beed-4feb-aea4-6b3b0fe4544d.png)


The average reading score for each grade level from each school

![image](https://user-images.githubusercontent.com/93686963/144766997-74aa435d-8f82-4089-ada2-f9988a371821.png)


The scores by school spending per student, by school size, and by school type:

spending_summary_df
![image](https://user-images.githubusercontent.com/93686963/144767068-ebfd654b-e83a-4f9e-92e4-8cb8b3da2e70.png)

size_summary_df
![image](https://user-images.githubusercontent.com/93686963/144767109-15360b01-eddf-450b-acca-eb628d7bec5f.png)

type_summary_df
![image](https://user-images.githubusercontent.com/93686963/144767123-7e57581a-ee4b-43fa-aee7-02f5d67c7346.png)


