![Skills_Network](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0221EN-Coursera/images/image.png)  

<h1 align="center">IBM Cognos Analytics - Final Assignment</h1>  

This case study explains, step by step, how to complete the **Final Assignment – Part 2** of the IBM course **BI Dashboards with IBM Cognos Analytics and Google Looker** on Coursera.

The objective of the exam is to create **two dashboard tabs** in IBM Cognos Analytics, using the sample dataset **Auto group data module**, and to export the final dashboard as a PDF for submission.

---

## 1. Understanding the Assignment

The official assignment asks you to create **two dashboards** inside the same Cognos dashboard project:

- a **Sales** tab, using the template with **4 small panels at the top and 1 large panel below**
- a **Service** tab, using the **2 × 2 panel template**

The dataset is already available inside Cognos as **Auto group data module**, under:

`Team content > Samples > By industry > Automotive > Data`

From there, you must right-click the data module and choose **Create Dashboard**.

---

## 2. What You Need Before Starting

Before building the dashboard, make sure that:

- you are logged into your Cognos Analytics trial environment
- you can access **Team content**
- the sample path **Samples > By industry > Automotive > Data** is visible
- the item **Auto group data module** is available

Once this is confirmed, you are ready to begin.

---

## 3. Open the Dataset and Create the Dashboard

### Step 1 — Open Team Content

From the left navigation panel in Cognos:

1. Click **Team content**
2. Open **Samples**
3. Navigate to:
   - **By industry**
   - **Automotive**
   - **Data**

### Step 2 — Create a Dashboard from the Data Module

Find **Auto group data module**.

1. Right-click on **Auto group data module**
2. Select **Create Dashboard**

Cognos will now ask you to choose a dashboard template.

---

## 4. Create the First Tab: Sales

The first required dashboard is the **Sales** tab.

### Step 3 — Choose the Correct Template for Sales

Select the tabbed template that contains:

- **4 small rectangles on the top row**
- **1 large rectangle below them**

This is the exact template required by the exam.

### Step 4 — Rename the Tab

Once the dashboard opens:

1. Click the tab name
2. Rename it to:

```text
Sales
```

---

## 5. Build the Sales Dashboard

The Sales dashboard must contain **five visualizations**.

---

### Panel 1 — Profit KPI

In the **first small rectangle**, create a KPI for **Profit**.

#### Required result

- Metric: **Profit**
- Visualization type: **KPI / single value**
- Formatting: **1 decimal place**
- Unit: **millions of US dollars**

#### How to do it

1. Drag the field **Profit** into the first panel
2. Let Cognos create a KPI visualization
3. Open the visualization properties or formatting options
4. Format the number so it displays in **millions**
5. Set it to **1 decimal place**

Your final result should look similar to:

```text
$78.4M
```

---

### Panel 2 — Quantity Sold KPI

In the **second small rectangle**, create a KPI for **Quantity Sold**.

#### Required result

- Metric: **Quantity Sold**
- Visualization type: **KPI / single value**

#### How to do it

1. Drag **Quantity Sold** into the second panel
2. Keep it as a single-value KPI

This should show the total quantity sold across the dataset.

---

### Panel 3 — Quantity Sold by Model

In the **third small rectangle**, create a **bar chart** showing **Quantity Sold by Model**.

#### Required result

- Category: **Model**
- Measure: **Quantity Sold**
- Visualization type: **Bar chart**

#### How to do it

1. Drag **Model** into the third panel
2. Drag **Quantity Sold** onto the same panel
3. If Cognos does not automatically create the correct chart, change the visualization type manually to **Bar**

This panel should compare the quantity sold across the different car models.

---

### Panel 4 — Average Quantity Sold

In the **fourth small rectangle**, create a KPI for **Average Quantity Sold**.

#### Required result

- Metric: **Quantity Sold**
- Aggregation: **Average**
- Visualization type: **KPI / single value**

#### How to do it

1. Drag **Quantity Sold** into the fourth panel
2. Open the aggregation options
3. Change aggregation from **Sum** to **Average**

The result should display the average quantity sold rather than the total.

