# 📊 KPI Definitions

This document outlines the key metrics used in the **Marketing Campaign Dashboard**.

---

### 👥 Total Customers

**Definition:**
Count of distinct customers in the dataset.

**DAX:**

```dax
Total Customers = DISTINCTCOUNT(MarketingData[ID])
```

---

### 📩 Avg. Campaign Acceptance

**Definition:**
Average number of campaigns accepted by each customer.

**DAX:**

```dax
Avg Campaign Acceptance =
AVERAGE(MarketingData[Total_Campaigns_Accepted])
```

---

### 💰 Avg. Customer Spend

**Definition:**
Average of total amount spent across all product categories.

**DAX:**

```dax
Avg Customer Spend =
AVERAGE(MarketingData[Total_Spend])
```

---

### ⏳ Recent Inactivity

**Definition:**
Number of days since the customer last engaged with the platform.

**Field Used:** `Recency`

**Insight:**
Lower `Recency` = more recent engagement

---

> ⚡ These KPIs form the core performance indicators that help understand customer behavior and campaign success.
