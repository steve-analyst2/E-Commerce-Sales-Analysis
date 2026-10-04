# Business Questions

## Purpose

Before cleaning and analyzing the e-commerce dataset, I first reviewed the available fields to understand the information contained in the data and what business problems could reasonably be investigated.

The analysis was then guided by five key business questions. Defining these questions before data cleaning helped determine which fields required particular attention during data preparation, validation, and analysis.

## Key Business Questions

### 1. How has sales performance changed over time?

**Purpose:**  
To examine monthly sales performance and identify changes, peaks, declines, and overall sales patterns across the available time period.

**Key fields required:**
- Order Date
- Total Sales / Clean Total Sales

---

### 2. Which product categories generate the highest sales?

**Purpose:**  
To compare sales contribution across product categories and identify the categories generating the greatest sales value.

**Key fields required:**
- Product Category
- Total Sales / Clean Total Sales

---

### 3. Which products are the top performers by sales?

**Purpose:**  
To identify the individual products contributing the highest sales value and determine which products are major sales drivers.

**Key fields required:**
- Product Name
- Total Sales / Clean Total Sales

---

### 4. Which countries generate the highest sales?

**Purpose:**  
To compare sales performance across countries and identify geographic markets contributing the greatest sales value.

**Key fields required:**
- Country
- Total Sales / Clean Total Sales

---

### 5. What is the distribution of orders by delivery status?

**Purpose:**  
To understand how orders are distributed across delivery outcomes such as Delivered, Shipped, Processing, Returned, Cancelled, and Unknown.

**Key fields required:**
- Order ID
- Delivery Status

---

## How the Questions Guided Data Preparation

The business questions provided direction for the cleaning process.

For example:

- **Order Date** needed to be standardized before analyzing sales trends over time.
- **Product Category** and **Product Name** needed consistent naming before comparing product performance.
- **Country** required standardization before geographic sales analysis.
- **Total Sales** required validation because some recorded values did not match the expected sales calculation.
- **Order ID** required validation before being used to measure valid orders.
- **Delivery Status** required standardization before comparing order outcomes.

This approach ensured that data cleaning was connected to the analytical objectives of the project rather than being performed without a defined business purpose.