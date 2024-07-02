# Stock-Market-Analysis

## Problem Statement
Observations on the following are made:
1. Closing Price of Stocks 
2. Total volume of stocks being traded each day
3. Daily Returns
4. Relationship between companies in terms of closing price
5. Risk Analysis

## Dataset

The dataset for this project can be downloaded here: https://bit.ly/SandP500StockData

- Overview of features in the dataset

   <img width="332" alt="Dataset overview" src="https://user-images.githubusercontent.com/71536311/192172474-fb920796-6b0e-4526-852e-6b364569d1ae.png">

- The dataset has the following columns:
    - **Date** - in format: yy-mm-dd
    - **Open** - price of the stock at market open (considering that this is NYSE data, all prices are in USD)
    - **High** - highest price reached in the day
    - **Low Close** - lowest price reached in the day
    - **Volume** - number of shares traded
    - **Name** - the stock's ticker name

## Data Analysis Using Python

### Closing Price of Stocks
- Convert string to date format of the ‘date’ feature.
- Extract the names of the companies (Amazon - AMZN, Apple - AAPL, Google - GOOG and Microsoft - MSFT) and plot the graph using **pyplot module** of **Python's matplotlib library**.

<p align="center"><img width="530" alt="image" src="https://user-images.githubusercontent.com/71536311/192176573-2ec7c7a9-d8f5-42a3-ac22-6dba3a90fb4e.png"></p> 

### Total volume of stocks being traded each day
- Visualized volume trading using **Python graphing library plotly**.

<p align="center"><img width="710" alt="image" src="https://user-images.githubusercontent.com/71536311/192260841-81bf6889-5f87-4aa1-82ad-3e2717a54335.png"></p> 
<p align="center"><img width="676" alt="image" src="https://user-images.githubusercontent.com/71536311/192274806-1975d653-dc4a-443e-8d17-a9bc8fae1192.png"></p> 

### Daily Returns
- Calculate the daily return by subtracting the open price from the close price and dividing it by 100.
- Plotted the daily returns graph using **plotly**.

<p align="center"><img width="443" alt="image" src="https://user-images.githubusercontent.com/71536311/192282101-931138c9-79bb-40fa-8b92-0166177fe9ae.png"></p>

### Relationship between companies in terms of closing price (Multivariate Analysis)
- Find maximum closing price for the feature by resampling it and finding mean.

<p align="center"><img width="332" alt="image" src="https://user-images.githubusercontent.com/71536311/192428389-1aed6be9-4d54-46e0-8e2c-607997a42e99.png"></p> 


- To illustrate the relationship between companies with respect to closing price, use the **seaborn library** and plot a **pairplot** or **heatmap** for describing the relationship.

<p align="center"><img width="386" alt="image" src="https://user-images.githubusercontent.com/71536311/192428488-2b38548e-8b35-427a-b1a0-b417a517758b.png"></p> 

### Risk Analysis
- Interpret the range that contains the majority of the data points to analyze the risk.

<p align="center"><img width="274" alt="image" src="https://user-images.githubusercontent.com/71536311/192429097-cf93ab38-a738-44ed-b84e-51e2678d7e6b.png"></p> 


## Tools Used
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)   ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)   ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)   ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)   ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23#ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=white)   ![Plotly](https://img.shields.io/badge/Plotly-%233F4F75.svg?style=for-the-badge&logo=plotly&logoColor=white)

- **Jupyter Notebook** is used as IDE.
- Among the **Python libraries**, **Pandas** and **NumPy** are used for handling data, preprocessing, and mathematical operations, respectively.
- **Plotly, Seaborn**, and **Matplotlib** are used for visualizing plots.

For more details, please go through the Jupyter Notebook attached above.

## Conclusion

- ***Amazon*** has the highest closing price out of the four companies.
- ***In 2014, Apple*** had a maximum volume trade of more than 250 million.
- Compared to previous years, ***2018*** closed with the highest price.
- The ***closing prices of Amazon and Microsoft are nearly the same***.
-  ***99.7% of all Apple data falls within the third standard deviation***, which ranges from -3.5 to 3.5.
