# Supermarket-Sales-Analysis
This is a python project analyze the dataset from a fictional supermarket chain to uncover key insights about store performance
## INTRODUCTION 
This project analyze a dataset from a fictional supermarket chain to uncover key insight about store performance. Python and Pandas was used in goggle collab to explore relationship between store size, inventory, customer traffic, revenue. The goal helps stakeholders understand which stores are performing best and why. 

**TABE OF CONTENT** 

[PROJECT SUMMARY AND OBJECTIVES](https://github.com/OlajesuOgunyemi/Supermarket-Sales-Analysis#1-project-summary-and-objectives) 

[DATASET DESCRIPTION](https://github.com/OlajesuOgunyemi/Supermarket-Sales-Analysis#2-data-description) 

[ENVIRONMENT AND TOOLS](https://github.com/OlajesuOgunyemi/Supermarket-Sales-Analysis#3-environment-and-tools) 

[STEP BY  STEP DATA ANALYSIS](https://github.com/OlajesuOgunyemi/Supermarket-Sales-Analysis#4-step-by-step-analysis) 

     Loading and inspecting the data 

    Cleaning and preparing colums 
    
    Question 1: Which store has the highest sales? 

    Question 2 : What the average store area and daily customer 

    Question 3 : Relationship between store area and daily customer count 

    Question 4 : Top Store by sales and traffic
    

[RECOMMENDATION](https://github.com/OlajesuOgunyemi/Supermarket-Sales-Analysis#5-recommendation) 





## 1 PROJECT SUMMARY AND OBJECTIVES

Exploratory analysis were performed to answer questions like 

***. Which store sold the most*** 

***. What is the average area and customer count per store***

***. Do bigger store get more customers*** 




## 2 DATA DESCRIPTION** 

Five stores, each rows  include 

***STORE  ID*** 

***STORE  AREA*** 

***ITEM AVAILABLE*** 

***DAILY CUSTOMER COUNT*** 

***STORE SALES***



## 3 ENVIRONMENT AND TOOLS** 

***Python*** :(Jupiter style notebook in goggle colab) 

***Pandas*** : for data handling 

 

## 4 STEP BY STEP ANALYSIS** 

**a)  Loading and inspecting**

import pandas as pd 
**df = pd.read_csv('/content/drive/MyDrive/Sales Data/Supermarket sales.csv')** 

**df.head()** 

**df.columns.tolist()**

**b) cleaning and preparing** 

Ensured no missing values and proper datatype 

 

**C)  Question 1** : Which store has the highest sales 

**top_store = df.loc[df['Store_Sales'].idxmax()]** 

 

**d) Question 2** :  Average area and daily customer 

**avg_area = df['Store_Area'].mean() avg_customers = df['Daily_Customer_Count'].mean()** 

 

**e) Question 3** : Relationship between area and customers 

**corr = df['Store_Area'].corr(df['Daily_Customer_Count'])** 

 

**f) Question 4** : Top 5 store by sales 

**top5 = df.nlargest(5, 'Store_Sales')**

## 5 RECOMMENDATION** 

  **Expand Analysis** : Add visualization (e.g scatter plot) for presentation or dashboard project 

  **Modelling** : Use the correlation findings to predict customer count or revenue using simple regression 

  **Portfolio Integration** :  

 
