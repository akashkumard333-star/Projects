# 🏏 ICC Cricket World Cup 2019 – Performance Analytics Dashboard  
### Interactive Data Visualization & Reporting using Tableau

---

## 🧭 Project Overview

This project presents an **interactive Tableau dashboard** that analyzes team performance, match outcomes, venues, and strategic trends from the **ICC Cricket World Cup 2019**.

The dashboard transforms raw cricket match data into **actionable insights** by visualizing team success, scoring patterns, venue impact, and match strategies such as batting first vs chasing.  
It is designed for **fans, analysts, coaches, and data enthusiasts** to explore tournament trends through dynamic filters and visuals.

🔗 **Tableau Public Dashboard:**  
https://public.tableau.com/app/profile/akash.kumar.dineshkumar/viz/533project/Dashboard1

---
---

## 📊 Tableau Dashboard Preview

_Interactive overview of team performance, venues, match strategies, and outcomes from the ICC Cricket World Cup 2019._

<img
  width="940"
  height="529"
  alt="ICC World Cup 2019 Tableau Dashboard"
  src="https://raw.githubusercontent.com/akashkumard333-star/akashkumard333/ae606f95889e2f604cec21658dd45963a7ee692d/assets/Dashboard.png"
/>

## 🧠 Project Planning & Design (Mural)

This Mural board captures the **end-to-end planning process** for the dashboard, including:
- Phase-wise project planning
- Question formulation and analytical goals
- Visualization selection and chart rationale
- Dashboard layout and interaction design

🔗 **Mural Board:**  
https://app.mural.co/t/team133626/m/team133626/1744656745625/73ea577e98524dd9edb60a81f23e1ae5a9e44445?sender=u326fe82ee130dabcffbc7325

---
## 📊 Key Deliverables

### **1. Interactive Tableau Dashboard**
- Team-wise and venue-wise performance analysis  
- Match strategy insights (bat first vs chase)  
- Innings-wise scoring trends  
- High-scoring venues and successful defenses  

### **2. Dynamic Filters & Controls**
- Team selector (Country)
- Venue selector (Ground)
- Result filter (won / lost / tied / no result)
- Innings filter (1st vs 2nd innings)
- Toss decision filter (bat / field)
- Target score slider (300+ runs analysis)

---

## 📂 Dataset Overview

### **Cricket Match Dataset – ICC World Cup 2019**
Public dataset sourced from Kaggle containing **match-level and performance data** from the 2019 ICC Cricket World Cup.

🔗 Dataset Source:  
https://www.kaggle.com/code/venky73/icc-cricket-world-cup-2019-analysis/input?select=ODI_Match_Totals.csv

**Key attributes include:**
- Team & opposition
- Match result and toss decision
- Scores, overs, runs per over (RPO)
- Venue and match date
- Innings and target score

---

## 🧹 Data Preprocessing & Cleaning

The dataset was cleaned and transformed before visualization to ensure accuracy and consistency:

- Extracted numeric runs from score values (e.g., `250/8 → 250`)
- Converted RPO values from string to numeric format
- Normalized team and opposition names
- Standardized match results (Won, Lost, Tied, No Result)
- Converted match dates to proper Date format
- Removed inconsistencies and null values

These steps enabled reliable aggregations and visual analysis in Tableau.

---

## 🧩 Dashboard Sections & Visualizations

---

## **General Match & Team Performance**
- Which team won the most matches?
- Which team had the highest average score?
- Which team achieved the best win percentage?

**Visuals Used:**
- Horizontal bar charts
- Vertical bar charts
- Donut charts

---

## **Venue & Location-Based Analysis**
- Which venues hosted the most matches?
- Which grounds were high-scoring?
- Which venues favored chasing teams?

**Visuals Used:**
- Bar charts
- Scatter plots
- Grouped bar charts

---

## **Match Strategy Analysis**
- Impact of batting first vs fielding first
- First innings vs second innings scoring patterns
- Teams with the best chasing success rate
- Success rate of defending targets above 300 runs

**Visuals Used:**
- Stacked bar charts
- Side-by-side bar charts
- Line charts
- Pie charts

---

## 🎛 Dashboard Interactivity

The dashboard supports **dynamic exploration** using Tableau controls:

- **Country Filter:** Team-based analysis  
- **Ground Filter:** Venue-specific trends  
- **Result Filter:** Win/loss-focused insights  
- **Innings Selector:** Compare 1st vs 2nd innings  
- **Toss Decision Filter:** Strategic analysis  
- **Target Score Slider:** Analyze 300+ run defenses  

These controls allow users to personalize insights instantly.

---

## 👥 Intended Users

- Cricket coaches and team analysts  
- Sports analysts and statisticians  
- Broadcasters and commentators  
- Data analytics students and researchers  
- General cricket fans  
- Fantasy league players and sports app developers  

---

## 💡 Key Insights Generated

- Identification of top-performing teams
- Win percentage comparison across teams
- High-scoring and chase-friendly venues
- Strategic advantage of batting vs fielding
- Teams most effective while chasing targets
- Defensive success rate for large totals (300+)

---

## 🛠 Tools & Technologies

- **Visualization Tool:** Tableau  
- **Data Processing:** Tableau calculated fields  
- **Data Source:** CSV (Kaggle dataset)  
- **Techniques:** Filtering, aggregation, storytelling, dashboard actions  

---
