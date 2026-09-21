# RedFlag: The Fraud Files 
> **Pure SQL Fraud Detection Engine for PayFast Transaction Logs**[cite: 1]

---

## 📌 Executive Summary

This project implements a complete, pure SQL fraud analytics engine to monitor, analyze, and detect financial crime across high-volume digital payments—built without 
machine learning or Python dependencies[cite: 1]. 

Working with six months of raw ledger data from **PayFast** (a payment aggregator handling 200,000 transactions per day), this repository contains the queries required 
to isolate **12 distinct fraud archetypes** from legitimate user traffic[cite: 1].

---

## ⚡ Key Highlights & Metrics

* **Core Deliverable:** A unified, production-ready SQL script designed to identify complex fraud patterns on sight[cite: 1].
* **No ML / Pure SQL:** Solves complex behavioral anomalies using window frames, sliding intervals, cohort aggregations, and CTEs[cite: 1].
* **Data Scale:** Analyzes **200,000 transactions** spanning January 1, 2024 to June 30, 2024[cite: 2].
* **Entity Coverage:** Monitors **~14,500 legitimate users**, flags **255+ suspect bad actors**, and audits **800 merchants** across 12 business categories[cite: 2].
* **Real-World Fintech Scope:** Modeled directly after transactional monitoring operations at top payment firms (PhonePe, Razorpay, CRED, Slice)[cite: 1].

---

## 🗂️ Data Foundation at a Glance

All detection models run against the core `transactions` relation[cite: 2]:

* **Volume & Value:** Ticket sizes ranging from ₹1 to ₹1,00,000 across UPI, Cards, Netbanking, and Wallets[cite: 2].
* **Geographic Scope:** Multi-city transaction logs spanning 20 major Indian urban centers to detect location-hopping anomalies[cite: 2].
* **Transaction Lifecycle:** Granular status checks (`SUCCESS` vs. `FAILED`) and direction flow tracking (`DEBIT`, `CREDIT`, `REFUND`) to surface card testing and refund abuse[cite: 2].

---

