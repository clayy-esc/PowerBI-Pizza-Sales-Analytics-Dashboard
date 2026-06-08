<p align="center">
  <img src="images/pizza_sales_analytics_dashboard.png" width="800">
</p>

<h1 align="center">🍕 Pizza Sales Analytics Dashboard</h1>

<p align="center">
  <strong>A Business Intelligence Dashboard for Analyzing Pizza Sales Performance, Customer Preferences, and Menu Optimization.</strong>
</p>

---

## 📖 Overview

The **Pizza Sales Analytics Dashboard** is a Power BI project designed to transform raw transactional data into meaningful business insights. The dashboard enables stakeholders to monitor sales performance, understand customer purchasing behavior, identify high-performing products, and discover opportunities for menu optimization.

The report follows a business-driven approach where every visualization is designed to answer a specific operational or strategic question.

---

## 🎯 Objectives

### Pizza Sales Overview

| Business Question                             | Purpose                                                  |
| --------------------------------------------- | -------------------------------------------------------- |
| What are the total sales per month?           | Analyze sales trends and seasonality throughout the year |
| What are the total sales for each pizza size? | Evaluate revenue contribution by pizza size              |
| Which category generates the most revenue?    | Identify the strongest performing pizza category         |

### Product Performance Analysis

| Business Question                                                              | Purpose                                            |
| ------------------------------------------------------------------------------ | -------------------------------------------------- |
| What are the Top 5 most bought pizzas?                                         | Identify customer favorites                        |
| What percentage does the most preferred size represent in each pizza category? | Analyze size preference patterns within categories |
| What are the total sales for each pizza?                                       | Measure product-level revenue performance          |
| How many pizzas are sold per size?                                             | Understand customer size preferences               |

### Menu Optimization

| Business Question                                                  | Purpose                                  |
| ------------------------------------------------------------------ | ---------------------------------------- |
| Are there pizzas that should be removed from the menu or promoted? | Evaluate menu effectiveness              |
| Which pizzas may need promotional support or removal?              | Identify underperforming products        |
| Which pizzas generate the most revenue per unit sold?              | Discover premium and high-value products |

---

## 📅 Data Scope

| Attribute        | Details                      |
| ---------------- | ---------------------------- |
| Reporting Period | January 2015 – December 2015 |
| Industry         | Food & Beverage              |
| Dataset Type     | Transactional Sales Data     |
| Dashboard Layout | Desktop View Only            |

---

## 🗂 Dataset

The project consists of four related tables used to model the complete pizza ordering process.

| Table         | Field            | Description                                          |
| ------------- | ---------------- | ---------------------------------------------------- |
| orders        | order_id         | Unique identifier for each order placed              |
| orders        | date             | Date the order was placed                            |
| orders        | time             | Time the order was placed                            |
| order_details | order_details_id | Unique identifier for each pizza transaction         |
| order_details | order_id         | Foreign key linked to orders                         |
| order_details | pizza_id         | Foreign key linked to pizzas                         |
| order_details | quantity         | Quantity ordered                                     |
| pizzas        | pizza_id         | Unique identifier for each pizza                     |
| pizzas        | pizza_type_id    | Foreign key linked to pizza types                    |
| pizzas        | size             | Pizza size (Small, Medium, Large, X Large, XX Large) |
| pizzas        | price            | Pizza price in USD                                   |
| pizza_types   | pizza_type_id    | Unique identifier for each pizza type                |
| pizza_types   | name             | Pizza name shown on the menu                         |
| pizza_types   | category         | Pizza category (Classic, Chicken, Supreme, Veggie)   |
| pizza_types   | ingredients      | Comma-delimited list of ingredients                  |

### Data Model

```text
 Orders
   │
   └── order_id
           │
     Order Details
           │
           └── pizza_id
                   │
                 Pizzas
                   │
                   └── pizza_type_id
                           │
                      Pizza Types
```

---

## 📏 Metrics

The dashboard uses DAX measures to calculate business KPIs.

| Metric                   | Description                                  |
| ------------------------ | -------------------------------------------- |
| Total Revenue            | Total revenue generated from pizza sales     |
| Total Orders             | Total number of customer orders              |
| Total Pizzas Sold        | Total quantity of pizzas sold                |
| Average Order Value      | Average revenue generated per order          |
| Average Pizzas per Order | Average number of pizzas purchased per order |

---

## 📊 Dashboard Views

### 1️⃣ Pizza Sales Overview

Provides a high-level summary of sales performance and customer purchasing activity.

| Visualization         | Business Purpose                                 |
| --------------------- | ------------------------------------------------ |
| KPI Cards             | Executive summary of business performance        |
| Monthly Revenue Trend | Monitor revenue performance throughout the year  |
| Revenue by Pizza Size | Compare revenue contribution by pizza size       |
| Revenue by Category   | Identify the strongest performing pizza category |

---

### 2️⃣ Product Performance Analysis

Focuses on customer preferences and product popularity.

| Visualization                     | Business Purpose                                   |
| --------------------------------- | -------------------------------------------------- |
| Top 5 Best Selling Pizzas         | Identify customer favorites                        |
| Pizza Size Preference by Category | Analyze preferred pizza sizes within each category |
| Sales by Pizza Name               | Evaluate product-level revenue contribution        |
| Most Purchased Pizza Sizes        | Analyze demand distribution across pizza sizes     |

---

### 3️⃣ Menu Optimization

Provides strategic insights for menu improvement and promotional planning.

| Visualization                   | Business Purpose                                             |
| ------------------------------- | ------------------------------------------------------------ |
| Menu Engineering Matrix         | Evaluate products based on popularity and revenue generation |
| Bottom 5 Performing Pizzas      | Identify products that may require promotion or removal      |
| Revenue per Pizza Sold          | Identify premium and high-value products                     |

---

## ⚙️ Development Process

The dashboard was developed following a structured Business Intelligence workflow.

| Phase                        | Description                                                      |
| ---------------------------- | ---------------------------------------------------------------- |
| Data Collection              | Importing and validating source datasets                         |
| Transformation and Modeling  | Data cleaning, relationship creation, and DAX development        |
| Design Blueprint             | Planning dashboard structure and analytical storytelling         |
| Design Aesthetics            | Applying consistent visual design and branding                   |
| Interactivity and Navigation | Implementing filters, slicers, tooltips, and navigation features |

---

## 🔍 Custom Tooltip

A dedicated tooltip page was developed to provide additional context without overcrowding the report pages.

### Availability

The tooltip is available only within selected visualizations on the **Pizza Sales Overview** page.

### Tooltip Information

| Information Displayed |
| --------------------- |
| Pizza Name            |
| Revenue Contribution  |
| Total Revenue         |

This feature enables users to access detailed pizza-level insights while remaining on the current report page.

---

## 🛠 Technologies Used

| Technology       | Purpose                           |
| ---------------- | --------------------------------- |
| Power BI Desktop | Dashboard Development             |
| DAX              | KPI and Measure Calculations      |
| Power Query      | Data Transformation               |
| CSV Files        | Data Source                       |
| GitHub           | Version Control and Documentation |

---

## 📄 Key Insights Delivered

* Sales performance trends throughout the reporting period
* Revenue contribution by pizza category and size
* Customer purchasing preferences
* Top-performing pizza products
* Underperforming menu items
* Menu optimization opportunities
* Premium product identification
* Actionable recommendations for promotions and pricing strategies

---

## 📷 Dashboard Preview

<p align="center">
  <img src="images/pizza_sales_analytics_dashboard.png" width="900">
</p>

---
