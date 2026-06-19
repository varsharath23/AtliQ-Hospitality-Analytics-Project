# AtliQ Hospitality Analytics Dashboard - PowerBI

- Domain: Hospitality
- Function: Revenue

Link to the [Challenge](https://codebasics.io/challenges/codebasics-resume-project-challenge/4)

Link to [Interactive Dashboard](https://app.powerbi.com/view?r=eyJrIjoiODRmZDZiNzEtZjk1Zi00ZmNkLTk5ODItMGQxZTk5NmMyM2RmIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

## Problem statement

Atliq Grands owns multiple five-star hotels across India. They have been in the hospitality industry for the past 20 years. Due to strategic moves from other competitors and ineffective decision-making in management, Atliq Grands are losing its market share and revenue in the luxury/business hotels category. As a strategic move, the managing director of Atliq Grands wanted to incorporate “Business and Data Intelligence” in order to regain their market share and revenue. However, they do not have an in-house data analytics team to provide them with these insights.

Their revenue management team had decided to hire a 3rd party service provider to provide them insights from their historical data.

### Task List

You are a data analyst who has been provided with sample data and a mock-up dashboard to work on the following task. You can download all relevant documents from the download section.

- Create the metrics according to the metric list. 
- Create a dashboard according to the mock-up provided by stakeholders. 
- Create relevant insights that are not provided in the metric list/mock-up dashboard.


## Provided Mock-up Dashboard
<p align="center">
    <img src="https://github.com/Naveen-S6/AtliQ_Hospitality_Analysis_PowerBI/blob/main/Dataset/mock%20up%20dashboard_atliq%20grands.png" width="600">
</p>


## Learnings:

### 1. Data Validation is important before analysis
- Learned to validate data quality before building any dashboard.
- Learned to check null values, date inconsistencies, and data-type issues that could have led to incorrect business conclusions.
- Identified that the ratings_given column contained many null values & decided not to replace them because a missing review is fundamentally different from a poor review. 

### 2. Data Modeling & Relationships matter more than complex DAX
- Learned how to build and work with a star schema.

### 3. Understanding Filter Context is the most important DAX skill
- Learned the practical difference between ALL() and ALLSELECTED()
- While building Revenue Contribution %, I found that: 
  - Atliq Exotica Mumbai showed 12.43% in one visual. 
  - The same property showed 22.45% in another visual. 
  - Traced the issue to how ALLSELECTED() interacted with a Top N filter. 

### 4. Importance of a dedicated Date Table
- Learned that time-based analysis becomes significantly easier and more reliable with a proper date table. 
- Used the date table to build: 
  - Weekly Trends 
  - Revenue WoW % 
  - Occupancy WoW % 
  - Monthly filtering
 
### 5. Hospitality Performance is a Balance of Demand, Pricing and Capacity
- Developed an understanding of:
  - Occupancy % 
  - ADR 
  - RevPAR 
  - Revenue 
  - Realisation % 
  - Cancellation % 
  - No-Shows
- RevPAR is one of the most important top-line metrics in hospitality.
- Learned that:
  - High Occupancy alone does not guarantee strong performance. 
  - High ADR with poor Occupancy may indicate pricing issues. 
  - RevPAR is valuable because it combines pricing and occupancy performance. 
  - Revenue Realized is often more meaningful than Revenue Generated because cancellations and no-shows affect actual outcomes.
 

## Insights:

- Total revenue is ₹1.71bn (+7.23% WoW), but RevPAR (₹7.35K) and Occupancy (57.87%) have declined WoW by nearly 1%.
- Average Daily Rate (ADR) remains completely flat at ₹12.70K across all weeks, failing to adapt to shifting market demand.
- Due to flat pricing, RevPAR directly mirrors regular, cyclical drops in occupancy, bottoming out around 51% during low weeks.
- The Luxury segment (62%) and Elite rooms (33%) drive the business, with Mumbai generating 39% of total revenue.
- Properties with poor guest ratings (~3.0) suffer from low occupancy (~53%), whereas highly rated properties (4.2+) maintain ~66% occupancy.
- Atliq Bay (Hyderabad) maintains a strong 65.87% occupancy but yields the lowest ADR in the portfolio at ₹9.44K.
- Every single distribution channel and property suffers from an identical, high cancellation rate (24%–26%) and no-show rate (~5%).
- 42.13% of total inventory goes unutilized daily (1.07K rooms), with 71% of that waste concentrated in high-margin tiers (Elite, Premium, Presidential).
- Weekend occupancy structurally outperforms weekdays (67% vs 60%), yet weekends account for only 30.87% of captured guest reviews.
- Week 32 experienced an unprecedented flip where weekday occupancy spiked to 65.3% while weekend occupancy collapsed to 49.2%.

- Atliq Grands is actively losing market share in its core luxury/business sectors due to aggressive competitor moves and a lack of internal business intelligence capabilities.














