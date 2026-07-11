# SpendDNA – Financial Fingerprint Analysis

# 📌 Overview

This project analyzes a real-world styled bank transaction dataset to extract meaningful financial insights, user spending behavior, and lifestyle patterns. It transforms raw, unstructured transaction data into a clean, structured, and analytics-ready format using Python and Pandas.

The system mimics a fintech-grade personal finance analyzer by implementing multiple data processing and analytical features.

---

## 📂 Dataset Description

The dataset contains **6 months of bank transactions (Jan–Jun 2024)** with the following fields:

* **Date** – Transaction date (multiple formats)
* **Time** – Time of transaction
* **Description** – Raw transaction details
* **Type** – Debit/Credit (inconsistent formats)
* **Amount** – Transaction amount (₹, commas, mixed formats)
* **Balance** – Account balance after transaction
* **Mode** – Payment method (UPI, NEFT, etc.)
* **Ref** – Unique transaction reference ID

---

## ⚙️ Key Features

### 🔹 1. Transaction Parser

* Cleans and standardizes raw data
* Handles multiple date formats
* Converts currency strings into numeric values
* Removes duplicates
* Normalizes transaction types (debit/credit)

---

### 🔹 2. Vendor Extractor

* Identifies and standardizes merchant names
* Uses keyword-based mapping
* Detects:

  * E-commerce platforms
  * Food delivery apps
  * Transport services
  * P2P transfers
  * ATM withdrawals

---

### 🔹 3. Category Tagger

* Maps vendors into meaningful categories:

  * Food Delivery
  * Transport
  * Ecommerce
  * Investments
  * Utilities
  * Subscriptions
  * and more
* Handles uncategorized transactions safely

---

### 🔹 4. Spending Overview

* Total credits & debits
* Net savings & savings rate
* Top spending categories
* Top vendors by expenditure

---

### 🔹 5. Monthly Trend Analysis

* Tracks category-wise spending across months
* Identifies:

  * Fastest growing expense category
  * Declining spending patterns
* Uses pivot tables for structured analysis

---

### 🔹 6. Time-of-Day Behavior Analysis

* Analyzes spending patterns across 24 hours
* Detects lifestyle habits such as:

  * Late-night food ordering
  * Morning café spending
* Generates visual activity distribution
  
---

## 🚀 Use Cases

* Personal finance tracking
* Spend behavior analysis
* Fintech product prototyping
* Data cleaning & feature engineering practice
* SQL/Python analytics projects

---

## 🛠️ Tech Stack

* Python
* Pandas
* NumPy

---

## 📈 Outcome

This project demonstrates how raw financial data can be transformed into actionable insights using data cleaning, feature engineering, and analytical techniques—similar to real-world fintech applications like spend analyzers and budgeting tools.
