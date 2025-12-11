# FUTURE_DS_02
Digital Marketing Analytics – Power BI Project

This project transforms Facebook Ads campaign data into a complete analytics solution. The goal was to clean and structure raw campaign data, calculate key KPIs, and design a clear, actionable Power BI dashboard that delivers real business insights — not just visuals.

Data Preparation (Python / Pandas)

All tables were cleaned and prepared using Python.
Key tasks included:

Fixing missing and inconsistent values

Standardizing date and campaign fields

Aggregating metrics by age, gender, campaign, and interest

Calculating KPIs like CTR, CVR, CPA, CPC, CPM

Creating segments for audience insights (Age × Gender × Interest)

This ensured Power BI receives clean, structured data ready for fast calculations.

Data Model

A simple star schema was used for performance:

Fact table: campaign impressions, clicks, spend, conversions

Dimensions: age, gender, campaign, interests, and date table for time intelligence

DAX Measures

All KPIs in the report were built using optimized DAX measures:

CPA (Cost per Approved Conversion)

CTR % (Click Through Rate)

CVR (Conversion Rate)

CPC (Cost per Click)

CPM (Cost per 1,000 Impressions)

Total Spend, Impressions, Clicks, Conversions

Segmented metrics by Age, Gender, Campaign, Interests

Time intelligence measures for weekly/monthly trends

Dashboard Design

The report layout is clean, with soft colors, emojis for readability, and simple navigation. The design includes:

KPI cards for CPA, CTR, CVR, CPC, CPM

Audience insights: Age × Gender × Interests

Campaign performance charts

Heatmaps and bar charts for cost-efficiency and conversions

Slicers for filtering by campaign, date, gender, and age

Clear navigation and actionable insight cards

Main Insights

Overall Performance:

CTR is extremely low (0.02%) → ad engagement is weak

CVR is strong (7.92%) → clicks convert well

CPA is high ($59) → budget not efficiently turning clicks into approved conversions

213M impressions but only 38K clicks → large audience, poor message fit

Gender Insights:

Men: higher CVR (10.3%), lower CPA ($45)

Women: more clicks, higher CPA ($74) → targeting/creative mismatch

Age Insights:

Best ROI: 30–34 & 35–39 → lower CPA, higher conversion

Weak: 45–49 → high CPA ($124)

Campaign Performance:

Campaign 916: top performer, CVR 31.5%, CPA $10.51 → scalable

Campaign 936: moderate CPA ($25)

Campaign 1178: high volume but high CPA ($64) → optimize

Interest Insights:

Top-performing interests: Interest 4, 7, 15 → low CPA, high CVR

Poor-performing interests: Interest 3, CPA > $50

Business Impact

This dashboard helps identify:

Real drivers of conversions and ROI

Segments worth scaling

Weak audiences and campaigns needing optimization

Which interest and age groups convert most efficiently

Where to allocate budget for maximum efficiency

Insights support decisions in ad targeting, budget allocation, creative optimization, and campaign scaling.

Repository Structure

📦 Facebook-Ads-PowerBI
├─ 📁 Power_Bi (.pbix file + viuals )
├─ 📁 Data ( raw CSVs)
├─ 📁 notebooks
(data cleaning.ipynb (cleaning, KPI calculations... )+ cleaned dataset )
├─ README.md (this file)

How to Use the Report

Open the .pbix file in Power BI Desktop or view the live dashboard(https://app.powerbi.com/groups/me/reports/4c0ca791-f504-400b-9f96-b7a3c70b85d0/dac43e057ffa3137854a?experience=power-bi)

Interact with filters for campaign, age, gender, and interests.

Hover over charts for detailed KPIs.
