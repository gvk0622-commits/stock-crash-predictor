# Stock Market Crash Prediction & Asset Management System 📈

A full-stack financial technology ecosystem designed to bridge the gap between passive wealth tracking and proactive, algorithmic risk management. 

This platform allows users to track a diverse portfolio (Equities, Mutual Funds, Real Estate, Bullion) with zero-latency caching, while a background engine autonomously executes recurring investments and monitors systemic market risk.

## 🚀 Core Features
* **Zero-Latency Dashboard:** Engineered an offline-first mobile architecture using **Flutter** and **Hive (NoSQL)**, reducing perceived network latency to <0.1s via a Stale-While-Revalidate caching pattern.
* **Automated Wealth Generation:** Implemented background cron jobs using **APScheduler** to autonomously validate wallet balances, deduct funds, and execute recurring Systematic Investment Plans (SIPs).
* **Algorithmic Fallback Engine:** Bypassed regional API rate-limiting by dynamically calculating physical bullion prices using global futures mathematical conversions and deployed a multi-tier UI fallback system for missing CDN assets.
* **Bank-Grade Security:** Secured transaction execution with **Local Auth** (Biometrics/Face ID) and generated downloadable PDF Tax/P&L statements natively.

## 🛠️ Tech Stack
**Frontend:** Flutter, Dart, Hive (Local Caching), fl_chart (Data Viz), Lottie (Animations)
**Backend:** Python, Flask, PostgreSQL, SQLAlchemy, APScheduler
**Infrastructure & DevOps:** Docker, Render (Serverless Deployment), Git/GitHub
**APIs:** Google Finance (Scraping), Google News RSS, yfinance

## ⚙️ Architecture & Engineering Practices
* **RESTful API Design:** Built secure, decoupled endpoints managing strict relational database schemas (Users, Wallets, Purchases, SIPs).
* **Containerization:** Dockerized the Python/Gunicorn backend to ensure hardware-agnostic, consistent cloud deployment.
* **Algorithmic Problem Solving:** Decomposed complex business logic to handle time-series data aggregation, paginated fetching, and edge-case failure scenarios (e.g., dynamic vector avatar generation upon CDN failure).
