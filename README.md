# HerTech-Trail-Bootcamp


## **Table of Contents**
- [Project Overview](#project-overview)
- [Data Source](#data-source)
  - [Dataset Description](#dataset-description)
- [Tool Used](#tool-used)
- [Data Cleaning and Preprocessing](#data-cleaning-and-preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Results and Findings](#results-and-findings)
- [Limitation(s)](#limitation(s))


### Project Overview
---
The Car Owner Dataset Analysis project aims to explore and analyze a dataset containing information about car owners. By examining various attributes such as policy start and end dates, demographic information, car details, and geographic location, this project seeks to uncover insights that could inform business strategies, marketing campaigns, and risk assessment processes within the automotive industry. 

However, this project narrows down to data manipulation, exploration and a few visual relationships.


### Data Source
---
The dataset utilized in this analysis consists of information pertaining to car owners. It was sourced from "Nig_data.csv", a reputable data provider known for its comprehensive datasets in the automotive domain.

  - **Dataset Description**

The dataset comprises the following attributes:

  1. **ID**: Unique identifier for each car owner.
  2. **Policy Start Date**: Date when the car insurance policy starts.
  3. **Policy End Date**: Date when the car insurance policy ends.
  4. **Gender**: Gender of the car owner.
  5. **Age**: Age of the car owner.
  6. **Car Category**: Category or type of the car (e.g., Saloon, Jeep).
  7. **Subject Car Colour**: Colour of the car owned by the individual.
  8. **Subject Car Make**: Make or manufacturer of the car owned by the individual.
  9. **LGA (Local Government Area)**: Geographic area where the car owner resides.
 10. **State**: State where the car owner resides.
 11. **Product Name**: Name of the insurance product.
 12. **Target**: Target variable (e.g., likelihood of policy renewal, customer churn, etc.).


### Tool Used
---
I used Python (Google Collab) for this analysis [See Here](https://colab.research.google.com/#scrollTo=GJBs_flRovLc)

Python is a versatile programming language renowned for its extensive libraries and robust data analysis capabilities, was utilized as the primary tool for conducting the analysis of the car owner dataset.


### Data Cleaning and Preprocessing
---
In data cleaning and preprocessing, missing values, outliers, and inconsistencies in the dataset were handled.

By addressing missing values, outliers, and inconsistencies in the dataset during the data cleaning and preprocessing stage, analysts ensure that the data is reliable, accurate, and suitable for further analysis, leading to more robust and trustworthy results.

 - First, I imported Python libraries (Pandas, NumPy) to facilitate efficient data manipulation, exploration, and visualization tasks yet ensuring its suitability for analysis.

![library import](https://github.com/DebComet/HerTech-Trail-Bootcamp/assets/158510031/57fdf08e-df1b-4638-9f2a-92b8e8fa0ddc)

 - Next the data is read thus:     `df = pd.read_csv(r'C:\Users\hp\Downloads\Nig_data - Nig_data (1).csv')`
![Capture 1](https://github.com/DebComet/HerTech-Trail-Bootcamp/assets/158510031/d3e0e045-07ed-409f-a544-2bdb7f96611e)

 - Data assessment begins
    - I checked for datatypes   `df.dtypes` and the inaccurate datatypes noted
    - I checked for null values and duplicates
   
`print(df.isnull().sum())`
`print(f"This is the number of duplicates: {df.duplicated().sum()}")`
![Null value 2](https://github.com/DebComet/HerTech-Trail-Bootcamp/assets/158510031/d715ff11-4d5b-4343-9711-827119285259)

![Datatypes pic](https://github.com/DebComet/HerTech-Trail-Bootcamp/assets/158510031/0382d0fc-c09e-4d41-ba4e-2067231d3a03)

- I assessed inconsistencies in the data entries

![Assessing inconsistencies](https://github.com/DebComet/HerTech-Trail-Bootcamp/assets/158510031/a3438dd7-5c83-47a0-a8f4-a50a17677393)

- I checked for outliers

![Outliers](https://github.com/DebComet/HerTech-Trail-Bootcamp/assets/158510031/238db8ef-5ce1-41ba-9b9e-7e5845dc562c)

- Then data cleaning proper

![Data cleaning](https://github.com/DebComet/HerTech-Trail-Bootcamp/assets/158510031/a614a42c-2f40-4738-9c54-522968edc639)

   - I handled the datatypes

![Handeling datatype](https://github.com/DebComet/HerTech-Trail-Bootcamp/assets/158510031/e89a0bea-0b97-432a-8462-fc77be06f162)

   - I handled null vaues

![handling null values 1](https://github.com/DebComet/HerTech-Trail-Bootcamp/assets/158510031/eb85a2fa-37b0-4edf-8aba-ddd461b4acd8)

![handling null values 2](https://github.com/DebComet/HerTech-Trail-Bootcamp/assets/158510031/7ddc15ae-0651-4b5b-bc34-864bf142eeaa)

   - Data inconistencies were also handled

![handling data incnsistencies](https://github.com/DebComet/HerTech-Trail-Bootcamp/assets/158510031/b72fbcd0-5a43-4cae-8807-589fe3aa8373)

![handling data inconsistencies 2](https://github.com/DebComet/HerTech-Trail-Bootcamp/assets/158510031/25204c8b-b6af-46f3-98e5-03f4c1d01e61)

   - I cleaned the LGA names

![LGA NAMES](https://github.com/DebComet/HerTech-Trail-Bootcamp/assets/158510031/ec6d7abd-5be8-46fc-bbcb-309c7f3ca298)

- Data is now clean!

![df clean](https://github.com/DebComet/HerTech-Trail-Bootcamp/assets/158510031/9a718aee-3a9a-4e8c-b405-6a6b3e570f48)

### Exploratory Data Analysis

Exploratory Data Analysis (EDA) serves as a fundamental pillar in the data analysis journey. It helps us see what's in the data and understand it better. By looking closely at the data, we can spot any problems or tricky things that need fixing before we start doing complicated stuff. EDA basically helps us build a strong base so we can explore the data more confidently later on.

 - I imported matplotlip to further undertand the data

![EDA 1](https://github.com/DebComet/HerTech-Trail-Bootcamp/assets/158510031/174a3fa6-bc3d-438c-bdc4-3a5b7de00485)

![EDA 2](https://github.com/DebComet/HerTech-Trail-Bootcamp/assets/158510031/098477f4-0fe1-4fcc-9491-93a1b7dfe4cf)

![EDA 3](https://github.com/DebComet/HerTech-Trail-Bootcamp/assets/158510031/a0ba0d73-bc44-4f8d-bfaa-c44ee7714766)

![EDA 4](https://github.com/DebComet/HerTech-Trail-Bootcamp/assets/158510031/770a1cde-1de8-4ca0-b035-b315eceecc67)

### Results/Findings
  - Good study and understanding of the dataset will help an analysis use the best approach in analyzing the data.
  - In cases where the are numerous null values, an analysis mustn't consider eliminating them, but should rather ask questions or should consider replacing the null values with the     
    mode of the distribution as an alterntive.

### Limitation(s)
I had to replace the null values with the mode of the ditribution in other not to loose vital information in the dataset that would affect he accuracy of my concluion from the analysis.
