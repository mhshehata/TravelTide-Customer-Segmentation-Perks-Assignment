# TravelTide Customer Segmentation Perks Assignment
<img src="https://github.com/mhshehata/TravelTide-Customer-Segmentation-Perks-Assignment/blob/main/logo.png">

## Project Description
The goal of this project is to segment customers in the TravelTide database into five different segments based on their spending patterns, booking habits, and travel preferences. Based on these segments, we will assign customers to one of five relevant perks. These perks are intended to foster customer loyalty, increase engagement, and improve overall satisfaction.

### The five perks are as follows:

10% Flight Discount

10% Hotel Discount

One Night Free Hotel

Free Airport Transportation

Free Cancelation or Free Checked-Bag

### Business Objective
Create a compelling rewards program that encourages customer loyalty and repeat business on the TravelTide platform.

## Data and Methodology

### Data
The data used in this project was obtained from the TravelTide database. As per the marketing manager's instructions, we analyzed user sessions that occurred between April 1, 2023, and July 23, 2023. Only users with a minimum of seven sessions during this period were included in the analysis.

### Methodology
- Starting with 5,408,063 user sessions, EDA, cleaning, and aggregating the data were done using PostgreSQL.
- To avoid potential biases from incomplete data, only booked and completed trips were included in the analysis.
- This resulted in a dataset of 5,998 unique users, which is used to calculate key metrics via Feature Engineering.
- To prepare the dataset for K-Means Clustering, Python is utilized for data visualization, manipulation, and Principal Component
- Analysis (PCA). Silhouette analysis is adopted to determine the optimal number of clusters.
- Based on the K-Means Clustering results, customers are grouped into segments with similar characteristics. Each segment is then assigned a specific perk.

## Feature Engineering

<img src ="https://github.com/mhshehata/TravelTide-Customer-Segmentation-Perks-Assignment/blob/main/feature%20engineering.png">

## Segments Charachteristics

**Frequent Flyers**: These customers have a high frequency of flights and significant spending on air travel.

**Family/Group Travelers**: This segment is characterized by longer trips, multiple nights booked, and a higher number of seats, suggesting they often travel with family or in groups.

**Long-Hotel-Stay Travelers**: Customers in this group tend to book longer hotel stays, often requiring multiple rooms and incurring higher hotel expenses.

**Couple Travelers**: This segment typically consists of couples taking trips of moderate length. They often book two seats, check two bags, and stay in a single hotel room.

**Solo/Business Travelers**: These customers usually travel alone or on business trips. They have a single bag, require only one room and seat, and their trips are of medium duration.


## Segmentation Criteria

**Frequent Flyers**: Customers are considered frequent flyers if they have 6 or more flights.

**Family/Group Travelers**: Customers are classified as "family or group" travelers if they have an average of more than 2 seats per trip or an average of at least 2 rooms per trip.

**Long-Hotel-Stay Travelers**: are defined as customers who have an average of at least 5 nights per trip and minimum of 3 hotel trips.

**Couple Travelers**: Couples are defined as customers who have an average of at least 3 nights per trip, 
2 seats per trip, and no more than 1 room per trip.

**Solo/Business Travelers**: Customers are considered solo or business travelers if they have an average of 
1 seat and 1 bag per trip.


## Results
### Perks Distribution

<img src="https://github.com/mhshehata/TravelTide-Customer-Segmentation-Perks-Assignment/blob/main/perk_distribution.png">

## Recommendations

**A/B Testing: Comparing the Impact of Targeted Perks vs. Random Perks**

Compare the effectiveness of perks specifically tailored to customer segments (targeted perks) against a control group receiving randomly selected perks.

**Customer Feedback**

Collect customer feedback after a beta implementation of the loyalty program and do further analysis considering the retrieved data.

**Female-Centric Appeal**

Analyze the factors contributing to the predominance of female users in our dataset.

**Tailoring Marketing Campaigns for U.S. Users**
Given the significant number of U.S. users in our database, creating targeted marketing campaigns specifically designed for this demographic could yield substantial benefits.
