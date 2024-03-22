# HerTech-Trail-Bootcamp


## **Table of Contents**
- [Project Overview](#project-overview)
- [Data Source](#data-source)
  - [Dataset Description](#dataset-description)
- [Tool Used](#tool-used)
- [Data Cleaning and Preprocessing](#data-cleaning-and-preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results and Findings](#results-and-findings)
- [Recommendations](#recommendations)
- [Limitation(s)](#limitation(s))


### Project Overview
---
The Car Owner Dataset Analysis project aims to explore and analyze a dataset containing information about car owners. By examining various attributes such as policy start and end dates, demographic information, car details, and geographic location, this project seeks to uncover insights that could inform business strategies, marketing campaigns, and risk assessment processes within the automotive industry. 

However, this project narrows down to data manipulations, exploration and a few visual relationships.


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
I used Python (Google Collab) for this analysis.
Python is a versatile programming language renowned for its extensive libraries and robust data analysis capabilities, was utilized as the primary tool for conducting the analysis of the car owner dataset.


### Data Cleaning and Preprocessing
---
In data cleaning and preprocessing, missing values, outliers, and inconsistencies in the dataset were handled.

By addressing missing values, outliers, and inconsistencies in the dataset during the data cleaning and preprocessing stage, analysts ensure that the data is reliable, accurate, and suitable for further analysis, leading to more robust and trustworthy results.

 - First, I imported Python libraries (Pandas, NumPy) to facilitate efficient data manipulation, exploration, and visualization tasks yet ensuring its suitability for analysis.

![](Capture-1.JPG)

 - Next the data is read thus:     `df = pd.read_csv(r'C:\Users\hp\Downloads\Nig_data - Nig_data (1).csv')`

 - Data assessment begins
    - I checked for datatypes   `df.dtypes` and the inaccurate datatypes noted
    - I checked for null values and duplicates
   
   print(df.isnull().sum())
   print(f"This is the number of duplicates: {df.duplicated().sum()}")
      


