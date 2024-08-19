# HR-Analytics-Dashboard-using-PowerBi

Attrition Analysis with Power BI .This project analyzes employee attrition using Power BI. 
It includes a data model, interactive reports, and visualizations to explore factors contributing to employee turnover. The analysis helps identify key drivers of attrition, enabling data-driven decision-making for workforce management.

# Features:

1) Comprehensive data model for employee data.
2) Interactive dashboards and reports.
3) Insights into attrition trends, demographics, and other factors.
   
# Steps:
1) Download the data from kaggle.com
   
2) Load the data in power bi and start data cleaning .
a) Start with checking of Null values .
![Screenshot (75)](https://github.com/user-attachments/assets/7e5c0fd5-a846-4f46-b777-f58a7d721bcd)
We can use Group by on employ Id and then use Count to check further .
We may select the null values by clinking on column name then we can remove them under remove rows option .

b) The values in column BusinessTravel have an error of treating Travel Rarely and Travel_Rarely as different .So we need to replace Travel Rarely as Travel_Rarely using Replace option .
![Screenshot (77)](https://github.com/user-attachments/assets/e1899c6e-d32e-4c6c-8db2-6007596099b9)

3)Use ![Background image](https://github.com/user-attachments/assets/242b0a63-0b22-49d6-9b00-58a6e6eb1a3f) as a background image.

4) Start building the dashboard starting from count of employee using cards .We also created a slicer for 3 departments i.e. HR, Research and Sales
   ![Screenshot (80)](https://github.com/user-attachments/assets/7a578fc6-baea-4ec1-9503-761983a50d77)
   
5) Calculate the Attrition Rate using a small query in the new measure option(SUM(HR ANALYTICS[ATTRITION COUNT])/SUM(HR ANALYTICS[EMPLOYEE COUNT])) *100 .We also need to create a whole number column for attrition in the Power Query .For that use Conditional Column and use Value as '1' for Yes and '0' For No.Then use close and apply in power query .
   
6) Then device more cards based on same steps.But in  cards having Average Age ,Average working years we need to take average in the fields section .
   ![Screenshot (84)](https://github.com/user-attachments/assets/2dc3da24-d051-4693-9edf-6316bd5ce3d2)
   
6)   We then construct 6 charts and tables based on the requirements of Education , Age, Job Satisfaction ,Salary ,Years Worked and Job Role .

a) Attrition count by education : Here we see the education qualifications of the employees who leave the firm .A pie chart or donut chart can display the proportion of employees at each education level, helping to contextualize the attrition data.
![Screenshot (82)](https://github.com/user-attachments/assets/d78822ab-4cda-4803-b438-410cba5c0772)

b) Attrition count by Age group : Here we see the age group  of the employees who leave the firm using a bar chart .Use a bar chart with age groups (e.g., 20-30, 31-40, 41-50) on the x-axis and attrition rate on the y-axis. This can reveal trends, such as whether younger or older employees are more likely to leave.
![Screenshot (83)](https://github.com/user-attachments/assets/fd73f142-b9ea-497c-ac3e-709113a2cc7b)

c) Attrition count by Job Satisfaction :Job satisfaction score by the various departments can describe about the contions in that particular department that cause the employee to leave the firm .This helps identify if lower satisfaction correlates with higher attrition.
![Screenshot (87)](https://github.com/user-attachments/assets/d58eae4a-1ea6-40a5-9f5d-3ec06489a52d)

d) Attrition count by Salary :This helps to find the payscale of employees who leave the firm the most .
![Screenshot (86)](https://github.com/user-attachments/assets/480087ae-d414-445c-bff1-ca59a575f369)

e) Attrition count by Number of years worked : This helps to find in which year of job the attrition rate is the highest .
![Screenshot (85)](https://github.com/user-attachments/assets/67eb42a7-35dd-436a-9b8d-354250130e2f)

f) Attrition rate by Job Role : This helps us to find out which job roles cause the most attrition .
![Screenshot (88)](https://github.com/user-attachments/assets/10e740ed-bb51-4954-b406-64382f55d1fc)

7) The final Dashboard looks like :
![Screenshot (89)](https://github.com/user-attachments/assets/f474c496-64fe-46bd-a056-087ad925f7e4)

 












   
   

 







