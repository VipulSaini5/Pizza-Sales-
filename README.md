# 🍕 Pizza Sales Analytics: SQL Slicing & Dicing 🔍

## Data - Kaggle(https://www.kaggle.com/datasets/keremkarayaz/coffee-shop-sales/data)

## 🚀 Project Overview

Dive into the store of a Pizza outlet sales with this SQL-powered analytics project! Uncover the secret ingredients of business success through data-driven insights.

## 🌟 Key Features

- **Order Insights**: Track total orders and peak hours
- **Revenue Analysis**: Calculate total and cumulative revenue
- **Product Performance**: Identify top-selling and highest-priced pizzas
- **Customer Preferences**: Analyze favorite sizes and types
- **Category Breakdown**: Explore sales distribution across categories

## 📊 Sample Insights

1. 🏆 **Top 3 Revenue Generators**
2. 📈 **Hourly Order Trends**
3. 💰 **Revenue Contribution by Pizza Type**
4. 📏 **Most Popular Pizza Sizes**
5. 🍽️ **Average Daily Pizza Orders**

## 🛠️ Tech Stack

- MySQL

## 🔍 Data Deep Dive

Our analysis spans multiple database tables:

- `orders`: The heart of our sales data
- `order_details`: The nitty-gritty of each order
- `pizzas`: Our delicious product lineup
- `pizza_types`: Categories and flavors galore

## 🧮 Analytical Challenges Tackled

1. **Total Order Count**:
      `SELECT COUNT(order_id) FROM orders;`
2. **Revenue Calculation**: 
      `SELECT ROUND(SUM(order_details.quantity * pizzas.price), 2) AS total_sales
       FROM order_details
       JOIN pizzas ON pizzas.pizza_id = order_details.pizza_id;

