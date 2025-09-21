# Data-Visualization  
Olist E-commerce Analytics  

Olist is a Brazilian e-commerce marketplace that connects small businesses with major online platforms.  
This repository contains a **data analytics project** for the Olist e-commerce dataset (orders, customers, sellers, products, reviews, payments, geolocation).  

The goal is to perform **sales and logistics analytics**: customer behavior, seller activity, order statistics, payment types, delivery times, product categories, and review scores.  

---

## ERD Diagram  

![ERD](images/erd.png)  

---

## Dataset  

Files (CSV) used in the project (stored in `archive/`):  

- `orders.csv` — order details and timestamps  
- `customers.csv` — customer demographic and location data  
- `sellers.csv` — seller information  
- `products.csv` — product metadata and categories  
- `order_items.csv` — products included in orders  
- `order_payments.csv` — payments and methods used  
- `order_reviews.csv` — reviews and ratings from customers  
- `geolocation.csv` — customer and seller locations  
- `category_translation.csv` — translation of product categories into English  

---

## Contents of the repository  

- `schema.sql` — CREATE TABLE statements for all tables (with primary and foreign keys)  
- `queries.sql` — 10 analytical SQL queries (with comments)  
- `main.py` — Python script to connect to the DB and run sample queries  
- `requirements.txt` — Python dependencies  
- `archive/` — CSV files (not included in repo if large)  
- `images/` — ER diagram and screenshots of query results  
- `data.sql` — SQL commands to import CSV files into PostgreSQL  

---

## Quick setup & run instructions  

### 1. Prerequisites  
- macOS / Linux / Windows  
- PostgreSQL 16 (or compatible) installed and running  
- pgAdmin (optional, for GUI and ERD)  
- Python 3.12+  
- Git and optionally the GitHub CLI (`gh`)  

---

### 2. Create virtual environment and install dependencies  
```bash
# in project folder
python3 -m venv venv
source venv/bin/activate    # macOS / Linux
# Windows PowerShell:
.\venv\Scripts\Activate.ps1

pip install -r requirements.txt
