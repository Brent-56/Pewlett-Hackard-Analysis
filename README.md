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
