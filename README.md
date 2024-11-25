# Customer Segmentation by RFM Analysis
# I. Introduction
## 1. Introduction to RFM analysis:
- RFM analysis is a popular customer analysis technique in marketing and customer relationship management (CRM). It evaluates customers based on three factors:
  - Recency (R): How recently did the customer make a purchase? The more recent, the higher their likelihood to engage.
  - Frequency (F): How often does the customer make purchases? Frequent buyers tend to be more loyal.
  - Monetary (M): How much has the customer spent in total? Higher spending indicates potentially valuable customers.
- By analyzing these factors, RFM helps businesses segment customers to optimize marketing strategies, personalize promotions, and enhance customer retention, driving data-driven decision-making efficiently.
## 2. Project Purpose:
- Determine RFM scores to segment customers into different groups.
- Analyze the company - Superstore's performance status and provide recommendations for the marketing department.
- Identify which of the three metrics (R, F, and M) should be prioritized.
# II. Exploratory Data Analysis - EDA
## 1. Explore Data:
  ![image](https://github.com/user-attachments/assets/54a4778d-0d4d-48e2-8538-e6825ec7ce75)
## 2. Apply Conditions On Dataset:
  ![image](https://github.com/user-attachments/assets/c4a121b5-9151-4528-ade6-372f4fdc225f)
  - Only users from UK are chosen for analysis, as they contributed for 98% of the dataset.
  - Data in 'Quantity' must take a positive value.
  - Data in 'UnitPrice' must take a positive value.
## 3. Check & Handle Null Values:
  ![image](https://github.com/user-attachments/assets/2987ea5a-590c-4686-9ad4-e011c08175db)
  - Null values are not accepted in primal key column.
  - Action: Drop null values.
## 4. Correct Data Type:
  ![image](https://github.com/user-attachments/assets/61355ad5-2c73-4d4d-8831-2360d590cac7)
  - Changing 'CustomerID' data type from float64 to int64.
## 5. Check & Handle Missing Values:
  ![image](https://github.com/user-attachments/assets/429ff302-27d3-438e-afc5-469af086d717)
## 6. Conclusion:
  ![image](https://github.com/user-attachments/assets/d3dc0a10-16c6-480c-b454-8ad748bad0d9)
# III. Data Visualization Using Python
## 1. Distribution of Recency:
   ![R](https://github.com/user-attachments/assets/d0ef484f-d93a-4faa-9ace-7d896f27db30)
   - The distribution of Recency is right-skewed. As the Recency increases, there is a steep decline in the number of customers.
   - The histogram shows that most customers have made recent purchases (<=100 days). About 1,700 customers have already bought something at Superstore in the last 50 days.
   - It indicates that most of the Superstore's customers are active customers who tend to make purchases recently.
## 2. Distribution of Frequency:
  ![F](https://github.com/user-attachments/assets/29d3405a-cee8-40f5-82ae-8a4164a705ce)
  - The distribution of Frequency is highly right-skewed. As the Frequency increases, there is a significant drop in the number of customers.
  - This historam shows that most of customers have fewer than 20 transactions. For particular, more than 3,500 customers have made 1 to 10 purchases, when only few hundreds of customers have placed more than 10 orders and barely any have placed 20 or more.
  - It indicates that the majority of Superstore's customers are low-frequency purchasers who do not make purchases often.
## 3. Distribution of Monetary:
  ![M](https://github.com/user-attachments/assets/fdde9212-e3da-4c89-81b6-4f470ca2d5e5)
  - The distribution of Monetary is highly right-skewed. As the Monetary increases, there is a significant drop in the number of customers.
  - This historam shows that most of customers have fewer than 10,000 monetary values. For particular, more than 3,500 customers have spent less than 5,000, when only hundreds of customers have spent more than 5,000. Virtually none have spent more than 10,000.
  - It indicates that most of Superstore customers have low spending, while a small portion of customers contributes to the high monetary value segment.
## 4. Customer Segmentation By Total Sale:
  ![Seg By Total Sales](https://github.com/user-attachments/assets/4b4e03e5-1db3-4cee-885e-77c9a15122c6)
  - Ranking the customer segmentation by total sales:
    1.Champions
    2.Loyal
    3.At Risk
    4.Need Attention
    5.Hibernating Customers
    6.Potential Loyalist
    7.Cannot Lose Them
    8.Lost Customers
    9.Promising
    10.About To Sleep
    11.New Customers
## 5. Customer Segmentation By Customer Value:
  ![Seg By Customer Value](https://github.com/user-attachments/assets/be74fc49-d574-42b4-871a-79db099811fd)
  - Ranking the customer segmentation by total sales:
    1.Champions
    2.Hibernating Customers
    3.Lost Customers
    4.Loyal
    5.Potential Loyalist
    6.At Risk
    7.Need Attention
    8.About To Sleep
    9.New Customers
    10.Promising
    11.Cannot Lose Them
## 6. Distribution Of Customer Across Segments:
  ![Dis Across Seg](https://github.com/user-attachments/assets/425b6680-07d3-4548-b7a8-d35ea5831840)
  - Customer segments can be categorized into 3 groups:
    - High-Value Customers (HVC): Champions, Loyal, Potential Loyalist, New Customers, Promising.
    - At-Risk Customers (ARC): Need Attention. About To Sleep, At Risk, Cannot Lose Them.
    - Low-Value Customers (LVC): Hibernating Customers, Lost Customers.
  ![image](https://github.com/user-attachments/assets/dbc6a3f0-87e4-447a-9c40-b96edddd0a14)
  - Observation:
    - HVC category contributes the most, with 1871 customers.
    - LVC category contributes the second - 1075 customers.
    - ARC category, while the smallest, still contributes a considerable amount of 974 customers.
    - It indicates that the business is in a growing state despite facing with several problems.
  # III. Insights
  ![image](https://github.com/user-attachments/assets/a3ee9c85-adf9-4ba4-a79d-4e6aad470888)
  - [Link](https://docs.google.com/spreadsheets/d/1MBt3b48lT-RzD44xsbMsgwtVO-JmIJjU/edit?usp=sharing&ouid=107825711284033293753&rtpof=true&sd=true)  
  # IV. Recommendation
  ![image](https://github.com/user-attachments/assets/92dfe72f-e37a-480e-9b63-8b4bd6fb47bb)
  ![image](https://github.com/user-attachments/assets/46e756d9-7165-4708-9b25-8d02b35f0feb)
  ![image](https://github.com/user-attachments/assets/f0130773-8e9b-4546-80c7-1534e9cafc9a)
  - [Link](https://docs.google.com/spreadsheets/d/1MBt3b48lT-RzD44xsbMsgwtVO-JmIJjU/edit?usp=sharing&ouid=107825711284033293753&rtpof=true&sd=true)

    








