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

|               account |         iap_purchase | account_date_session |
|----------------------:|---------------------:|---------------------:|
|            account_id |           account_id |	       account_id |
|          created_time |	              date |         created_time |
|        created_device |	     session_count |      package_id_hash |
|      created_platform | session_duration_sec |  iap_price_usd_cents |
|          country_code |	                   |	     app_store_id |
|  created_app_store_id |                      |	                  | 

## Part 1: Product Engagement and Revenue Dashboard on Tableau
### Key Features

- **Year-to-date performance overview:** A summary of overall performance and monthly trends of key metrics capturing trends of engagement, revenue, retention & LTV
    - Monthly Active Users (MAU): Shows how many unique players engage with the game monthly
    - Lifetime Value (LTV): Total revenue from a player over their lifetime, essential for calculating customer acquisition cost (CAC) thresholds.
    - Retention Rate (Day 1, Day 7, Day 30, etc.): The percentage of players who return to the game after 1, 7, or 30 days, crucial for understanding first impressions and long-term value.
      ![YTD Performance](https://github.com/user-attachments/assets/62abc33b-4b32-4efb-b399-86f0a4a88852)

- **Engagement**
    - Daily Active Users (DAU): Shows how many unique players engage with the game daily
    - Session Length: How long a player spends in the game per session, helps assess game pacing, content length, and player interest.
    - Session Frequency / Sessions per User per Day: Measures how often users return in a day, higher frequency typically indicates strong engagement or addictive loops.
![Engagement](https://github.com/user-attachments/assets/cce207c1-92ba-43f5-aa4d-e3a283bca1c3)

- **Monetization** 
    - Average Revenue Per Daily Active User (ARPDAU): Revenue generated per active user per day, key for understanding short-term revenue health.
    - Average Revenue Per Paying User (ARPPU): Shows how much paying users spend on average, helps optimize pricing and in-game offers. 
![Monetization (IAP)](https://github.com/user-attachments/assets/d951f724-bf9d-4003-b9ef-bbea2e1be16f)

- **Cohort Analysis:** groups users based on install date and tracks their behavior and LTV over time, informs payback periods and how long you can afford to wait before a user becomes profitable.
![Cohort by Day](https://github.com/user-attachments/assets/4ba48a7e-018b-4862-8332-0ab5bf443f58)


- **Performance by Market:** Overview game performance by market
![Performance by Market](https://github.com/user-attachments/assets/e25ee3da-c864-4858-bfe3-92691d8a2253)

## Part 2: Player LTV Prediction (work-in-progress)
