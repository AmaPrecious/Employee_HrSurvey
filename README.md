# Employee-Hr Survey Analysis

![](https://github.com/AmaPrecious/Employee_HrSurvey/blob/main/IMG_1550.JPG)

## Overview

The Employee Survey Responses dataset offers a comprehensive view of employee engagement within Pierce County, WA. With 14,725 records and 10 fields, this dataset provides valuable insights into the perceptions, experiences, and sentiments of government employees. By analyzing this data, organizations can gain a deeper understanding of factors influencing employee satisfaction, morale, and overall engagement in the workplace. This dataset serves as a foundational resource for strategic planning, human resource management, and organizational development initiatives aimed at enhancing employee well-being and organizational performance.

## Problem Statement

### Question 1.
Which survey questions did respondents agree with or disagree with most?

### Question 2.
Do you see any patterns or trends by department or role?

### Question 3.
As an employer, what steps might you take to improve employee satisfaction based on the survey results?

**Data Source** [Click here](https://github.com/AmaPrecious/Employee_HrSurvey/blob/main/Employee%20Survey%20-%20HR%20Survey%20Reponses.csv)

## Analysis Process

1. *Data Preparation:*
   - Utilized Excel and Power BI for data preparation, leveraging their functionalities for cleaning, transforming, and structuring the raw data.
   - Employed Excel for initial data cleaning tasks such as removing duplicates, filtering inaccurate entries, and handling missing values.
   - Transitioned to Power BI for more advanced data manipulation tasks, including DAX calculations, grouping, and creating new measures.
   - Ensured data consistency, and addressed any discrepancies or inconsistencies in the dataset.

2. *DAX Calculations:*
   - Utilized DAX (Data Analysis Expressions) in Power BI to perform complex calculations and derive meaningful insights from the data.
   - Created DAX measures to calculate aggregate metrics such as total revenue, average ratings, and satisfaction scores.
   - Applied DAX functions to group, filter, and aggregate data based on specific criteria, enabling deeper analysis and exploration of the dataset.
  
   Agree Count = CALCULATE(
                           COUNTROWS(FILTER('Employee Survey - HR Survey Reponses',
                            'Employee Survey - HR Survey Reponses'[Response Text]="Agree"
                              || 'Employee Survey - HR Survey Reponses'[Response Text]= "strongly agree")))


 Disagree Count = CALCULATE(COUNTROWS ( 
                     FILTER('Employee Survey - HR Survey Reponses', 
                     'Employee Survey - HR Survey Reponses'[Response Text]="Disagree" 
                     || 'Employee Survey - HR Survey Reponses'[Response Text]= "Strongly disagree")))

![image](https://github.com/AmaPrecious/Employee_HrSurvey/assets/155967136/7f096f02-245a-4330-89e4-6399d403f368)
   
3. *Grouping and Aggregation:*
   - Grouped data based on relevant attributes 
   - Aggregated data to calculate summary statistics
   - Employed grouping and aggregation techniques to summarize large datasets and extract key insights without losing important details.

4. *Adding New Measures and Slicers:*
   - Added new measures using DAX to calculate additional metrics or performance indicators not present in the original dataset.
   - Created slicers to enable interactive filtering and exploration of the data, allowing users to dynamically analyze different subsets of the dataset based on specific criteria.
   - Enhanced the analytical capabilities of the Power BI dashboard by incorporating slicers for variables such as time periods, product categories, or customer segments.

By following this analysis process, I was able to leverage Excel and Power BI effectively to prepare, analyze, and visualize the dataset, extracting valuable insights to inform decision-making and drive actionable outcomes.

## Visualization 

![](https://github.com/AmaPrecious/Employee_HrSurvey/blob/main/RESPONSE.jpg)


Insights derived from the employee engagement survey analysis:

1. *Clarity of Expectations and Recognition:*
   - The analysis reveals that a significant portion of respondents agree that they know what is expected of them at work and have received recognition or praise for their good work. This suggests that there is a level of clarity in job roles and responsibilities, and employees feel appreciated for their contributions.

2. *Feeling Valued at Work:*
   - Many respondents also agree that their supervisor or someone at work cares about them as a person, and they feel their job is important due to the organization's mission or purpose. This indicates that there is a sense of belonging and value among employees, contributing to overall job satisfaction.

3. *Areas for Improvement:*
   - Despite the positive responses, there are areas identified for improvement. Specifically, opportunities for learning and growth appear to be lacking, as indicated by lower agreement levels in this area. This suggests that there may be a need for more training programs, career development initiatives, or mentorship opportunities within the organization.
   - Additionally, respondents indicate that accountability from supervisors and inclusivity in the workplace could be enhanced. This highlights the importance of clear expectations and consistent feedback from management, as well as fostering a diverse and inclusive work environment.

4. *Discrepancies and Potential Concerns:*
   - Discrepancies between agreement and disagreement responses across various survey statements suggest potential areas of concern or focus for organizational improvement initiatives. For example, while many respondents agree that they feel valued and recognized at work, a significant portion also disagree with statements related to supervisor accountability and inclusivity. These discrepancies warrant further investigation and targeted action to address underlying issues and improve employee satisfaction and engagement.

Overall, the insights derived from the analysis provide valuable information for the organization to identify strengths, address weaknesses, and implement strategies to enhance employee engagement and satisfaction in the workplace.


![](https://github.com/AmaPrecious/Employee_HrSurvey/blob/main/DEPARTMENTAL%20TRENDS.jpg)

Question 1: "I know what is expected of me at work"
- Directors: 12 agree
- Managers: 76 agree
- Staff: 106 agree
- Supervisors: 158 agree

Question 2: "At work, I have the opportunity to do what I do best every day"
- Directors: 13 agree
- Managers: 86 agree
- Staff: 97 agree
- Supervisors: 143 agree

Question 3: "In the last seven days, I have received recognition or praise for doing good work"
- Directors: 10 agree
- Managers: 76 agree
- Staff: 74 agree
- Supervisors: 199 agree

Question 4: "My supervisor holds employees accountable for performance"
- Directors: 12 agree
- Managers: 84 agree
- Staff: 103 agree
- Supervisors: 146 agree

Question 5: "The mission or purpose of our organization makes me feel my job is important"
- Directors: 15 agree
- Managers: 95 agree
- Staff: 94 agree
- Supervisors: 142 agree

Question 6: "I have a best friend at work"
- Directors: 6 agree
- Managers: 45 agree
- Staff: 45 agree
- Supervisors: 80 agree

Question 7: "This last year, I have had opportunities at work to learn and grow"
- Directors: 6 agree
- Managers: 30 agree
- Staff: 26 agree
- Supervisors: 39 agree

Question 8: "My department is inclusive and demonstrates support of a diverse workforce"
- Directors: 13 agree
- Managers: 90 agree
- Staff: 90 agree
- Supervisors: 137 agree

Question 9: "My supervisor, or someone at work, seems to care about me as a person"
- Directors: 13 agree
- Managers: 95 agree
- Staff: 104 agree
- Supervisors: 147 agree

Question 10: "Overall I am satisfied with my job"
- Directors: 11 agree
- Managers: 89 agree
- Staff: 95 agree
- Supervisors: 132 agree

These responses provide valuable insights into employee perceptions and satisfaction levels across different organizational roles.


[click here](https://github.com/AmaPrecious/Employee_HrSurvey/blob/main/EMPLOYEE%20HR%20SURVEY%20DASHBOARD.pbix) for the interactive dashboard.

## Conclusion and Recommendation

Based on the survey results, it's evident that there are areas where employee satisfaction is strong, such as clarity of expectations, feeling valued at work, and recognition for good work. However, there are also areas for improvement, including opportunities for learning and growth, accountability from supervisors, and inclusivity in the workplace. Discrepancies between agreement and disagreement responses highlight potential areas of concern or focus for organizational improvement initiatives.

## Recommendations:
1. Implement Training and Development Programs: Offer regular training sessions and professional development opportunities to employees to enhance their skills and knowledge, fostering a culture of continuous learning and growth.

2. Enhance Supervisor Accountability: Provide supervisors with additional training on performance management and accountability to ensure consistent and fair treatment of employees. Encourage regular feedback and performance reviews to recognize achievements and address areas for improvement.

3. Foster Inclusivity and Diversity: Develop initiatives to promote inclusivity and diversity within the organization, such as employee resource groups, diversity training, and mentorship programs. Create a welcoming and supportive environment where all employees feel valued and respected.

4. Strengthen Communication Channels: Establish open and transparent communication channels between management and employees to address concerns, solicit feedback, and keep employees informed about organizational goals and initiatives. Encourage regular dialogue and collaboration to build trust and engagement.

5. Recognize and Reward Employee Contributions: Implement a formal recognition and reward program to acknowledge employees' contributions and achievements. Celebrate milestones, accomplishments, and outstanding performance to boost morale and motivation.

6. Conduct Regular Employee Surveys: Continuously assess employee satisfaction and engagement through regular surveys and feedback mechanisms. Use the insights gained to identify trends, address issues, and make data-driven decisions to improve the workplace environment.

By taking proactive steps to address areas of improvement identified in the survey results, employers can enhance employee satisfaction, engagement, and overall organizational success.
