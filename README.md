# ****School_District_Analysis****

## Overview of Project
- To see how the different districts/schools/students fared in relation to their student grades, funding, size, and school type. Using the student and school dataset that has already been combed through and Jupyter notebook, results were created for the analysis of the school district.  
- The school board has notified that the students_complete.csv file shows evidence of academic dishonesty; specifically, **reading and math grades for Thomas High School ninth graders** appear to have been altered. Although the school board does not know the full extent of the academic dishonesty, they want to uphold state-testing standards.
  -  To replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. 
  -  Once the math and reading scores have been replaces, the school district analysis was repeated leading to this written report.
-----------------

## Results: 
- How is the district summary affected?
  - The district summary is faintly effected from the lower scores, and  overall passing percentage from removing the Thomas High School 9th grade data.

![image](https://user-images.githubusercontent.com/106709942/177456071-e2319a5a-9b11-4345-b15d-5ae824bf6f73.png)   

![image](https://user-images.githubusercontent.com/106709942/177456139-1acf99d3-6db7-4c48-8860-c46876edec58.png)


- How is the school summary affected?
  - The school summary was effected by one data point which is Thomas High School. As seen below, Thomas High School original (altered) passing math %, passing reading %, and overall passing % is significantly higher than the nulled data school summary.

![image](https://user-images.githubusercontent.com/106709942/177457506-f0e62ec2-d904-4fe0-887e-b727d4e8f3d7.png)

![image](https://user-images.githubusercontent.com/106709942/177457425-cc985cce-8343-4837-9415-15a8eb0f081c.png)

- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
  - Replacing the ninth graders math and reading score had minimal affect relatative to the other schools. Thomas High school was ranked second in the original data set, and still second after removing the ninth graders' score. 

![image](https://user-images.githubusercontent.com/106709942/177467257-e493f337-9856-43bb-a108-f493f9eb59d8.png)


- How does replacing the ninth-grade scores affect the following:
  - Math and reading scores by grade
    - By replacing the ninth-grade data to Nans, it is seen immediately in the tables below.
    - By replacing that, the score affected was minimal. 
    - Student_count() Before Tomas High School Cleanup was: 1635
    - Student_count() After Tomas High School Cleanup was: 1174
    
  
![image](https://user-images.githubusercontent.com/106709942/177461930-8049d843-4cb3-45bd-bd3a-11437cfac952.png)    ![image](https://user-images.githubusercontent.com/106709942/177462422-abd1d53d-f8a2-4d34-9c84-7a5eb93097d7.png)


![image](https://user-images.githubusercontent.com/106709942/177462003-c9c12897-7141-4ffb-a894-0a271338975a.png)   ![image](https://user-images.githubusercontent.com/106709942/177462753-29034d3f-6933-498b-bd97-3d9ebd634b13.png)

  - Scores by school spending
    -  Removing 9th grade Students and their grades from Thomas High School data reduces the "% Passing Math", "% Passing Reading" and "% Overall Passing" scores for spending bucket "$631-645".
    - The difference seen here before formatting for scores by school spending is fractional. After the formatting the scores are the same value. 
  
  ![image](https://user-images.githubusercontent.com/106709942/177464750-9f571fe6-906e-4836-ac29-e6d0502d9e0c.png)
  
  ![image](https://user-images.githubusercontent.com/106709942/177464840-3373829e-c6ce-4222-8f98-c60aaacd11db.png)

  - Scores by school size
    - Removing 9th grade Students and their grades from Thomas High School data reduces the "% Passing Math", "% Passing Reading" and "% Overall Passing" scores for school size.
    - The difference in score by school size is so minimal, that after formatting both origianl and replaced data provide the same output seen below: 

![image](https://user-images.githubusercontent.com/106709942/177465733-5c3bcae0-fdcf-4e18-98ef-0de2fbc673e1.png)

  - Scores by school type
    - The difference in score by school school is so minimal, that after formatting both origianl and replaced data provide the same output seen below: 

![image](https://user-images.githubusercontent.com/106709942/177466522-4f714f6a-fbde-4e38-aa6e-1d949d4c09d5.png)

----------------


## Summary:
- The district had very little impact when removing the ninth graders from the over 39,000 pool of students. 
- Thomas High School remain to be the second best performing school with the ninth graders in the data or with them not included. This indicating that Thomas High School students remain top performers in comparison to the other schools. 
- In the original data set including the  ninth  graders, the overall passing percentage was 91%, and after excluding the ninth graders, the overall passing percentage was 65%. However, After calculating the overall percentage of 10th-12th grade students passing read from Thomas High School, the percentage jumped back to 90.6%. 
- Changes to scores by School and size where less than 1%. 
- Overall, the changes of removing the ninth graders was minimal to most school district analysis excluding the school summary analysis when using NaNs. 
