
![Skills_Network](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0221EN-Coursera/images/image.png)  

# Case Study
## Building a Sales and Service Dashboard with Google Looker Studio
### IBM Data Engineering Professional Certificate – Final Assignment (Part 2B)

---

## 1. Introduction

This case study explains step-by-step how to complete the **Final Assignment – Part 2B**
of the *IBM Data Engineering Professional Certificate*.

In this assignment we recreate a **Business Intelligence dashboard using Google Looker Studio**.
The objective is to build a **two-page dashboard** that allows a regional manager of a car dealership
network to analyze both **sales performance** and **service performance**.

The final dashboard contains:

• A **Sales dashboard** with five visualizations  
• A **Service dashboard** with four visualizations  

---

# 2. Software Used

Google Looker Studio (Free Version)

https://lookerstudio.google.com/

---

# 3. Dataset

The dataset used in this assignment comes from the **IBM Accelerator Catalog**.
The files provided in the lab must be uploaded to **Google Drive** and connected
to Looker Studio using the **Google Sheets connector**.

Steps:

1. Download the dataset from the assignment lab.
2. Upload the files to **Google Drive**.
3. If necessary, open the files in **Google Sheets**.
4. Use the **Google Sheets connector** inside Looker Studio to connect the data.

---

# 4. Creating the Dashboard Report

## Step 1 — Create a New Report

1. Open **Google Looker Studio**
2. Click **Blank Report**
3. Add a **Data Source**
4. Choose **Google Sheets**
5. Select the dataset files uploaded to Google Drive
6. Click **Add to Report**

Now the dataset is connected and visualizations can be created.

---

# 5. Creating the Sales Dashboard

Rename **Page 1 → Sales**

The layout should contain **5 panels**:

4 small panels on the top and one large panel below.

---

## Panel 1 — Profit KPI

Insert a **Scorecard**

Configuration:

Metric:
Profit

Format:
Currency

Display Unit:
Millions (M)

Decimal precision:
1

Example result:

Profit = **$78.3M**

---

## Panel 2 — Quantity Sold

Insert another **Scorecard**

Metric:

Quantity Sold

This shows the total number of vehicles sold.

Example:

Quantity Sold = **58,118**

---

## Panel 3 — Quantity Sold by Model

Insert a **Bar Chart**

Dimension:

Model

Metric:

Quantity Sold

Sort:

Descending

This visualization compares how many units were sold for each car model.

---

## Panel 4 — Average Quantity Sold

Insert a **Scorecard**

Metric:

Average Quantity Sold

Example value:

19.37

---

## Panel 5 — Profit by Dealer ID

Insert a **Column Chart**

Dimension:

Dealer ID

Metric:

Profit

Sort:

Ascending

This chart allows the manager to compare dealer performance based on profit.

---

# 6. Creating the Service Dashboard

Add a **new page**.

Rename it:

Service

The layout must contain **4 panels arranged in a 2×2 grid**.

---

## Panel 1 — Number of Recalls by Model

Insert a **Column Chart**

Dimension:

Model

Metric:

Units

This chart shows how many recall events exist for each vehicle model.

---

## Panel 2 — Customer Sentiment

Insert a **Treemap**

Dimension:

Sentiment

Metric:

Record Count

Categories:

• Positive  
• Neutral  
• Negative

This visualization compares the distribution of customer reviews.

---

## Panel 3 — Quantity Sold vs Profit by Month

Insert a **Combo Chart**

Dimension:

Month

Metrics:

Quantity Sold (bars)  
Profit (line)

This visualization compares monthly sales volume with profit trends.

---

## Panel 4 — Recalls by System and Model

Insert a **Pivot Table**

Rows:

Model

Columns:

System Affected

Metric:

Units

Enable:

Heatmap

This chart highlights which vehicle systems experience the most recalls.

---

# 7. Exporting the Dashboard

Once both pages are completed:

1. Click the **Share** button
2. Select **Download Report**
3. Choose **Download as PDF**
4. Select **All Pages**
5. Click **Download**

Save the PDF file locally for submission.

---

# 8. Final Dashboard Structure

The final report contains:

Sales Dashboard

• Profit KPI  
• Quantity Sold KPI  
• Quantity Sold by Model  
• Average Quantity Sold KPI  
• Profit by Dealer ID  

Service Dashboard

• Recalls by Model  
• Customer Sentiment Treemap  
• Quantity Sold vs Profit by Month  
• Recalls by System and Model Heatmap  

---

# 9. Skills Demonstrated

Business Intelligence  
Dashboard Design  
Data Visualization  
Google Looker Studio  
KPI Analysis  
Sales Analytics  
Service Analytics

---

# 10. Conclusion

This assignment demonstrates how **Google Looker Studio** can be used to transform
raw operational data into an **interactive dashboard** that supports business decision making.

The two dashboards provide visibility into:

• Sales performance across dealerships  
• Customer sentiment and service issues  
• Monthly revenue trends  
• Product reliability through recall analysis

