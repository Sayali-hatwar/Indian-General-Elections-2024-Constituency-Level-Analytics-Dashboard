# Indian General Elections 2024 – Constituency-Level Analytics Dashboard

This project presents a complete **end-to-end data analysis and business intelligence solution** for the **2024 Indian Lok Sabha (Parliamentary) Election results**. It combines powerful **SQL-based data modeling** with an **interactive Power BI dashboard**, delivering constituency-level insights across 543 seats.
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

<img width="800" height="593" alt="Screenshot (312)" src="https://github.com/user-attachments/assets/3c74a517-755a-4cdb-a26b-7a429578e06e" />

###  Dashboard 2: **State Demographic Analysis**
- State-wise seat distribution with **map charts & tooltips**
- Drill-through to view all constituencies and winners
- Identifies state with highest seats for each alliance

<img width="800" height="599" alt="E1" src="https://github.com/user-attachments/assets/b0828f7a-eec1-481d-b0b9-3d1803e019fe" />

###  Dashboard 3: **Political Landscape by State**
- Filter by any state
- Donut charts for party-wise seat share
- Grid view of all parties and alliances

<img width="800" height="603" alt="Screenshot (314)" src="https://github.com/user-attachments/assets/79e3d60a-5693-4cb8-8f7f-df5c90d8cc87" />

###  Dashboard 4: **Constituency Analysis**
- Deep dive into each constituency
- Shows **total votes**, **EVM vs Postal votes**
- Candidate-level breakdown: Winner, Runner-up, 2nd Runner-up

<img width="800" height="601" alt="Screenshot (315)" src="https://github.com/user-attachments/assets/659effcf-b4aa-4097-99bf-d71036bc1ed6" />

###  Dashboard 5: **Details Grid**
- Exportable grid view of all constituencies
- Includes: votes, margins, alliances, and filter controls

<img width="800" height="603" alt="Screenshot (316)" src="https://github.com/user-attachments/assets/42d236ef-d6f9-46b9-a72d-c107b4503632" />

###  Dashboard 6: **Landing Page**
- Clean UI with navigation buttons
- Home button on every page
- Responsive layout with hover effects

<img width="800" height="605" alt="Screenshot (317)" src="https://github.com/user-attachments/assets/15767f2a-b5c0-492c-9405-689f48cc65d2" />

---

## Summary Executive
### Overview of finding
This project analyzes the Indian General Elections 2024 at the constituency level, providing insights into party performance, winning margins, alliance strength, and voter patterns across states. The dashboard highlights key outcomes such as the dominance of major alliances, close contests in critical constituencies, and shifts in vote share compared to previous elections. These findings not only summarize election results but also demonstrate how interactive dashboards can simplify large-scale, complex datasets into actionable insights, making it valuable for researchers, political analysts, journalists, and citizens interested in understanding election dynamics.[here](https://drive.google.com/open?id=1qqRn5y4LEZ_HPxAn67aHvz9KsqNy_3JB&usp=drive_fs)

---
Check out the Dashboard -

*(.ppt file)* - [here](https://1drv.ms/p/c/8a0e9e1df0bcd847/EYmSWrhYVPROpCNCsnNTJLIBZ9scsZ6T1O_FjaYtO12g6Q?e=mhgCqf)

*(.pbix file)* - [here](https://app.powerbi.com/links/6jFhRmNZIB?ctid=3fc1a503-a415-43d0-a42c-0c46da001df4&pbi_source=linkShare&bookmarkGuid=cadce831-093e-446c-82bb-ad53f14b6557)
