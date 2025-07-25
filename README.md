# Indian-General-Elections-2024-Constituency-Level-Analytics-Dashboard

This project is an ongoing end-to-end data analysis and business intelligence solution that explores the **2024 Indian Lok Sabha (Parliamentary) Election results**. It leverages **SQL** for data modeling and querying, and **Power BI** for dynamic, interactive visual storytelling across 543 constituencies.

## 📌 Objective 

To build a powerful, data-driven dashboard that enables stakeholders to:
- Analyze **party-wise** and **alliance-wise** performance (NDA, I.N.D.I.A., Others)
- Explore **state-level** and **constituency-level** results
- Compare **EVM vs postal vote distributions**
- Identify **top candidates**, **winning margins**, and **voter trends**

## 🧰 Tools & Technologies 

- **SQL Server** – for data cleaning, joins, window functions, aggregations
- **Power BI** – for dashboarding, DAX measures, drill-throughs, filters
- **CSV Dataset** – including 5000+ rows across state, constituency, party, and candidate data

## 🏗️ Dataset & Schema

- `constituencywise_results.csv`: Candidate-wise results including margin, total votes, and winning status
- `partywise_results.csv`: Alliance mapping, party performance, and total seats won
- `statewise_results.csv`: Mapping between constituencies and states
- SQL joins were created across these tables to allow meaningful analysis via Power BI

## 📊 Key Features

- **Landing Page Dashboard**: National-level summary including total seats, alliance performance, and map-based filters
- **Alliance Analysis**: Breakdown of seat share by NDA, I.N.D.I.A., and Others (with custom `party_alliance` field in SQL)
- **State-Wise Drilldown**: Use slicers to explore region-specific results
- **Top Candidates Module**: Identify candidates with the highest EVM votes and winning margins
- **EVM vs Postal Vote Split**: Vote-type distribution across select constituencies
- **Runner-up vs Winner Analysis**: Using window functions in SQL to determine 1st and 2nd positions
- **Custom DAX Measures**: For total seat aggregation, vote margin groups, and dynamic titles

## 🧠 Sample SQL Operations

- Created derived columns like `party_alliance` for classification into NDA, I.N.D.I.A., and Others
- Used `JOIN`, `CASE`, and `ROW_NUMBER()` to determine rankings and top performers
- Aggregated vote counts, party seats, and state-level summaries