---

### Panel 5 — Profit by Dealer ID

In the **large lower rectangle**, create a **column chart** showing **Profit by Dealer ID**.

#### Required result

- Category: **Dealer ID**
- Measure: **Profit**
- Visualization type: **Column chart**
- Sorting: **Ascending order**

#### How to do it

1. Drag **Dealer ID** into the large bottom panel
2. Drag **Profit** into the same panel
3. Set the chart type to **Column**
4. Open the sorting options
5. Sort the visualization in **ascending order**

This is one of the most important grading points, so make sure the sort order is correct.

---

## 6. Create the Second Tab: Service

Now create the second required dashboard tab.

### Step 5 — Add a New Tab

Add another dashboard tab.

### Step 6 — Choose the Correct Template for Service

Select the **2 × 2 rectangle template**.

This template must contain:

- top-left panel
- top-right panel
- bottom-left panel
- bottom-right panel

### Step 7 — Rename the Tab

Rename this tab to:

```text
Service
```

---

## 7. Build the Service Dashboard

The Service dashboard must contain **four visualizations**.

---

### Panel 1 — Number of Recalls by Model

In the **top-left panel**, create a **column chart** showing the **number of recalls by model**.

#### Required result

- Category: **Model**
- Measure: **Number of Recalls**
- Visualization type: **Column chart**

#### How to do it

1. Drag **Model** into the first panel
2. Drag the recall measure into the same panel
3. Ensure the chart type is **Column**

This chart should compare recall volume across car models.

---

### Panel 2 — Customer Sentiment Treemap

In the **top-right panel**, create a **treemap** comparing customer sentiment.

#### Required result

- Category: **Sentiment** (Positive, Neutral, Negative)
- Measure: sentiment count / review count
- Visualization type: **Treemap**

#### How to do it

1. Drag **Sentiment** into the second panel
2. Drag the sentiment count field into the same panel
3. Change the visualization type to **Treemap**

This chart should clearly compare **Positive**, **Neutral**, and **Negative** customer reviews.

---

### Panel 3 — Quantity Sold per Month Compared to Profit

In the **bottom-left panel**, create a **line and column chart**.

#### Required result

- Category: **Month**
- Measures:
  - **Quantity Sold**
  - **Profit**
- Visualization type: **Line and column chart**

#### How to do it

1. Drag **Month** into the third panel
2. Drag **Quantity Sold** into the same panel
3. Drag **Profit** into the panel as a second measure
4. Change the chart type to **Line and Column**

Typically, Cognos will show one measure as columns and the other as a line.

This panel is meant to compare sales volume and profit over time.

---

### Panel 4 — Number of Recalls by Affected System and Model

In the **bottom-right panel**, create a **heat map** showing the number of recalls by **Affected System** and **Model**.

#### Required result

- One axis: **Affected System**
- Other axis: **Model**
- Measure: **Number of Recalls**
- Visualization type: **Heat map**

#### How to do it

1. Drag **Affected System** into the fourth panel
2. Drag **Model** into the same panel
3. Drag the recall count measure as the value
4. Change the visualization type to **Heat map**

This chart helps identify outliers, such as a particular model having many recalls in a specific system.

---

## 8. Check Your Dashboard Against the Expected Output

Before exporting the dashboard, verify the following carefully.

### Sales tab checklist

- The tab is named **Sales**
- The layout is **4 small panels + 1 large panel**
- Panel 1 = **Profit KPI**, formatted in **millions**, **1 decimal place**
- Panel 2 = **Quantity Sold KPI**
- Panel 3 = **Quantity Sold by Model** as a **bar chart**
- Panel 4 = **Average Quantity Sold KPI**
- Panel 5 = **Profit by Dealer ID** as a **column chart**, **sorted ascending**

### Service tab checklist

- The tab is named **Service**
- The layout is **2 × 2**
- Panel 1 = **# of Recalls by Model** as a **column chart**
- Panel 2 = **Customer Sentiment** as a **treemap**
- Panel 3 = **Quantity Sold per Month compared to Profit** as a **line and column chart**
- Panel 4 = **# of Recalls by Affected System and Model** as a **heat map**

