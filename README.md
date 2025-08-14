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
<img width="1302" height="878" alt="image" src="https://github.com/user-attachments/assets/56538e62-db17-4f27-8524-66588695774c" />
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

---

## ▶️ How to Use
1. **Open** `Covid19_Insights.pbix` in **Power BI Desktop**
2. Use the **Date** and **Country** slicers to filter views
3. Switch between **Overview** and **Map** tabs for trends vs. spatial insights
4. Hover over visuals for detailed tooltips; click bars/points to cross-filter

---

## 📈 Example Observations (from the sample state)
- **Total Cases:** 54M | **Total Deaths:** 3M | **CFR:** 6.28% | **Highest Daily New Cases:** 89K  
- **Trends:** Rapid global escalation Mar–Apr 2020  
- **Top-10s:** Vary by metric; **CFR leaders** differ from **total cases leaders**  
- **Map:** Hotspots concentrated in **Europe**, **North America**, **South Asia**

> Replace these numbers with your latest refresh if your dataset updates.

---

## 🧪 Method Notes
- Outlier handling and safe division used for CFR to avoid divide-by-zero errors
- Visuals designed for **scanability** and **comparability** (Top-10 lists, treemap, KPIs)
- Map uses proportional markers to reflect **relative severity**

---

## ⚠️ Limitations
- CFR depends on **testing coverage** and **reporting quality**; compare cautiously
- Time windows and data refresh frequency may affect currentness
- Per-capita comparisons require population-normalized views (future enhancement)

---

## 🚀 Roadmap / Future Work
- Normalize by population (cases/deaths **per 100k**)
- Add **vaccination** metrics & overlays
- Include **mobility** or **policy stringency** indices for context
- Advanced **forecasting** or growth-rate analytics
- Drill-through pages for **country profiles**

---

## 📸 Screenshots
> Add your images to `/assets` and update the links below.

![Overview Dashboard](assets/overview_screenshot.png)
![Map – Global Spread & Severity](assets/map_screenshot.png)

---

## 👤 Author
**Emmanuel Ikechukwu Osuagwu**  
*Data Analyst — interactive dashboards, KPI design, and geographic analytics.*

- LinkedIn: *(add link)*
- Email: *(add email)*

---

## 📄 License
This project is licensed under the **MIT License** (or your preferred license). Add `LICENSE` file if applicable.

