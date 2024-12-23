
# Marketing Analytics Business Case

## Problem Statement

ShopEasy, an online retail business, is facing reduced customer engagement and conversion rates despite launching several new online marketing campaigns. They are reaching out to you to help conduct a detailed analysis and identify areas for improvement in their marketing strategies.

Key Points:
- Reduced Customer Engagement: The number of customer interactions and engagement with the site and marketing content has declined.
- Decreased Conversion Rates: Fewer site visitors are converting into paying customers.
- High Marketing Expenses: Significant investments in marketing campaigns are not yielding expected returns.
- Need for Customer Feedback Analysis: Understanding customer opinions about products and services is crucial for improving engagement and conversions.

## Goal:

- Increase Conversion Rates:
  - Goal: Identify factors impacting the conversion rate and provide recommendations to improve it.
  - Insight: Highlight key stages where visitors drop off and suggest improvements to optimize the conversion funnel.

- Enhance Customer Engagement:
  - Goal: Determine which types of content drive the highest engagement. 
  - Insight: Analyze interaction levels with different types of marketing content to inform better content strategies.

- Improve Customer Feedback Scores:
  - Goal: Understand common themes in customer reviews and provide actionable insights.
  - Insight: Identify recurring positive and negative feedback to guide product and service improvements.


## Steps followed :

- Step 1 : Load the Database in MS SQL Server
    - Connect to the database and explore its structure, including tables, relationships, and data types.
    - Use SQL queries to preview the data and understand its contents.
- Step 2 : Understand and Clean the Tables
  - Identify redundant, missing, or inconsistent data.
  - Perform data cleaning using SQL queries: Remove duplicates, Handle missing values appropriately, Standardize data formats.
  - Document transformations for future reference.
- Step 3 : Perform Sentiment Analysis Using Python
   - Extract the reviews data from SQL Server using Python libraries like pyodbc or sqlalchemy.
   - Use sentiment analysis tools such as VADER, NLTK to analyze reviews.
   - Assign sentiment scores to reviews and create buckets: 
     - Positive: High sentiment score and rating.
     - Mixed Positive: Positive sentiment but neutral or low rating.
     - Neutral: Balanced sentiment and rating.
     - Mixed Negative: Negative sentiment but neutral or high rating.
     - Negative: Low sentiment score and rating.
- Step 4 : Generate a CSV File
    - Save processed data with sentiment scores and categories into a CSV file.
- Step 5 : Load Data into Power BI
     - Import the CSV file and use Power Query Editor for any additional transformations. 
- Step 6 : Create Dashboard and Draw Insights
    -  Design visuals like pie charts, bar charts, and line charts to represent sentiment distributions and trends.
    - Highlight key metrics (e.g., Positive vs. Negative reviews).
- Step 7 : Enhance Dashboard with Additional Features
     - Add filters for sentiment categories and date ranges.
     - Include KPIs like total reviews and average sentiment score.
    
 
 ## Report Snapshot (Power BI Desktop)
 
