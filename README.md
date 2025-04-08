# Casual Game Analytics: Product Performance Dashboard and Player LTV Prediction

[![View on Tableau](https://img.shields.io/badge/View_on_Tableau-PURPLE?logo=Tableau)](https://public.tableau.com/app/profile/linh.chu3700/viz/GameAnalyticsDashboard_17437556396800/YTD)


## Summary
The project was built using a dataset from a Supercell game, with 2 main deliverables:
1. (Done) A Tableau dashboard to monitor and analyze app metrics: engagement, monetization, cohort retention and LTV
2. (WIP) An ML model to predict player LTV

### Datasets
The datasets contain 3 tables:
1. account
2. account_date_session
3. iap_purchase

| account | iap_purchase | account_date_session |
|-----:|---------------:|--:|
| account_id |	account_id |	account_id |
| created_time |	date	| created_time |
| created_device |	session_count |	package_id_hash |
| created_platform |	session_duration_sec |	iap_price_usd_cents |
| country_code |	|	app_store_id | 
| created_app_store_id	| |	

## Part 1: Product Engagement and Revenue Dashboard on Tableau
## Key Features

- **Year-to-date performance overview:** A summary of overall performance and monthly trends of key metrics
    - Monthly charts capturing trends of metrics on engagement, revenue, retention & LTV
      ![YTD Performance](https://github.com/user-attachments/assets/62abc33b-4b32-4efb-b399-86f0a4a88852)

- **Engagement** Zoom into a specific period using a start-end date filter
    - Provide a snapshot of KPIs, along with comparisons with another period which users can choose based on their needs
    - Metric comparison by day: include filters to choose 2 metrics to trend over time
    - Campaign phase contribution: drill down on spend & revenue pacing
    - Audience mix efficiency: to understand how each audience group responds to the ads and decide whether to scale up/down the investment
![Engagement](https://github.com/user-attachments/assets/cce207c1-92ba-43f5-aa4d-e3a283bca1c3)

- **Monetization** Zoom into a specific period using a start-end date filter
![Monetization (IAP)](https://github.com/user-attachments/assets/d951f724-bf9d-4003-b9ef-bbea2e1be16f)

- **Cohort Analysis** Zoom into a specific period using a start-end date filter
![Cohort by Day](https://github.com/user-attachments/assets/4ba48a7e-018b-4862-8332-0ab5bf443f58)


- **Performance by Market** Zoom into a specific period using a start-end date filter
![Performance by Market](https://github.com/user-attachments/assets/e25ee3da-c864-4858-bfe3-92691d8a2253)
