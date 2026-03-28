# Customer Personality Clustering: Project Overview
- Build a clustering model to help marketing team segmenting the customers into 6 segments to help deciding the best marketing strategies for each customers based on their profile and behaviors.
- Cleaned the data from missing value in the income's feature (26 empty columns), 4 Invalid data ouliers (3 from year born feature where the customers age above 100yo and 1 from income feature where the income is ununsually high numbers (666.666.000) and 4x the second highest income while the spending is really low.
- The X features are split into profile (8 features) and and behavior (8 features) to help the segment analyzed from various angle.
- Model trained with KMeans algorithms

## Problems
- Overall, most of customers in the database have low Web Campaign Conversion Rate. Where the average Campaign Conversion Rate only 4%
- Majority of customer’s too have low Campaign Acceptance Rate.  Out of total 2213 customers only 458 (21%) that ever respond to any campaigns. 
<img width="765" height="202" alt="image" src="https://github.com/user-attachments/assets/20406afd-2cb0-4f3e-b319-1f1c7fa41cc4" />

## Purposes
Help the marketing team to boost the campaign acceptance and conversion rate by splitting the customers into few segments to help the team personlized the marketing strategy used for each segments.

## Early Insight from The Data
- Based on education, most of the company customers have rather high education degree.
<img width="668" height="567" alt="image" src="https://github.com/user-attachments/assets/83b444fa-9566-468d-b5fc-f637fb85bcde" />

- Most of customers are married
<img width="638" height="506" alt="image" src="https://github.com/user-attachments/assets/0d96034f-e40d-4b74-a299-f58a596b59e4" />

- The company business are dominated by customers with 60+ age range.  In the future the company may need to attract more of younger generation.
<img width="640" height="509" alt="image" src="https://github.com/user-attachments/assets/9ef47e61-4000-49e5-b86a-5310dab21971" />

- The customers distributed evenly based on their income group tier
<img width="494" height="329" alt="image" src="https://github.com/user-attachments/assets/e1224cc6-9ea8-4fee-96ba-8b4c2999b4b0" />

- Physical stores remain the primary touchpoint, accounting for 50.5% of total distribution across all demographics.
<img width="520" height="283" alt="image" src="https://github.com/user-attachments/assets/aa5a500c-763e-42f8-addd-d2e02aad403a" />

## ML Modeling
Before modeling, the data split into 2 groups: Customer Profile & Customer Behavior. This was done to make sure the customer personality can be analyzed from multiple angle. Each groups then analyzed using silhouette & elbow method to help identifying most optimal number of clusters for each group. Then each group trained using KMeans algorithm based on their optimal clusters.

## The Result
1. Customer Profile
- Cluster 0. Mature Established Families: Highest percentage in oldest (60+) age group, dominant in Mid - High Income group, higher education average, Long tenure Stable, mature, financially capable customers
- Cluster 1. Mid-Age Balanced Segment: Dominated by customers in 40-59 age group. Income distributed evenly and have long tenure
- Cluster 3. Younger & Early-Stage Families: Higher propotions in younger customers and lower income group than other clusters also have long tenure.
<img width="1048" height="660" alt="image" src="https://github.com/user-attachments/assets/3313fd8d-68ee-4dde-a762-1ad30fd6866e" />

2. Customer Behavior
- Cluster 0. Premium Responders: High spending, not that interested in deals, prefers catalouge and have high acceptance and conversion rate towards campaigns.
- Cluster 1. Low-Value Deal Hunters: Lower total spending, interested in deals, prefer web and store channels, lower accepance and conversion rate towards campaign.
<img width="1060" height="659" alt="image" src="https://github.com/user-attachments/assets/c5a2a748-eb37-4a3b-ae9d-4b96b36b5a27" />

3. Cross Insight
Each cluster then combined into these segment:
<img width="744" height="408" alt="image" src="https://github.com/user-attachments/assets/2773a853-366e-40bb-8a49-2fcb9421bf3b" />

#### CP
These project was created using dataset from Rakamin as part of assigment. For more information feel free to contact me from:

- No/WA: +6281292728395

- E-mail: mercy.claudiam@gmail.com

-  LinkedIn: : linkedin.com/in/mercy-claudia09
