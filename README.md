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
