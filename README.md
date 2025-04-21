# 🚕 Ride-Sharing Company Analytics — SQL Project

A complete SQL-based analytics project for a fictional ride-sharing company, designed to uncover customer trends, driver performance, revenue insights, and operational metrics.

---

## 📌 Project Overview

This project simulates a ride-sharing company’s database and provides **25 insightful SQL queries** to analyze customer behavior, revenue streams, and performance KPIs. Ideal for practicing SQL skills as a data analyst or showcasing in a portfolio.

---

## 🗂️ Database Schema

### 🧑‍💼 `customers`
| Column        | Type    | Description         |
|---------------|---------|---------------------|
| customer_id   | INT PK  | Unique customer ID  |
| name          | VARCHAR | Customer name       |
| gender        | VARCHAR | Male/Female/Other   |
| age           | INT     | Customer age        |
| city          | VARCHAR | City of residence   |
| signup_date   | DATE    | Date of signup      |

### 🚗 `drivers`
| Column        | Type    | Description        |
|---------------|---------|--------------------|
| driver_id     | INT PK  | Unique driver ID   |
| name          | VARCHAR | Driver name        |
| gender        | VARCHAR | Driver gender      |
| rating        | DECIMAL | Driver rating      |
| car_type      | VARCHAR | Sedan, Hatchback…  |
| city          | VARCHAR | Operating city     |
| joined_date   | DATE    | Join date          |

### 🛺 `rides`
| Column          | Type      | Description                   |
|-----------------|-----------|-------------------------------|
| ride_id         | INT PK    | Ride identifier               |
| customer_id     | INT FK    | Who booked the ride           |
| driver_id       | INT FK    | Who completed the ride        |
| pickup_time     | DATETIME  | When ride started             |
| drop_time       | DATETIME  | When ride ended               |
| pickup_location | VARCHAR   | Start location                |
| drop_location   | VARCHAR   | End location                  |
| distance_km     | DECIMAL   | Ride distance                 |
| fare_amount     | DECIMAL   | Fare collected                |
| ride_status     | VARCHAR   | Completed, Cancelled, No-show |

### 💳 `payments`
| Column         | Type      | Description         |
|----------------|-----------|---------------------|
| payment_id     | INT PK    | Payment identifier  |
| ride_id        | INT FK    | Linked ride         |
| payment_method | VARCHAR   | Card, Wallet, Cash  |
| payment_status | VARCHAR   | Success / Failed    |

---

## 📊 25 SQL Queries with Insights

✅ Explore revenue, customer trends, driver ratings, payment preferences, and more!

Examples include:
- Total completed rides
- Revenue per city
- Most used payment method
- Peak ride hours
- Driver earnings leaderboard

➡️ **[Download All 25 SQL Queries & Insights (PDF)](Ride_Sharing_SQL_Project_Queries.pdf)**

---

## 📈 Visualization Ideas (Power BI / Tableau)

- **City-wise Heatmap of Rides**
- **Revenue Over Time**
- **Ride Status Funnel**
- **Top Performing Drivers**
- **Payment Method Distribution**
- **Repeat Customer Retention**

---

## 🚀 How to Use

1. Clone this repo
2. Load mock data (if using provided CSVs)
3. Run SQL queries in MySQL/PostgreSQL
4. Create dashboards using your favorite BI tool

--
