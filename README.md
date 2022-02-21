# SQL_Analysis_Challenge
Employee Database with SQL ( Pewlett_Hackard_Analysis )



## Overview: 

After reviewing the employee files, an entity relationship diagram was created using quick database diagrams to gather and organize the key elements from various data tables.  
The data was imported using postgres and the pgAdmin interface.  SQL queries were written to create data tables by joining primary keys from different data sets together and establishing foreign keys. The leadership is concerned about a "silver tsunami," where there is a mass exodus of retiring employees creating a massive amount of job vacancies.  SQL queries were created to generate a list of retiring employees by title and a list of employees eligible for mentorship.    


## Results: 

1. With the first review of creating a list of potential "silver tsunamis," the query resulted in many duplicates due having multiple positions.
![Pic 1](https://github.com/josepcherian/SQL_Analysis_Challenge/blob/main/Challenge_Documents/duplicates_titles_pic.PNG)

2. Using the 'distinct on' SQL script, the duplicates were removed leaving the most recent job title to create a unique list of retiring employees.  

![Pic 2](https://github.com/josepcherian/SQL_Analysis_Challenge/blob/main/Challenge_Documents/unique_titles_pic.PNG)

3. Retiring Counts by Title for a total of 90,398 potential retirees.  
![Pic 3](https://github.com/josepcherian/SQL_Analysis_Challenge/blob/main/Challenge_Documents/Retiring_count_titles.PNG) 


4. Mentor Eligibility List of 1549 employees born in 1965.
![Pic 4](https://github.com/josepcherian/SQL_Analysis_Challenge/blob/main/Challenge_Documents/mentor_list.PNG)

## Summary: 

### 1. The "silver tsunami" will have a significant impact of leaving 90,398 vacancies.   

### 2. Using the criteria of those born in 1965, the potential mentee list is 1,549 employees. The gap between approximately 90,000 mentors and 1,500 mentees is significant.  



## Future Area of Focus:
Creating a new query to further investigate the gap, the two charts below compare the counts by titles of the retiring and mentor eligible employees.  There is a reasonable ratio of titles between the two tables implying that matching mentor to mentee is scalable under the right criteria.  However, it is concerning that no managers met the mentor eligibility requirement.  Further discussion is need to fill the manager gap.  
![Pic 5](https://github.com/josepcherian/SQL_Analysis_Challenge/blob/main/Challenge_Documents/Retiring_count_titles.PNG) ![Pic 6](https://github.com/josepcherian/SQL_Analysis_Challenge/blob/main/Challenge_Documents/mentee_counts.PNG)

To move forward with the approximately 1,500 potential mentee list as a pilot mentoring program, the list of more than 90,000 retiring employees was narrowed to close the gap of matching mentor to mentee.  The potential mentor list was narrowed by setting the criteria for being around age 35 when they started their current job title resulting in 5,521 employees that could be matched with the 1,549 mentees, which significantly narrows the mentor-mentee gap.

![Pic 7](https://github.com/josepcherian/SQL_Analysis_Challenge/blob/main/Challenge_Documents/narrow_retiring_mentor_list.PNG)
![Pic 8](https://github.com/josepcherian/SQL_Analysis_Challenge/blob/main/Challenge_Documents/mentee_counts.PNG)

Lessons from creating a mentoring pilot program with the 1,549 mentees can be studied and then expanded to more potential mentees when a new list is generated by expanding the date criteria.
