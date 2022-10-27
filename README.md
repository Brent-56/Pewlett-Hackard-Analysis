# Pewlett-Hackard-Analysis

### Overview
The purpose of this project was to perform analysis on the employees. In this case we were performing the analyis to future proof the company. We wanted to know how many employees were going into retirement in the foreseeable future so we could plan accordingly. This means ramping up initiatives to hire more people so the company does not see overwhelming number of vacancies when we start to see an increase in retiring employees. Planning ahead in this case will ensure a smooth transition phase and will allow the company time to gather resources and personnel to hire and train new employees. 

### Results



![D059BC4F-5F70-4444-B4DA-80A1215EAD41](https://user-images.githubusercontent.com/112785655/198403401-db042f8f-d7e1-4e52-a962-a3df2993bbfb.jpeg)

- There seems to be a large number of employees in the retirement range. We first need to consider funding for benefits packages and recruiting initiatoves. 

- The employees that are in the retirement range appear to have high levels of experience so we need to take mentorship intitiatives seriosly so their replacements don't miss a beat. 


The code we used to determine retiring titles was 

SELECT COUNT (ut.emp_no), ut.title
INTO retiring_titles
FROM Unique_titles as ut
GROUP BY title
ORDER BY COUNT(title) DESC;
SELECT * FROM retiring_titles

We are selecting columns employee no and title from the Unique titles table and puttting it into the new table called "retiring_titles.
From there we are grouping by title and ordering by count of title wanting it listed in descending order. Select from retiring_titles is us wanting to see the table. 


![48C7F7DF-4C24-448D-8921-6817F2EAF534](https://user-images.githubusercontent.com/112785655/198412068-9cee08d8-0610-4ace-b7b3-e3d3f05488d9.jpeg)
- The good news is that there are also a high number of mentorship eligible employees. 

- We need to cease the opportunity to start the mentorship process early prior to losing experienced workers.

- The number mentorship eligible employees is simply the number. Some of the mentorship eligible employees may not stay with the company which is another reason why it would be beneficial to start early. Starting early would ensure production stays up to standard and will likely encourage employees to stay considering they are looking at taking on more responsibilities and aquiring more presigiuous positions within the company.


### Conclusion
Considering we have a high number of employees that are eligible for retirement I think it's safe to say that the company should be looking at heavy recruiting and mentorship initiatives. It would be awful to wait until employees started retiring to start mentoring and recruiting. We want the experience and to stay within the company so the work and work culture continues to be up to standard. We can't simply rely on mentorhship eligibles as all of them probably wont agree to go with the program. This is key in why we should be looking at recruiting new and experienced employees from other companies in addition to mentoring the employees that are willing to be mentored. This is confirmed through extracting the retirrment titles as finding out which areas will need replacing is the main focus.