If all of these are present, your dashboard should satisfy the main grading criteria.

---

## 9. Export the Dashboard as PDF

Once both tabs are complete, export the dashboard.

### Step 8 — Open the Share Menu

On the toolbar of the dashboard page:

1. Click the **Share** icon

### Step 9 — Use the Export Tab

1. Open the **Export** tab
2. Check the option:

```text
Include filters
```

3. Click **Export**

### Step 10 — Save as PDF

When the print window appears:

1. In **Destination**, select:

```text
Save as PDF
```

2. Save the file locally, preferably in your **Downloads** folder

This PDF is the file you will upload to Coursera.

---

## 10. What If PDF Export Does Not Work?

If Cognos does not let you export the dashboard as a PDF, the assignment allows a fallback solution.

You can:

- take screenshots of both dashboard tabs
- submit those screenshots instead of the PDF

So even if the export fails, you can still complete the assignment successfully.

---

## 11. Main Grading Criteria

According to the assignment, the dashboard is mainly graded on four points:

1. **Have the correct tabs been created?**
2. **Have you captured the correct metrics?**
3. **Are the results correct?**
4. **Have you used the appropriate visualizations?**

This means that accuracy of structure and chart type matters more than cosmetic perfection.

---

## 12. Practical Advice to Pass Smoothly

Here are a few practical suggestions that help avoid mistakes during the exam:

### 1. Rename the tabs immediately
Do not leave the default tab names. Rename them to **Sales** and **Service** as soon as you create them.

### 2. Double-check the chart type
Cognos sometimes guesses a visualization automatically, but it may not be the one requested. Always verify the required chart type manually.

### 3. Watch the aggregation
For KPI cards, Cognos may default to **Sum**. In Panel 4 of Sales, you must explicitly switch **Quantity Sold** to **Average**.

### 4. Verify sorting
The **Profit by Dealer ID** chart must be sorted in **ascending order**. This is easy to forget.

### 5. Keep the layout faithful to the instructions
Even if another design looks prettier, use exactly the templates required by the assignment.

---

## 13. Reference Outcome

If your dashboard is correct, it should broadly resemble the following final structure:

### Sales tab
- Profit KPI in millions
- Quantity Sold KPI
- Quantity Sold by Model bar chart
- Average Quantity Sold KPI
- Profit by Dealer ID column chart

### Service tab
- # of Recalls by Model column chart
- Customer Sentiment treemap
- Profit and Quantity Sold by Month line/column chart
- # of Recalls by Affected System and Model heat map

If your final dashboard matches this structure, you are very likely to pass the assignment.

---

## 14. Final Conclusion

This final exam is not especially difficult once you understand that it is mainly a **dashboard construction task** rather than a theoretical test.

To pass it successfully, focus on three things:

- choosing the **correct template** for each tab
- placing the **correct metric** into each panel
- ensuring the **visualization type and formatting** match the instructions exactly

Once that is done, export the dashboard as PDF and submit it.

---

## 15. Suggested Repository Title

If you want to publish this on GitHub as one of your case studies, a good title could be:

```text
How to Pass the IBM Cognos Analytics Final Assignment – Part 2 | Step-by-Step Case Study
```

Or, if you prefer a shorter version:

```text
IBM Cognos Final Dashboard Exam – Step-by-Step Guide
```

---

## 16. Suggested GitHub Intro Paragraph

You may also use the following introductory paragraph at the top of your repository or README:

> In this case study, I explain step by step how to complete the Final Assignment – Part 2 of the IBM Data Engineering course module *BI Dashboards with IBM Cognos Analytics and Google Looker*. The assignment requires the creation of two dashboards in IBM Cognos Analytics, named **Sales** and **Service**, using the sample **Auto group data module**. Below, I reconstruct the entire process in a precise and reproducible way.

---

## 17. Suggested Tags

```text
IBM Data Engineering, Cognos Analytics, Dashboard, Business Intelligence, Coursera, Case Study, Data Visualization, KPI, Treemap, Heat Map
```