![image](https://github.com/user-attachments/assets/65008ddf-8e02-4752-973b-56f17afb274f)

![image](https://github.com/user-attachments/assets/6e57467d-0166-4be5-8c13-acfc35beb552)

![image](https://github.com/user-attachments/assets/145d103b-bb70-4dc0-89d2-8824c2c825bb)

![image](https://github.com/user-attachments/assets/cdcc7d31-18df-4d55-8a46-6325accd646f)


## Insights

A 4 page report was created on Power BI Desktop which consist of Overview, Conversion Details, Social Media Details, Customer reviews details.

![image](https://github.com/user-attachments/assets/73645da6-05cd-4c00-9d96-37c92d33c44a)

Following inferences can be drawn from the dashboard;

### [1] Reduced Customer Engagement

   - Decreased Conversion Rates: The conversion rate demonstrated a strong rebound in December, reaching 10.2%, despite a notable dip to 5.0% in October.
  - General Conversion Trend: Throughout the year, conversion rates varied, with higher numbers of products converting successfully in months like February and July. This suggests that while some products had strong seasonal peaks, there is potential to improve conversions in lower-performing months through targeted interventions.
  - Lowest Conversion Month: May experienced the lowest overall conversion rate at 4.3%, with no products standing out significantly in terms of conversion. This indicates a potential need to revisit marketing strategies or promotions during this period to boost performance.
 - Highest Conversion Rates: January recorded the highest overall conversion rate at 18.5%, driven significantly by the Ski Boots with a remarkable 150% conversion. This indicates a strong start to the year, likely fueled by seasonal demand and effective marketing strategies.


![image](https://github.com/user-attachments/assets/162d493a-3fb0-43d9-af03-ea26f6beaa11)

           
### [2] Reduced Customer Engagement:

 - There is a decline in overall social media engagement, with views dropping throughout the year.
 - While clicks and likes are low compared to views, the click-through rate stands at 15.37%, meaning that engaged users are still interacting effectively.
 - Declining Views: Views peaked in February and July but declined from August and on, indicating reduced audience engagement in the later half of the year.

 ![image](https://github.com/user-attachments/assets/4d7ac73b-c54b-4cfb-a3db-b08a34194862)

 - Low Interaction Rates: Clicks and likes remained consistently low compared to views, suggesting the need for more engaging content or stronger calls to action.
 - Content Type Performance: Blog content drove the most views, especially in April and July, while social media and video content maintained steady but slightly lower engagement.

 ![image](https://github.com/user-attachments/assets/cc497902-7793-49d2-ab57-d9a465307ae9)


  ### [3] Customer Feedback Analysis:
  
 - Customer ratings have remained consistent, averaging around 3.7 throughout the year.
 - Although stable, the average rating is below the target of 4.0, suggesting a need for focused improvements in customer satisfaction, for products below 3,5.
 - Customer Ratings Distribution: The majority of customer reviews are in the higher ratings, with 140 reviews at 4 stars and 135 reviews at 5 stars, indicating overall positive feedback. Lower ratings (1-2 stars) account for a smaller proportion, with 26 reviews at 1 star and 57 reviews at 2 stars.
   ![image](https://github.com/user-attachments/assets/a7b2fad2-a4ad-4e05-92dd-45939f1c3846)
 - Sentiment Analysis: Positive sentiment dominates with 275 reviews, reflecting a generally satisfied customer base. Negative sentiment is present in 82 reviews, with a smaller number of mixed and neutral sentiments, suggesting some areas for improvement but overall strong customer approval.
 ![image](https://github.com/user-attachments/assets/3f5a8585-17f6-425e-ab5d-69d36371ff00)
 - Opportunity for Improvement: The presence of mixed positive and mixed negative sentiments suggests that there are opportunities to convert those mixed experiences into more clearly positive ones, potentially boosting overall ratings. Addressing the specific concerns in mixed reviews could elevate customer satisfaction.

 ## Actions

 - Increase Conversion Rates:
   - Target High-Performing Product Categories: Focus marketing efforts on products with demonstrated high conversion rates, such as Kayaks, Ski Boots, and Baseball Gloves. Implement seasonal promotions or personalized campaigns during peak months (e.g., January and September) to capitalize on these trends.
- Enhance Customer Engagement:
   - Revitalize Content Strategy: To turn around declining views and low interaction rates, experiment with more engaging content formats, such as interactive videos or user-generated content. Additionally, boost engagement by optimizing call-to-action placement in social media and blog content, particularly during historically lower-engagement months (September-December).
- Improve Customer Feedback Scores:
   - Address Mixed and Negative Feedback: Implement a feedback loop where mixed and negative reviews are analyzed to identify common issues. Develop improvement plans to address these concerns. Consider following up with dissatisfied customers to resolve issues and encourage re-rating, aiming to move average ratings closer to the 4.0 target.



