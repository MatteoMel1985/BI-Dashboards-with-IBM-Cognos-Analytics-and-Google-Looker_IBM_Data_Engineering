
![Skills_Network](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0221EN-Coursera/images/image.png)  

<h1 align="center">Google Looker - Final Assignment</h1>  

# Creating the Dashboard Report

## Step 1: Create a New Report

1. Open **Google Looker Studio**
2. Click **Blank Report**
3. Add a **Data Source**
4. Choose **Google Sheets**
5. Select the dataset files uploaded to Google Drive
6. Click **Add to Report**

Now the dataset is connected and visualisations can be created.

---

# Creating the Sales Dashboard

Rename **Page 1 → Sales**

The layout should contain **5 panels**:

4 small panels on the top and one large panel below.

## Panel 1: Profit KPI

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

## Panel 2 — Quantity Sold

Insert another **Scorecard**

Metric:

Quantity Sold

This shows the total number of vehicles sold.

Example:

Quantity Sold = **58,118**

## Panel 3 — Quantity Sold by Model

Insert a **Bar Chart**

Dimension:

Model

Metric:

Quantity Sold

Sort:

Descending

This visualisation compares how many units were sold for each car model.

## Panel 4: Average Quantity Sold

Insert a **Scorecard**

Metric:

Average Quantity Sold

Example value:

19.37


## Panel 5: Profit by Dealer ID

Insert a **Column Chart**

Dimension:

Dealer ID

Metric:

Profit

Sort:

Ascending

This chart allows the manager to compare dealer performance based on profit.

# Creating the Service Dashboard

Add a **new page**.

Rename it:

Service

The layout must contain **4 panels arranged in a 2×2 grid**.


## Panel 1: Number of Recalls by Model

Insert a **Column Chart**

Dimension:

Model

Metric:

Units

This chart shows how many recall events exist for each vehicle model.

## Panel 2: Customer Sentiment

Insert a **Treemap**

Dimension:

Sentiment

Metric:

Record Count

Categories:

• Positive  
• Neutral  
• Negative

This visualisation compares the distribution of customer reviews.

## Panel 3: Quantity Sold vs Profit by Month

Insert a **Combo Chart**

Dimension:

Month

Metrics:

Quantity Sold (bars)  
Profit (line)

This visualisation compares monthly sales volume with profit trends.

## Panel 4: Recalls by System and Model

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


# Exporting the Dashboard

Once both pages are completed:

1. Click the **Share** button
2. Select **Download Report**
3. Choose **Download as PDF**
4. Select **All Pages**
5. Click **Download**
Save the PDF file locally for submission.

