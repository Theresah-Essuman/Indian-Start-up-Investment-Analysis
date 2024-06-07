### Indian-Start-up-Investment-Analysis - LP1

# 1. Project Overview
In this project, I explore the dynamic landscape of start-up funding in India from 2018 to 2021. My goal is to uncover key patterns, trends, and insights that characterize the investment ecosystem during these years. The dataset for this analysis was gathered from three different sources:







*First dataset*:  The data for 2020 and 2021 were saved in Microsoft SQL Server.

*Second dataset*: The data for 2019 were saved in OneDrive.

*Third dataset*: The data for 2018 were stored in GitHub repository.







# 2. Case Study


**Scenario**

Your team is trying to venture into the Indian start-up ecosystem. As the data expert of the team you are to investigate the ecosystem and propose the best course of action.



# 2.1 Ask


In this phase, I outline the business objectives, create hypotheses, and ask questions to support or refute these ideas. In addition, I hope to glean broad insights from the data.



# 2.2 Business Task

My main task is to analyse Indian start-up data in order to deliver relevant insights and answers to my team looking to enter the Indian start-up ecosystem. I would like to emphasise key metrics and considerations that will inform and guide their decisions before entering this dynamic market.



# 3. Hypothesis Testing
### Null Hypothesis (H0): 
 There is no significant difference in the average funding amounts received across different sectors within the Indian startup ecosystem from 2018 to 2021.

 ### Alternative Hypothesis (H1):
There is a significant difference in the average funding amounts received across different sectors within the Indian startup ecosystem from 2018 to 2021.

# 4. Business Questions

(4.1)  Analyze the growth trajectory of startups over the past four years from 2018 to 2021. Investigate if there is an increase in the number of startups being funded and the average size companies of funded annually.


(4.2) Investigate the financial landscape for Indian startups over the four years. Has the average funding amount increased, indicating growing investor confidence, or has it plateaued or decreased overtime?

(4.3) Identify the booming sectors withing the ecosystem and which top city serves as the industrial hub in India.

(4.4) Determine the top investors within the startup ecosystem and identify the proportion of investment by the first 3 investors that have funded different sectors from 2018 - 2021

(4.5) Explore which stages of startups (e.g., Seed, Series A, Series B) are receiving the majority of investments. What are the predominant stages funded, and which cities are the identified stages of business situated.



# 5. Deliverables
- A hypothesis.

- Questions to help gain insights into the data. A summary of the Analysis.

- Visualizations to communicate findings.

- Recommendations based on the analysis.





# 6. Data Preparation and Quality Checks
During this step, I collected data from several sources for the analysis.


# 7. Information on Data

The data for the project was provided by Azubi Africa (Trainers). The data contains 4 csv files: data_2018.csv, data_20192.csv, data_2020 (from SQL server) and data_2021 (also from SQL server)


### 7.1 The columns in the dataset are as follows:

- Company Name: The name of the company.
- Founded: The year the company was founded.
- Sector: The sector the company operates in.
- Stage: The funding stage of the company.
- Location: The location of the company’s headquarters.
- Amount: The amount of funding the company received.
- Description: The ‘The About of company’.
- Investor: The investor who funded the company.
- Founder: The founders of the company.


### 7.2 Limitations of the Data

The 2018 start-up data lacks two columns (Founders, Founded) that are present in the 2019, 2020, and 2021 datasets. It is important to note that the source of the 2018 dataset is unknown, and therefore, this data cannot be considered reliable for making real-life recommendations for entrepreneurs.


# 8. Data Selection

For the purpose of this study, all four datasets (2018-2021) were retrieved from their respective sources.


# 9. Tools for Analysis
The following tools were utilized:

- Python's:

- Pandas: For data manipulation and cleaning.

- NumPy: For numerical operations.

- Matplotlib and Seaborn: For data visualization.

- SQL: For querying and managing the 2020 and 2021 data stored in Microsoft SQL Server.

- GitHub: To access the 2018 dataset and manage version control for any scripts or notebooks used in the analysis.

- Jupyter Notebook: For interactive data analysis and sharing insights through well-documented notebooks.


# 10. Process
In this face, I preview all the 4 dataset to understand the structure

### 10.1 Imported relevant Libraries

import pyodbc
from dotenv import dotenv_values
import pandas as pd
import warnings
import numpy as np

warnings.filterwarnings('ignore')


### 10.2 Establishes a connection to server






