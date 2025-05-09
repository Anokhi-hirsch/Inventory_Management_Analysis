# Inventory and Supply Chain Analysis Dashboard

This Power BI project presents a comprehensive dashboard designed to analyze key metrics related to inventory and supply chain performance. It enables businesses to monitor operations, identify bottlenecks, and optimize decision-making through data-driven insights across regions and product categories.

## Objective

The goal of this project is to provide actionable insights for optimizing warehouse space, managing transportation costs, tracking sales trends, and identifying potential supply chain issues using visual analytics.

![Inventory and Supply Chain Dashboard](https://github.com/Anokhi-hirsch/Inventory_Supply_Chain_Analysis/blob/main/Screenshot%202025-05-05%20204633.jpg?raw=true)

## Dataset

The dataset includes historical and operational data across the following dimensions:
- Product Categories: Accessories, Clothing, Electronics, Furniture  
- Regional Data: North, South, East, West  
- Key Data Fields: Inventory Level, Warehouse Capacity, Cost of Goods Sold, Units Sold, Transportation Cost, Lead Time, Order Status  

## Key Metrics

- Warehouse Utilization  
- Days Sales of Inventory  
- Inventory Turnover Ratio  

## Tools and Technologies

- Power BI for data modeling and dashboard development  
- Microsoft Excel for data preparation  
- DAX for calculated measures  

## Core Calculations (DAX)

```DAX
Warehouse Utilization = 
DIVIDE(SUM('Inventory & Supply Chain Data'[Inventory Level]),
       SUM('Inventory & Supply Chain Data'[Warehouse Capacity])) * 100

Days Sales of Inventory = 
DIVIDE(SUM('Inventory & Supply Chain Data'[Inventory Level]),
       SUM('Inventory & Supply Chain Data'[Cost of Goods Sold])) * 365

Inventory Turnover Ratio = 
DIVIDE(SUM('Inventory & Supply Chain Data'[Cost of Goods Sold]),
       AVERAGE('Inventory & Supply Chain Data'[Inventory Level]))
```

## Insights and Recommendations

- Warehouse capacity is underutilized, suggesting a need for better inventory distribution or space planning.  
- High backorder volume indicates potential issues in demand forecasting or supplier delays.  
- Regional transportation costs vary significantly, pointing to opportunities for optimizing logistics.  
- Sales volume has grown significantly in recent years, requiring more agile inventory management.  
- Lead times are consistent across product categories, indicating stable supplier performance.
