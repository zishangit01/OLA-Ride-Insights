# 🚕 OLA Ride Insights – Power BI & SQL Analytics

## 🎥 Live Project Demo

▶️ **Full Walkthrough Video**  
[Watch Dashboard Walkthrough](OLA_Ride_Insights/Video_Demo/demo.mp4)





---

## 📌 Project Overview
This project analyzes OLA ride booking data to identify why rides fail, where revenue is lost, and how operational risk impacts business performance.

The goal is not just reporting, but to build a **revenue protection and operational intelligence system** using SQL, Excel and Power BI.

---

## 🎯 Business Problems
OLA faces four critical challenges:
- High ride cancellation rate
- Revenue leakage due to failed rides
- Peak hour service breakdown
- Driver and customer dissatisfaction

This project focuses on:
- Improving ride success rate  
- Reducing driver and customer cancellations  
- Optimizing payment and vehicle performance  
- Identifying high-risk time periods and locations  

---

## 📊 Dataset Summary

| Metric | Value |
|--------|-------|
| Time Period | July 2024 |
| Total Bookings | 103,024 |
| Successful Rides | 63,967 |
| Cancelled Rides | 28,933 |
| Cancellation Rate | ~28% |
| Total Booking Value | ₹35 Million |
| Revenue Lost | ₹15.95 Million |

---

## 🧹 Data Cleaning & Preparation
Raw data contained:
- Date and time stored as text
- Mixed cancellation flags
- Corrupted UTF-8 column names
- Ratings stored as strings

Cleaning was done using:
- Excel (Power Query + EDA)
- SQL data type conversion
- Creation of a master analytics view (`vw_ola_clean`)

---

## 🧱 SQL Analytics Layer

Power BI is connected to **SQL Views**, not raw tables.

Architecture:

Key SQL views:
- vw_overall_kpi  
- vw_daily_rides  
- vw_hourly_cancellation  
- vw_vehicle_risk  
- vw_payment_method  
- vw_driver_cancellations  
- vw_customer_cancellations  
- vw_ratings  

This ensures fast, reliable and scalable analytics.

---

## 📈 Key Business Insights

### Booking Funnel
Only **62%** of bookings become successful rides.  
**38% fail**, mainly due to driver and customer cancellations.

### Revenue Leakage
Nearly **₹16M** of revenue is lost due to cancelled rides.

### Peak Hour Risk
Peak hours (morning & evening) have the highest cancellation and revenue loss.

### Vehicle Type Risk
All vehicle types have similar cancellation (~28%), proving this is a **platform-wide operational issue**.

### Payment Risk
Cash rides generate high revenue but also have the highest cancellation and fraud risk.

---

## ⭐ Ratings
Average driver and customer ratings are around **4.0**, but high cancellations show ratings only reflect completed rides, not failures.

---

## 📁 Repository Structure

OLA_Ride_Insights
├── Data
│ └── ola_cleaned.csv
├── SQL
│ ├── vw_ola_clean.sql
│ ├── vw_overall_kpi.sql
│ ├── vw_vehicle_risk.sql
│ ├── vw_payment_method.sql
│ ├── vw_driver_cancellations.sql
│ └── vw_customer_cancellations.sql
├── PowerBI
│ └── OLA_Dashboard.pbix
└── Video_Demo
└── demo.mp4

---

## 🏆 Outcome
This project demonstrates how data analytics can:
- Reduce revenue leakage
- Improve customer experience
- Optimize driver operations
- Provide real business intelligence for decision-making

