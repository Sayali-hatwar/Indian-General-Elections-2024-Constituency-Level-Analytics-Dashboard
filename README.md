# 🇮🇳 Indian General Elections 2024 – Constituency-Level Analytics Dashboard

This project presents a complete **end-to-end data analysis and business intelligence solution** for the **2024 Indian Lok Sabha (Parliamentary) Election results**. It combines powerful **SQL-based data modeling** with an **interactive Power BI dashboard**, delivering constituency-level insights across 543 seats.

> ✅ **Status: Completed**

---

##  Objective

To build a robust and insightful election analytics dashboard that enables stakeholders to:
- Analyze **party-wise** and **alliance-wise** performance (NDA, I.N.D.I.A., Others)
- Explore **state-level** and **constituency-level** results
- Compare **EVM vs postal vote** distributions
- Identify **top-performing candidates**, **winning margins**, and **regional trends**

---

##  Tools & Technologies Used

- **SQL Server** – Data cleaning, joining tables, window functions, and aggregations
- **Power BI** – Dashboarding, DAX measures, drill-throughs, bookmarks, filters
- **CSV Datasets** – 5000+ rows covering states, constituencies, parties, and candidates

---

##  Dataset & Schema

| File | Description |
|------|-------------|
| `constituencywise_details.csv` | Candidate-level votes (EVM, Postal, Total) |
| `constituencywise_results.csv` | Constituency-level winning candidate and margin |
| `partywise_results.csv` | Party-wise seat counts + alliance classifications |
| `statewise_results.csv` | Maps each constituency to a state |
| `states.csv` | Master list of all Indian states |
| `India_Election_Result.pbix` | Final Power BI dashboard |

Relational joins were established between these files using keys like `Party_ID`, `Constituency_ID`, and `State_ID` to allow a unified data model in Power BI.

---

##  Key Features & Dashboards

###  Dashboard 1: **Overview Analysis**
- Seat share & % performance of NDA, I.N.D.I.A., and Others
- Grid view tables showing all seats won per alliance
- Interactive bookmarks for quick navigation

###  Dashboard 2: **State Demographic Analysis**
- State-wise seat distribution with **map charts & tooltips**
- Drill-through to view all constituencies and winners
- Identifies state with highest seats for each alliance

###  Dashboard 3: **Political Landscape by State**
- Filter by any state
- Donut charts for party-wise seat share
- Grid view of all parties and alliances

###  Dashboard 4: **Constituency Analysis**
- Deep dive into each constituency
- Shows **total votes**, **EVM vs Postal votes**
- Candidate-level breakdown: Winner, Runner-up, 2nd Runner-up

###  Dashboard 5: **Details Grid**
- Exportable grid view of all constituencies
- Includes: votes, margins, alliances, and filter controls

###  Dashboard 6: **Landing Page**
- Clean UI with navigation buttons
- Home button on every page
- Responsive layout with hover effects

---

##  SQL Operations Performed

- Added custom column `party_alliance` using `CASE` to classify parties as **NDA**, **I.N.D.I.A.**, or **Others**
- Used **`JOIN`**, **`ROW_NUMBER()`**, and **aggregations** to:
  - Rank candidates
  - Find top EVM vote winners
  - Compute seat distributions
- Applied **window functions** to identify runner-up and 2nd runner-up candidates
