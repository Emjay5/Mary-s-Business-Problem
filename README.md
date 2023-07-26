![IMG_0244](https://github.com/Emjay5/Mary-s-Business-Problem/assets/136242686/d1e73225-52be-4725-bc02-5c6bab032112)

# INDRODUCTION

WHY MARY'S PHARMACEUTICAL DRUG SALE IS STAGNANT  FOR OVER 6 YEARS
Coming up with business questions and generate metrics that could be tracked to identify trends and patterns in the sale of pharmaceutical drugs sold in the pharmacy over time.

1.	Why sale was stagnant for Mary’s store
2.	What are the ways to increase Mary’s sales?
3.	What drug Category contributes the most to the overall sales
4.	Are there seasonal trends or patterns in the sale of the pharmaceutical drug
5.	What is the average daily quantity of drugs sold
6.	What category of drugs has the highest and lowest profit.
7.	What pharmaceutical drugs have the highest and lowest sale volume in Mary’s pharmacy
8.	How does sale correlate with external factor such as weather conditions? 

 ANSWERS TO THESE BUSINESS QUESTIONS
 To answer these business questions we will have to genetrate KPIs (metrix) to track performance  based on the struture we have set.
 1. Calulate the total sales revenue based on diffirent dimension; Time of day.
 2. Calulate the total quantity and total sales
 3. Calculate percentage by sale
 4. Calculate top selling drugs  
 5. Calucate total sale  and quanty for each drug category; M01AB, M01AE, M02BA,M02BE,N05B, N05C, R03, R06.
 6. Calculate sales growth rate.


# Business problem
Mary is the owner of a small pharmacy located in a busy city center. She has been running the pharmacy for the past few years and has noticed that sales have stagnated. Despite the competitive pricing, Mary's Pharmacy has struggled to attract new customers.

To try and improve her business, Mary decided to contact Datafied Technologies to conduct a thorough analysis of her sales data using the transactional data collected over the past 6 years. She exports the data from her Point-of-Sale system, which includes information on the date and time of each sale, the name of the pharmaceutical drug sold, and the quantity of each drug sold.

You are the senior data analyst at Datafied Technologies. You are required to come up with business questions and generate metrics that could be tracked to identify trends and patterns in the sale of pharmaceutical drugs sold in the pharmacy over time. You also need to visualize the data and create dashboards to uncover hidden insights and track the metrics you have defined for the business.

Mary needs your help to uncover valuable insights about her business and take action to improve its performance. Mary intends to use this newfound knowledge to make informed decisions about her inventory and marketing strategies, ultimately leading to an increase in sales and the growth of her business.

# Dataset information
The dataset is built from the initial dataset consisting of transactional data collected in 6 years (period 2014-2019), indicating the date and time of sale, pharmaceutical drug brand name, and sold quantity, exported from the Point-of-Sale system in the individual pharmacy. The selected group of drugs from the dataset (57 drugs) is classified into the following Anatomical Therapeutic Chemical (ATC) Classification System categories:

- M01AB - Anti-inflammatory and antirheumatic products, non-steroids, Acetic acid derivatives, and related substances
- M01AE - Anti-inflammatory and antirheumatic products, non-steroids, Propionic acid derivatives
- N02BA - Other analgesics and antipyretics, Salicylic acid and derivatives
- N02BE/B - Other analgesics and antipyretics, Pyrazolones and Anilides
- N05B - Psycholeptics drugs, Anxiolytic drugs
- N05C - Psycholeptics drugs, Hypnotics, and sedatives drugs
- R03 - Drugs for obstructive airway diseases
- R06 - Antihistamines for systemic use

Data Source: [Mary's dataset](https://www.kaggle.com/datasets/milanzdravkovic/pharma-sales-data?select=salesdaily.csv)

## Project Objective
The objective of the project was to help Mary's Pharmacy improve its sales performance and overall business operations by analyzing transactional sales data and then creating dashboard(s) that provide valuable insights to the sales manager and CEO. The dashboard should uncover trends, patterns, and opportunities in the sale of pharmaceutical drugs, enabling informed decision-making and driving business growth.

Throughout the project, we were able to achieve the following:

### Understand Business Objectives and User Requirements
We tried to understand the specific requirements and objectives from the business problem. We identified key areas we want to focus on and the questions the business needs answers to.

## Define Business Questions and Metrics
Based on the discussions in Step 1, we defined specific business questions that the dashboard should answer. Example questions include:

- What is the overall sales trend for the pharmacy?
- Which drugs have the highest sales revenue?
- Are there any seasonal sales patterns for specific drugs or ATC categories?
- What time of the day has the highest sales?
  
## Define the metrics and Key Performance Indicators (KPIs) that will help answer the business questions.
  Example metrics include:
- Total sales revenue
- Quantity sold by drug or ATC category
- Sales growth rate
- Top-selling drugs by revenue or quantity
- Quantity growth rate.

## Preprocess the dataset:
The dataset was cleaned by removing duplicates, correcting any inconsistencies, and ensuring the data is in a suitable format for analysis and visualization.


### Dataset after cleaning

image


## Data modelling and relationships.
Dimensions with which to break down the analysis were identified. Hence, new tables for identified dimensions were created. These included:

Drugs Table
Date Table
Time Table
Additional features were created to give more robustness to our analysis
The data model was designed using the Star Schema where the different dimensions were connected to the Facts table in a one-to-many relationship.

image

<img width="878" alt="Screenshot 2023-07-23 163620" src="https://github.com/Emjay5/Mary-s-Business-Problem/assets/136242686/352ce386-ca29-4269-a637-8476d176057b">


## Create visualizations and charts:
Appropriate chart types (e.g., bar charts, line charts, pie charts) were used to represent the metrics and insights. Interactive features such as filters, drill-down options, and tooltips were used for detailed information.

image

<img width="511" alt="Screenshot 2023-07-23 163723" src="https://github.com/Emjay5/Mary-s-Business-Problem/assets/136242686/2e67bbf7-3bed-4bfb-8c54-f48498ec470f">



# Dashboard Testing and Refinement
To guide each student throughout the project, they get the opportunity to schedule a one-on-one session with an instructor. This is to get feedback on their work done and to see if they were meeting up with the project's requirements. The students gathered feedback from these sessions and made necessary adjustments to their dashboard layout, visualizations, and insights based on the feedback received.

## Incorporate relevant insights and trends:
I highlighted the most important insights and trends on my dashboard.


# Insights
General overall trend for sales was not steady. The pharmacy started off well. 2014, 2016, and 2018 were good years for the business. However, 2015, 2017, and 2019 were also down times for the business.
2018 had the highest sales
While it was established that 2018 was the best year in terms of sales, that is not the true picture for specific drugs.
Considering seasons, sales were generally good in winter and spring. However for specific drugs, the M0 series do well in autumn and winter, the R0 series do well in spring and the N0 series does not show a specific seasonal pattern.
Sales declined in 2015 by 8% this was strongly attributed to the decline in the sales and quantity sold of N05B (Psycholeptics drugs, Anxiolytic drugs) drugs in that year
Afternoon records the time with the most sales. However, across the drug category, the R0 drug series sell more in the evenings than in the afternoons.
N05B maintains the top-selling drugs across all years followed by N02BE and then R03 drugs. R03 overtook N02BE in terms of sales in 2018.
While N05B is the best seller in terms of sales, in terms of quantity, N02BE has the highest quantity sold selling 3 times the quantity sold for N05B.

# Recommendation
The management should look into the market conditions and strategies adopted for moving sales in 2014,2016 and 2918 such as operational efficiency, supply chain, customer service, and so on as those strategies might have worked.
Certain drugs showed good performance for particular seasons. Marketing efforts should be centered around them for that particular period.
For drugs that show seasonal patterns as well, the management should ensure enough supply of those drugs around that time to match up with the demand.
There might be a huge opportunity in sales if the pharmacy considers opening 24 hours
The management should consider increasing prices, especially for N02BE drugs as they have shown to drive the market more.
Deployment and Documentation
Once the dashboard was finalized, it was deployed to Power BI service. The project process and deliverables are documented here on GitHub.

Interact with the final dashboard here:

