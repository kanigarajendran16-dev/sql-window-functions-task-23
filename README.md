# 📊 SQL Window Functions - Task 23

## VEDA TECHNOLOGY - Data Analytics Internship

This project was completed as part of the VEDA Technology Data Analytics Internship - Task 23.

The project focuses on understanding and implementing SQL Window Functions for business-oriented sales analysis.

---

## 👨‍💻 Student Details

**Name:** R. Kaniga  
**Course:** B.Tech - Artificial Intelligence and Data Science  
**Department:** ARTIFICIAL INTELLIGENCE AND DATA SCIENCE  
**College:** Muthayammal Engineering College  
**Academic Period:** 2025 - 2029  
**Internship:** VEDA TECHNOLOGY  
**Task:** Task 23 - SQL Window Functions Intro  
**Platform:** Google Colab  

---

## 🎯 Objective

The main objective of this task is to learn and apply SQL Window Functions for analytical business questions.

The project demonstrates:

- ROW_NUMBER()
- RANK()
- DENSE_RANK()
- LAG()
- Running Total
- Moving Average
- Category Ranking
- Top 3 Products
- Sales Difference
- Sales Percentage Change
- Above/Below Average Analysis

---

## 🛠️ Technologies Used

- Python
- SQL
- SQLite
- Pandas
- NumPy
- Matplotlib
- Google Colab
- Excel
- GitHub

---

## 📂 Dataset

A custom sales dataset was created for this project.

### Dataset Columns

| Column | Description |
|---|---|
| Order_ID | Unique order identifier |
| Order_Date | Date of the order |
| Region | Sales region |
| Category | Product category |
| Product | Product name |
| Quantity | Quantity sold |
| Sales | Sales amount |

The dataset contains 100 sales records.

---

## 🔎 SQL Window Functions

### 1. ROW_NUMBER()

Assigns a unique sequential number to each row within a partition.

```sql
ROW_NUMBER() OVER(
    PARTITION BY Region
    ORDER BY Sales DESC
)
