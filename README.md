SmartRetail Insights: Full-Stack Data Analytics Web App

Project Overview

SmartRetail Insights is a full-stack portfolio-ready analytics platform designed for an e-commerce environment. It combines advanced database design, backend API services, Python-driven data analytics, and a modern dashboard frontend to analyze customer behavior, optimize sales, and forecast trends.


---

Objectives

Perform complex SQL data manipulation and extraction.

Apply Python-based statistical and machine learning analysis.

Integrate Node.js REST APIs for dynamic data access.

Build a secure role-based access dashboard using modern frontend frameworks.

Demonstrate advanced EERD design with analytics-focused schema.



---

Tech Stack


---

Database Schema (EERD Summary)

Core Entities:

Customer, Order, OrderItem, Product, Session, Cart, SearchLog, Discount

Employee, SupportTicket, Transcript


Access Control:

User, Role, AccessControl


Advanced Concepts:

Multivalued Attributes: Customer_Interests

Specialization: PremiumCustomer, RegularCustomer

Weak Entity: Cart

Relationship with Attributes: OrderItem(price_at_time)



---

Backend Design

Framework: Node.js with Express

Endpoints (examples):

/api/customers, /api/orders, /api/analytics/rfm, /api/forecast

Auth routes: /auth/login, /auth/register, protected by JWT


Middlewares:

Authentication: JWT

Authorization: Role-based (admin, support, manager, customer)


Security:

Password hashing with Bcrypt

SQL injection prevention via parameterized queries




---

Python Analytics Engine

Located in python_analysis/


Tasks:

1. RFM Segmentation:

Cluster customers into groups: Loyal, At-risk, New



2. Sales Forecasting:

Time-series using ARIMA or Prophet



3. Behavioral Analytics:

Cart abandonment, product views vs. conversions



4. Support Transcript Analysis:

Basic NLP: word clouds, sentiment classification (optional)




Outputs:

Stored as CSV/JSON + plots as PNG for frontend usage

Triggered via script or scheduled cronjobs



---

Frontend UI Design

Framework Options: Vanilla JS + HTML/CSS or React


Pages:

1. Login / Register


2. Dashboard (Role-based Views):

Admin: Full access

Support: View customers, tickets, transcripts

Customer: Orders, Profile, Interactions

Manager: Analytics and Reports



3. Analytics Tabs:

Customer Segmentation

Sales Forecast

Product Performance

Behavior Heatmaps




Charts:

Bar, Line, Pie (Chart.js or D3.js)

Interactive filters (date range, product category)



---

Folder Structure (Suggestion)

SmartRetailInsights/
├── backend/           # Node.js + Express
│   ├── controllers/
│   ├── routes/
│   ├── middleware/
│   └── models/
├── frontend/          # HTML/CSS/JS or React
│   └── public/
├── python_analysis/   # Python scripts & notebooks
│   └── reports/
├── sql_server/        # DDLs, views, procedures
├── assets/            # Images, EERD PNG, Docs
└── README.md


---

Deliverables

Full SQL Server DB setup (schema + dummy data)

EERD diagram (PNG + SQL)

Backend API with secure routes

Python analysis outputs (charts, tables)

Complete frontend with navigation and graphs

Role-based access control logic

Deployed version (if time permits)



---

Learning Outcomes

Real-world database modeling with advanced normalization

Full-cycle ETL + analytics flow using Python

Secure REST API creation with Node.js

Data visualization and dashboard engineering

End-to-end portfolio project demonstrating system design, development, and analytics



---

Let me know when to start building out each part and I’ll help you step by step!

