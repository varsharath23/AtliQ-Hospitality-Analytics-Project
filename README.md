# AtliQ Hospitality Analytics Dashboard - PowerBI

Link to the [Challenge](https://codebasics.io/challenge/codebasics-resume-project-challenge)

Link to [Interactive Dashboard]([https://www.novypro.com/project/-codebasics-september-month-resume-challenge](https://app.powerbi.com/view?r=eyJrIjoiODRmZDZiNzEtZjk1Zi00ZmNkLTk5ODItMGQxZTk5NmMyM2RmIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9))

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

### 2. Data Modeling & Relationships Matter More Than Complex DAX
- Learned how to build and work with a star schema.

### 3. Understanding Dilter Context is the most important DAX skill
- Learned the practical difference between ALL() and ALLSELECTED()
- While building Revenue Contribution %, I found that: 
  - Atliq Exotica Mumbai showed 12.43% in one visual. 
  - The same property showed 22.45% in another visual. 
  - Traced the issue to how ALLSELECTED() interacted with a Top N filter. 

### 4. Importance of a dedicated Date Table












