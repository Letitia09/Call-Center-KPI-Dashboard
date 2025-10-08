# 📞 Call-Center-KPI-Dashboard (Tableau)
## 🎯 Project Overview
This project focuses on building a monthly performance dashboard for a call center using Tableau Desktop.
The goal is to help managers monitor agent efficiency, call volume, resolution rate, and customer satisfaction — all from a single, interactive view.

---
## 📊 Dataset Description
The dataset simulates real-world call center operations, containing information about call handling performance for multiple agents across several months.
| Column                    | Description                               |
| ------------------------- | ----------------------------------------- |
| **Call ID**               | Unique identifier for each call           |
| **Agent**                 | Employee handling the call                |
| **Date**                  | Date of the call                          |
| **Time**                  | Time when the call came in                |
| **Topic**                 | Purpose or category of the call           |
| **Answered (Y/N)**        | Whether the call was answered             |
| **Resolved (Y/N)**        | Whether the issue was resolved            |
| **Speed of Answer (sec)** | Time taken to answer the call             |
| **Avg Talk Duration**     | Duration of the call (mm:ss)              |
| **Satisfaction Rating**   | Customer rating (1 = Poor, 5 = Excellent) |

---

## Sample (first 5 rows):
| Call ID | Agent | Date       | Time     | Topic           | Answered | Resolved | Speed of Answer (s) | Avg Talk Duration | Satisfaction Rating |
| ------- | ----- | ---------- | -------- | --------------- | -------- | -------- | ------------------- | ----------------- | ------------------- |
| ID0018  | Becky | 2021-01-01 | 11:57:07 | Admin Support   | N        | N        | –                   | –                 | –                   |
| ID0015  | Becky | 2021-01-01 | 11:55:41 | Admin Support   | Y        | Y        | 48                  | 0:03:47           | 4                   |
| ID0016  | Becky | 2021-01-01 | 11:55:41 | Admin Support   | Y        | Y        | 63                  | 0:05:26           | 2                   |
| ID0005  | Becky | 2021-01-01 | 10:00:29 | Payment Related | Y        | Y        | 95                  | 0:01:00           | 3                   |
| ID0044  | Becky | 2021-01-01 | 14:47:02 | Payment Related | Y        | Y        | 98                  | 0:03:14           | 5                   |

---

## 📈 Dashboard Features
| Section                       | Insight                                          | Visualization                         |
| ----------------------------- | ------------------------------------------------ | ------------------------------------- |
| **Call Volume During Week**   | Identifies busiest days of the week              | Bar chart with average reference line |
| **Inbound Calls Today**       | Shows daily call count and average talk duration | KPI Card                              |
| **Resolution Rate (Monthly)** | Displays percentage of issues resolved           | KPI Card                              |
| **Satisfaction Rating**       | Distribution of customer satisfaction (1–5)      | Bar Chart                             |
| **Speed of Answer by Agent**  | Median speed of answer per agent                 | Highlight Table (color-coded)         |
| **Resolution Rate by Agent**  | Agent efficiency based on resolved %             | Highlight Table (color-coded)         |
| **Resolved Calls by Agent**   | Workload comparison per agent                    | Highlight Table (color-coded)         |

---
## 🧠 Key Insights
- **Resolution Rate:** 70.47% overall — below the target benchmark of 85%.
- **Call Volume Peaks:** Highest on Monday–Thursday, suggesting mid-week staffing optimization.
- **Speed of Answer:** Agents with median response times under 65 seconds performed best.
- **Satisfaction Ratings:** Majority of ratings are 3–5, showing moderate customer satisfaction.
- **Agent Analysis:** Top performers – Martha, Stewart; underperformers – Dan, Joe (based on resolution %).
---
## 🎨 Design & Interactivity
- Unified color palette (Blue–Green diverging: Green = High performance, Blue = Low).
- Added reference lines for SLA targets (e.g., 85% resolution goal).
- Used boolean filters and LOD expressions for dynamic month selection.
- Dashboard layout optimized for executive overview (3×2 grid of KPIs and performance visuals).
---
## 🧰 Tools & Technologies
- Visualization: Tableau Desktop
- Data Cleaning: Tableau Prep / Tableau Calculated Fields
- Language: SQL-style expressions within Tableau (DATEPART)
- Dataset Format: CSV

## 🏷️ Tags
#Tableau #DataVisualization #Dashboard #OperationalAnalytics #CallCenterData #KPIDashboard
