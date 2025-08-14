# 🦠 COVID-19 Insights Dashboard (Power BI)

A two-tab interactive **Power BI** report that turns raw global COVID-19 data into clear, actionable insights on **trends**, **severity**, and **geographic spread**.

> **Tabs**
> 1) **Overview** – KPIs, trends, and Top-10 comparisons  
> 2) **Map** – Global COVID-19 Spread & Severity

---

## 📌 Problem Statement

Large volumes of global COVID-19 data—spread across countries and time—are hard to interpret quickly from raw tables. This makes it difficult to:
- Identify countries with the highest burden of **cases** and **fatalities**
- Monitor **Case Fatality Rate (CFR)** to detect higher-risk regions
- Understand proportionality between **infections vs. deaths**
- Track **geographic spread & severity** and spot emerging hotspots for timely, targeted interventions

This project addresses those gaps with a **KPI-driven** Overview and an **interactive global map** to support evidence-based decisions.

---

## 🧭 Dashboard Structure
<img width="1480" height="960" alt="Screenshot (125)" src="https://github.com/user-attachments/assets/05296292-864d-4892-b295-a7bf83ef85c1" />
<img width="1303" height="813" alt="image" src="https://github.com/user-attachments/assets/e890dea5-581b-4227-b9de-0d1166b6e8e8" />


### 1) Overview
**KPI Cards**
- **Total Cases:** 54M  
- **Total Deaths:** 3M  
- **Case Fatality Rate (CFR):** 6.28%  
- **Highest Daily New Cases:** 89K  

**Visuals**
- Global Trends (Cumulative Cases & Deaths)
- Top 10 Countries by **Total Cases**
- Top 10 Countries by **Total Deaths**
- Top 10 Countries by **CFR (%)**
- **Case Fatality Rate Leaders** (treemap)

**Key Insights**
- Sharp surge in global cases Mar–Apr 2020; deaths follow a similar shape at a lower slope  
- Countries leading in **cases** are not always the leaders in **CFR**, suggesting differences in testing, healthcare capacity, and outbreak stage  
- CFR leaders (e.g., France, Belgium, Italy in the sample) signal regions with higher mortality relative to infections

---

### 2) Map – Global Spread & Severity
**What it shows**
- Worldwide distribution of cases with proportional markers
- Regional hotspots and clusters

**Findings**
- Pandemic presence across nearly all continents
- High-density clusters in **Europe**, **North America**, and **South Asia**
- Several smaller countries/islands show large markers → potentially high **per-capita** rates
- Clear spatial context to guide **resource allocation** and **interventions**

---

## 🎯 Project Objectives
- Convert raw COVID-19 data into **interactive, comprehensible** analytics
- Track & compare **trends** using robust **KPIs** and time-series charts
- Identify **hotspots** and **regional disparities**
- Provide an intuitive **map** for location-based analysis and decision support

---

## 🛠 Tech Stack
- **Microsoft Power BI** (reporting & interactivity)
- Dataset fields used: `date`, `location`, `new_cases`, `new_deaths`, `total_cases`, `total_deaths`, and derived **CFR** measures

> **Note:** CFR (%) = `total_deaths / total_cases * 100` (handled with safe division in DAX)

---

## 📂 Repository Contents
