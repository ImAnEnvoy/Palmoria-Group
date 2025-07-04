# DSA Data Analysis (DSA Incubator Project) Documentation
This is where I started my portfolio building while taking my Data Analysis class with the Incubator Hub. As a result, I completed the final project using the Plamoria Group data set. This project was carried out to showcase my critical thinking, analytics, problem solving skills etc accumulated sofar during the DSA Incubator Data Analysis classes. This project done using Power BI tool, and as such, features such as power query, cards, slicers were used.
While carrying out this project, I assumed the position of HR Analytics expert for Plamoria Group.

## Project topic: 
Analysis on Gender Equality

### Project overview
The Palmoria Group is a manufacturing company based in Nigeria, embroiled in issues bordering on gender inequality in its 3 regions which are (Abuja, Kaduna Lagos).  The task to identify 
key areas within the business that could give rise to issues and address them immediately, and come up with recommendations for management’s attention and help to disanull the news headline “Palmoria, the Manufacturing Patriarchy”, by considering the gender, rating, pay gap, salary distributions structure of Plamoria Group and it's regions

For this analysis, a comprehensive Exploratory Data Analysis (EDA) was carried out using the Power Bi tools and techniques relevant to the context of this dataset was employed. THis included: 
- Ingestion: this is connecting analytics system with the storage system.
- Transformation: Cleaning the data to remove unwanted (null, error values, blanks etc) data from the dataset
- Modeling: Analyzing how two or more tables (or data set) are related. 
- Visualization: interpreting the data visuals e.g. graphs, chart, etc
- Analysis: performing calculations with the data
- Presentation: submitting the findings for decision making

## Discription of Data:
### Data Source
The Plmoria data was given by the CHRO, Mr Yunus Shofoluwe.

### Tools Used
This project utilizes Power BI tool and it powerful features like:
- Power query:
    - for connection to the data
    - For data cleaning, creating measures etc
- Power BI (for creating a report)
- Github repository (for project portfolio)

### Total Rows and Columns
Total Records: 874
Columns: 6

### Data Cleaning and Preparation
The following were done to clean and prepare the data for analysis and visiualization
- Assign a generic gender (e.g unknown) to status to these employees employees who refused to disclose their gender.
- Remove blanks (i.e. some employees are without a salary because they are no longer with the company).
- Remove departments that are indicated as “NULL”.
- Create measures ussing DAX expressions to determine total employee, percentages and number of male/female, average salary, etc

### Data Analysis Task
The analysis task for the project dataset are:
- Gender pay gap anaysis
    - To determine the gender distribution in the organization, and based on regions and departments 
    - To show insights for gender based on ratings based 
- Salary structure/regulation compliance
    - To analyse the company’s salary structure, and identify if there is a gender pay gap. If there is, identify the department and regions that should be the focus of management 
    - Identify if the company meets up with regulation that was adopted which requires manufacturing companies to pay employees a minimum of $90,000 
    - To show the pay distribution of employees grouped by a band of $10,000. For example: 
    - To determine How many employees fall into a band of $10,000 – $20,000, $20,000 – $30,000, etc.? 
- Insights and reporting
    - visualization by regions 

### Useful DAX expression
- Population = COUNTROWS('Palmoria Group emp-data')
- male = CALCULATE([Population],'Palmoria Group emp-data'[Gender]="Male")
- % Male = DIVIDE([male],[Population],0)
- female = CALCULATE([Population],'Palmoria Group emp-data'[Gender]="Female")
- % Female = DIVIDE([female],[Population],0)
- Unknown Gender = CALCULATE([Population],'Palmoria Group emp-data'[Gender]="Unknown")
- % unknown = DIVIDE([Unknown Gender],[Population])
- Total Salary = SUM('Palmoria Group emp-data'[Salary])
- Average Salary = AVERAGE('Palmoria Group emp-data'[Salary])
- Max salary = CALCULATE(MAX('Palmoria Group emp-data'[Salary]))
- Min salary = CALCULATE(Min('Palmoria Group emp-data'[Salary]))

## Screenshots
### Overall Gender Distribution
<img width="797" alt="Gender Distribution" src="https://github.com/user-attachments/assets/49c470ff-d2fc-41ee-9127-bd1176a87245" />

### Rating
<img width="802" alt="Rating" src="https://github.com/user-attachments/assets/e011cdd1-3d25-4b99-b8de-bbbade1eb5f1" />

### Salary Distribution/Structure
<img width="794" alt="Salary distribution" src="https://github.com/user-attachments/assets/e4d4d63a-1695-438e-b282-8fcacaf36c00" />

### Data Table
<img width="959" alt="data" src="https://github.com/user-attachments/assets/ea305950-7a3e-444c-83b1-b215188d4452" />

## Findings
The gender distribution at Plamoria Group is said to be balanced with 49% of males, 46% of females and 4% representing those whose gender was not stated. Gender distribution however vary by region and department, with Kaduna showing the largest gap of 51% males, 45% females. On the other hand, Abuja has an even distribution of 47%.

## About Me
###Ayoola Ezekiel O.
Higher National Diploma (HND) in Computer Science from the Federal Polytechnic Bauchi, Nigeria. I am passionate about learning, working and drawing actionable insights from data. My data analysis journey is also blended with graphics designs, which allows me to create dashboard visual for reporting and presentation.

## Contacts
Feel free to reach out to me on:
Email:       ezekieloluwafemiayoola@gmail.com
Phone:       +234 307 5187 993
WhatsApp:    +234 817 9264 472
Linkedin:    www.linkedin.com/in/ezekiel-ayoola-89a10983

##GitHub Support
If you find this work intersting and resourseful, kindly ⭐ this repository. Thank you.
