# online_retail


## Resources 
[Kaggle Dataset](https://www.kaggle.com/datasets/vijayuv/onlineretail)


## Project Sturcture 

```
├── OnlineRetail.csv      
├── clean_data.csv        
├── data_cleaning.ipynb   
├── data_analysis.ipynb
├── requirements.txt        
└── README.md
```

## Dataset Overview

The dataset contains online retail transactions.
### Key Fields
- `InvoiceNo`: Unique transaction ID
- `StockCode`: Product identifier
- `Quantity`: Number of units purchased
- `UnitPrice`: Price per unit
- `CustomerID`: Unique customer identifier
- `Country`: Customer location

## Feature Engineering

New features created:
- `TotalSales = Quantity × UnitPrice`
- `Hour`: Extracted from InvoiceDate
- `DayOfWeek`: Captures weekly purchasing patterns

## Dependencies
- pandas
- numpy
- matplotlib
- seaborn
- jupyter


## Data Cleaning Steps

- Removed duplicate transactions
- Handled missing `CustomerID` values
- Filtered out negative quantities (returns)
- Removed invalid unit prices (≤ 0)
- Converted `InvoiceDate` to datetime format


## Key Insights
<img width="1278" height="645" alt="top_10_quantity" src="https://github.com/user-attachments/assets/411f8295-f8b1-40b6-8d8f-be963519d756" />


- The top seller product, PACK OF 72 RETROSPOT CAKE CASES, contributes 18.3% of units sold among top 10 products. Additionally, Baking category which contains 'PACK OF 72 RETROSPOT CAKE CASES' and 'PACK OF 60 SPACEBOY CAKE CASES' products from top 10 products, have the highest sells. 

- The 'SPACEBOY LUNCH BOX' and 'DOLLY GIRL LUNCH BOX' products from Lunch boxes category have a similar sales volume, additionaly both products rank within the top 4 best-selling products. 
 
- The top 4 products account for approximately 58% of total sales volume among top-10 products. 

- Overall, small number of producst generate the majority of transactions. This indicates for highly concentrated sales distribution.
