# Speedline Wheels Sales Analysis - Data Cleaning and Analysis

## Introduction
This project involves a comprehensive cleaning and analysis of sales data for Speedline Wheels. The primary objective is to enhance understanding of customer relationships and prioritize interactions based on revenue generation. This analysis provides crucial insights into which clients contribute the most to the business and helps refine CRM strategies.  
Data was provided by Speedline Wheels, a business in Miami, Florida.

## Challenges Faced
The data cleaning process faced several challenges:
- **Incomplete Data Entries:** Many rows in the dataset had incomplete information, especially in the 'Business name' field, which only appeared at the first instance of each new business entry. This was due to the formatting of the reports that were sent to me.
- **Irrelevant Records:** Some records had zero amounts indicating no actual transaction. More understanding of the data was needed to conclude if the information needed to be taken into account or completely ignored.
- **Data Formatting:** Data in the CSV file had irregularities in the data types and made it problematic when working on the Pandas data frame since some data was not being detected. This could have been detrimental for the whole analysis because some amounts that were NOT being detected were very significant for the overall analysis. In the Jupyter notebook I documented how I went about fixing these issues.

    ![image](https://github.com/Lydionnn/Speedline-Wheels-Sales-Analaysis-Python-Tableau/assets/112720987/ddcdb6d0-28fb-4ef9-97f3-564f0db14045)

The NaN values ended up being present in the CSV files which made us idenfify what the problem was and how to fix it. 
This was documented on the '' Jupyter notebook for the project showing the data cleaning process and analysis.
![image](https://github.com/Lydionnn/Speedline-Wheels-Sales-Analaysis-Python-Tableau/assets/112720987/b582bd47-c248-43a3-b118-6b08fc4b6978)

![image](https://github.com/Lydionnn/Speedline-Wheels-Sales-Analaysis-Python-Tableau/assets/112720987/94cf7d2a-b58b-4ba5-a3e4-926a08ae48a7)

This was corrected by creating a function to enforce a uniform data type upon import, using converters in pandas.read_csv. This can ensure that all entries are read as strings first, which you can then clean and convert to numeric formats.

![image](https://github.com/Lydionnn/Speedline-Wheels-Sales-Analaysis-Python-Tableau/assets/112720987/1b916ba6-7c7d-41e2-9da9-f78afc60d542)


## Key Findings
- **Repeated Buyers:** By analyzing the frequency of transactions by unique dates, we identified key repeated buyers. This insight is critical for understanding which relationships are probably the strongest and could be the ones targeted with more focus for bigger deals, since there is already trust between the business and the clients.

    ![image](https://github.com/Lydionnn/Speedline-Wheels-Sales-Analaysis-Python-Tableau/assets/112720987/8da24882-5ca6-4911-b07d-396f971771c3)

- **Top Revenue Generating Clients:** The analysis highlighted the top clients based on revenue, which revealed the significant contributors to the business's sales. These clients are essential for targeted marketing and sales strategies.

    ![image](https://github.com/Lydionnn/Speedline-Wheels-Sales-Analaysis-Python-Tableau/assets/112720987/b4c70d36-aac2-4e3a-be81-d52ca95cc19a)





## Importance to CRM Improvement
The insights derived from this project are invaluable for refining the CRM approach:
- **Prioritizing High-Value Clients:** Understanding which clients bring in the most revenue allows the business to allocate resources effectively and prioritize high-value relationships.
- **Customized Interactions:** With a clear view of the sales history and client importance, the company can tailor its interactions to enhance client satisfaction and retention.
- **Strategic Decision Making:** The cleaned and analyzed data supports more informed decision-making, helping the business to strategize its sales and marketing efforts more effectively.

## Tableau Dashboard

### The full interactive dashboard can be accessed here: https://public.tableau.com/app/profile/fernando.amaya7973/viz/SpeedlineSales/SpeedlineDashboard

![dashboard](https://github.com/Lydionnn/Speedline-Wheels-Sales-Analaysis-Python-Tableau/assets/112720987/9fd44711-dba3-45fa-b5c8-334784a00b2e)


The Tableau dashboard designed for this project offers a dynamic and detailed visualization of key performance indicators (KPIs) such as the quantity of products sold, and total revenue generated (As requested by the client). Through this dashboard, a distinct correlation between the quantity of products purchased by a company and the corresponding revenue contribution to Speedline Wheels is clearly illustrated. This analysis not only highlights transactional data but also underscores the financial impact of each client's purchasing behavior.
Although this is a very simple Dashboard, they are able to navigate it and answer the main questions they had about their top customers in terms of revenue and also repeated customers. 
Additionally, a temporal analysis was conducted, showcasing sales trends by day of the week. This serves as a proof of concept that similar analyses could be extended to larger datasets, such as quarterly sales trends, to further enhance strategic planning.

Two critical insights were derived from the dashboard:
- **Client Revenue Contribution:** The dashboard visually represents the percentage of total revenue generated by each client. This visualization is pivotal in recognizing the disproportionate value derived from a select few clients. For instance, it was observed that three clients alone might contribute over 50% of total revenue, while another ten clients combined only account for 40%. Such insights are crucial for prioritizing where to allocate time and resources, emphasizing the importance of nurturing relationships with high-value clients.

    Snippet of dashboard: 
    ![image](https://github.com/Lydionnn/Speedline-Wheels-Sales-Analaysis-Python-Tableau/assets/112720987/7b788d4c-eaf4-427a-b609-3ebd4f595edd)


- **Top Customers Interaction:** An interactive chart of the top 10 customers allows users to explore and understand which clients are most crucial to Speedline Wheels. This interactive feature is essential for making data-driven decisions, helping stakeholders identify and focus on top revenue-generating clients, whether they be the top 5 or top 10.

    Snippet of dashboard: 

    ![image](https://github.com/Lydionnn/Speedline-Wheels-Sales-Analaysis-Python-Tableau/assets/112720987/5de46e01-3644-40dc-b588-37babba611c3)

These visualizations play a key role in guiding future strategic decisions, enabling Speedline Wheels to optimize its engagements and focus on the most profitable client relationships.

## Importance of Dashboard Insights in CRM Strategies

## Actionable Suggestions for Speedline Wheels
To leverage the insights gained from this project effectively, the following actionable suggestions are proposed for Speedline Wheels:
- **Client Segmentation and Prioritization:** Utilize the data to segment clients based on their revenue contribution and purchasing patterns. Develop targeted strategies for high-priority segments, focusing on personalized engagement and retention plans.
  
- **Enhanced Sales Targeting:** For future analysis we could focus on implementing predictive analytics to forecast future buying behaviors based on historical data and use this information to create targeted marketing campaigns and promotional offers that are likely to resonate with each segment.
  
- **Customer Relationship Development:** Invest in relationship management tools and training for sales representatives to ensure that interactions with high-value clients are consistently excellent. This could include more frequent communication, personalized service options, and first access to new products or services.
  
- **Feedback Loops and Continuous Improvement:** Establish regular feedback loops with key clients to gather insights into their needs and perceptions of the service provided. Use this feedback to continuously improve product offerings and customer service strategies.
  
- **Leveraging Temporal Sales Trends:** Utilize the temporal analysis from the dashboard to adjust inventory and staffing strategically around peak times of the week or in the bigger picture peak time of the year. This would that the business is well-prepared to handle fluctuations in demand efficiently.
