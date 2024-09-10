## Bank Marketing Campaign Analysis

# Objective
The goal of this project was to analyze the direct marketing campaigns of a Portuguese bank to understand the factors influencing customer subscription to term deposits. By leveraging customer data and exploring key features, we aimed to uncover patterns and trends that can improve future marketing campaigns.

# Dataset Information
Domain: Banking
Number of Records: 45,000 customers
Number of Contacts: 125,000 contacts
Target Variable: Whether the customer subscribed to a term deposit (yes/no)
## Attributes:
# Numerical Variables:
age: Customer age
balance: Average yearly balance in euros
duration: Last contact duration in seconds
campaign: Number of contacts during this campaign
pdays: Days since last contact
previous: Number of contacts before this campaign
# Categorical Variables:
job, marital, education, default, housing, loan, contact, poutcome, month
Target: Subscribed (binary: "yes"/"no")
2. Data Exploration and Cleaning
## Data Exploration
We began by exploring the dataset to understand the distribution of each feature:

Histograms for numerical variables like age, balance, duration, pdays.
Bar charts for categorical variables like job, marital, education, contact type, poutcome.
Handling Missing and Unknown Values
Categorical features such as job, education, default had 'unknown' values.
We analyzed the proportion of 'unknown' values and decided to treat them as a separate category.
## Outliers
Outliers were identified in balance, duration, and age. We visualized outliers using boxplots and determined if any needed to be handled based on business context (e.g., outliers in balance were retained as they might represent valuable customers).


![Screenshot 2024-09-10 145353](https://github.com/user-attachments/assets/ba4eb8f7-d0b6-4fab-b793-faff638d5328)


## Key Insights
Customer Base Analysis
Total Customers: 45,000 unique customers.
Total Contacts: 125,000 contacts made during the campaign (multiple contacts per customer).
Subscription Rate: Out of the 45,000 customers, 5,289 subscribed to the term deposit (~11.8%).
## Feature Analysis:
Credit History: Most customers had no credit in default. This can indicate financial stability among the majority of clients.
Contact Type: Cellular contact was used more frequently than telephone, indicating a shift in preference towards mobile communication.
Education Levels: Most customers had completed secondary or tertiary education, followed by those with professional qualifications.
Marital Status: Married customers formed the largest group, followed by single customers.
Age Range: The most common age group was between 30 and 50 years, indicating a middle-aged customer base.
Job Role & Subscriptions: Customers working in management had the highest subscription rate compared to other occupations.
Loan and Subscription: Most customers who subscribed had no personal loans, indicating that customers without additional debt may be more likely to invest in a term deposit.
## Campaign Effectiveness:
Pdays & Subscription: As the number of days since last contact (pdays) increased, the probability of subscription decreased. This suggests that re-engaging customers quickly after a previous campaign may improve outcomes.
Campaign & Subscription: Similarly, as the number of contacts made during the current campaign (campaign) increased, the likelihood of subscription decreased. This suggests that over-contacting customers might negatively affect conversion rates.

![Screenshot 2024-09-10 145446](https://github.com/user-attachments/assets/c1bba078-60ae-4523-a0f2-c772cb438efa)


## Conclusion
Business Recommendations
Based on the findings from the data: Customer Segmentation: Focus on customers between the ages of 30 and 50, especially those in management roles and those without personal loans, as they show a higher likelihood of subscribing.

Optimize Campaign Strategy: Avoid over-contacting customers during a campaign, as multiple contacts seem to reduce the probability of a subscription.

Faster Re-engagement: The sooner a customer is re-contacted after a previous campaign, the higher the chances of conversion.

Cellular over Telephone: Since cellular contact was more successful, marketing efforts should prioritize mobile communication.
