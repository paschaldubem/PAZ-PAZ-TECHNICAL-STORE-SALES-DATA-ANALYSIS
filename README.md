# PAZ-AND-PAZ-TECHNICAL-STORE-SALES-DATA-ANALYSIS


# TABLE OF CONTENTS
- [BACKGROUND](#background)
- [DATA STRUCTURE](#data-structure)
- [EXECUTIVE SUMMARY](#executive-summary)
- [INSIGHTS DEEP DIVE](#insights-deep-dive)
- [RECOMMENDATIONS](#recommendations)
- [ASSUMPTIONS AND CAVEATS](#assumptions-and-caveats)
- [IN PROGRESS](#in-progress)
- [NEXT STEPS](#next-steps)



## BACKGROUND

Paz & Paz Technical Tool Store is a Nigerian-based retailer specializing in building materials and household tools, serving a wide range of customers from construction professionals to everyday homeowners in Lagos, Nigeria. They have been in operation for over a decade and are a traditionally analog business, managing their sales documentation through handwritten paper records.

They experience a fairly common challenge many Nigerian SMEs encounter, which is an inability to track trends in sales and measure profit performance of the business in near real time or at all, as well as the inability to understand which products are driving growth due to fragmented handwritten sales records.

As the **Business Data Consultant**, my goal was to **digitize their analog record-keeping** [CLICK HERE](https://github.com/paschaldubem/PAZ-PAZ-TECHNICAL-STORE-SALES-DATA-ANALYSIS/blob/main/Raw%20sales%20records.jpg), build a **structured sales database**, and perform an in-depth data analysis to uncover actionable insights on sales, profit margins, and inventory efficiency.

This project report documents this end-to-end process with **the objective of transitioning the business from analog to digital data management**, uncovering insights that would help the company make informed decisions on inventory control, sales performance, and profitability optimization.



#### Insights and recommendations are provided on the following key areas:

1.	**Sales Performance Analysis**: Analyzing the prevalent sales trends and uncovering the existing profit margin driving the business
   
2.	**Product Performance**: Evaluating key products that significantly contribute to the business's bottom line and customer foot traffic in form of sales volumes 
   
3.	**Payment Preference Distribution**: An evaluation of customer behavior towards the available payment options.
   


For data privacy reasons limited access was granted to display a subset of records from the source data in the internal database used for my analysis 

A sample of the **Google Sheets sales management system** I built to digitize and analyze the data can therefore be accessed [HERE](https://docs.google.com/spreadsheets/d/1mCrLAiVWT02X35kcTT25Vh2haDWBIYO-xDRTetjax2Q/edit?usp=sharing)

An **Interactive PowerBI dashboard** used to report and explore key metrics and KPIs can be accessed [HERE](https://app.fabric.microsoft.com/view?r=eyJrIjoiMWY5MTc3OGMtNWE0Yy00ZWZkLWEwY2MtNTViMGQyOWU3YjMzIiwidCI6IjI5ZTg2YjVlLTVkMDctNGExNC1hZDQ0LWFiOTQ3NmUwZGE4NyJ9&pageName=30f08ec51ecdb0303240)



## DATA STRUCTURE

Paz and Paz’s main database structure consists of **four interconnected tables** in Google Sheets: **SALES, PRODUCTS, SUPPLIERS, and INVENTORY**, spanning 6 months with a total combined row count of 5000+ records. 

A description of each table is as follows:


**SALES DATABASE**: This consists of **22 unique columns and 4000+ records**, from real-time data entries and digitized from the handwritten sales book, described below

<img width="827" height="610" alt="SALES DATABASE" src="https://github.com/user-attachments/assets/2b64424f-a621-435d-a57c-3bc3d9c04825" />

Its entity relationship diagram:

<img width="1747" height="617" alt="SALES" src="https://github.com/user-attachments/assets/bbc6f179-50fa-48fc-bda4-4188ca552245" />


**PRODUCTS DATABASE**: This consists of **24 unique columns** and contains the Standardized product catalogue of over 1200+ unique items with assigned SKUs and categories described below

<img width="846" height="695" alt="PRODUCT DATABASE" src="https://github.com/user-attachments/assets/0eda0032-0e75-4174-8527-6cd72bdba440" />

Its entity relationship diagram:

<img width="1846" height="619" alt="PRODUCTS" src="https://github.com/user-attachments/assets/9b7b0db9-a446-4c41-9080-51b13edbe22c" />


**INVENTORY DATABASE**: This consists of **24 unique columns** with over 150+ unique records containing details of restocked product inventory described below

<img width="783" height="572" alt="INVENTORY DATABASE" src="https://github.com/user-attachments/assets/5cded665-f05b-4f37-9874-7d56b552584d" />

Its entity relationship diagram:

<img width="1859" height="613" alt="INVENTORY" src="https://github.com/user-attachments/assets/e0df144f-a6f1-4521-b78b-95a6fff7373f" />


**SUPPLIER DATABASE**: This consists of **9 unique columns** containing details of over **30+ suppliers** in the existing supply chain network described below

<img width="825" height="290" alt="SUPPLIER DATABASE" src="https://github.com/user-attachments/assets/4d058755-9d7a-4b20-8236-e101259b0531" />

Its entity relationship diagram:

<img width="1608" height="625" alt="SUPPLIER" src="https://github.com/user-attachments/assets/f4805f8e-618c-4aae-80b4-205a6a3e6dee" />



## EXECUTIVE SUMMARY 

### Overview of findings

Over **6 months of digitized  sales data**, especially Q3 2025, revealed three critical insights
1. Profit margins consistently fell **below the target 30%**, averaging **27% (965k)** in Q3 due to inconsistent pricing structures on key product revenue drivers.
   
2. Padlock products are ripe for investment, sitting at a perfect intersection, ranking within the **top 3 best product revenue drivers** (0ver **300k** in revenue in Q3) as well as the **top 5 best products with high sale volume** (**77 units** sold in Q3)
   
3. The supply chain inefficiencies in product delivery and inconsistent product naming conventions have caused data duplication and often product mismatch, which incurs extra logistics costs to rectify, which eats into your bottom line, causing an erosion of trust and lost profit opportunities.


This is an overview page from the PowerBI dashboard, more insights are highlighted throughout the report. 

But the full interactive dashboard report can be previewed [HERE](https://app.fabric.microsoft.com/view?r=eyJrIjoiMWY5MTc3OGMtNWE0Yy00ZWZkLWEwY2MtNTViMGQyOWU3YjMzIiwidCI6IjI5ZTg2YjVlLTVkMDctNGExNC1hZDQ0LWFiOTQ3NmUwZGE4NyJ9&pageName=30f08ec51ecdb0303240)

<img width="1515" height="851" alt="SALES REPORT" src="https://github.com/user-attachments/assets/bf2748a7-0fda-4a51-93bc-351e59d91f1f" />

<img width="1308" height="749" alt="PRODUCT REPORT" src="https://github.com/user-attachments/assets/b31c5418-9750-4b5e-ac42-bcdca00f0e95" />



## INSIGHTS DEEP DIVE 

### SALES PERFORMANCE ANALYSIS

<img width="1486" height="555" alt="Screenshot 2025-10-24 235621" src="https://github.com/user-attachments/assets/dbade630-d4c9-4337-987c-c110ef01ae78" />

1. In Q3 alone, Paz and Paz Tech stores’ profit margin averaged 27% (965k), underperforming its benchmark of 30% due to products like door keys, which are key revenue drivers averaging a profit margin of just **18%**

2. Average monthly sales value consistently surpassed **₦1m in Q3**, indicating strong upward trajectory from Q2 (800k)

<img width="642" height="220" alt="Screenshot 2025-10-25 004227" src="https://github.com/user-attachments/assets/39d42da3-839b-42af-a615-0dd4a135b8fe" />

3. **Thursday** recorded the highest sales volume in Q3, representing **23% of total sales**

<img width="652" height="295" alt="Screenshot 2025-10-25 000235" src="https://github.com/user-attachments/assets/24a20655-33b4-4425-bf47-ee79f81a6599" />

4. **Bolts and nuts** have had some of the highest profit margins (**45%+**), which, though likely bumped up the overall average, offers a potential for better margins and pricing strategies.


### PRODUCT PERFORMANCE:

<img width="1308" height="749" alt="PRODUCT REPORT" src="https://github.com/user-attachments/assets/b92afc0d-8912-492f-a721-5ffbf38c338e" />

1. Screws (214 units), padlocks (77 units), nails (145 units), and bolts and nuts (132 units) consistently ranked among the top 5 most frequently sold items month-over-month. contributing significantly to customer foot traffic to the business.

2. Padlocks performed best in Q3, balancing high sale volume (77 units sold in Q3) and high sales value (313k revenue generated in Q3), simultaneously making it a key product of interest ripe for investment in the coming months.

3. Battery terminals, taps, and fasteners showed low turnover in Q3, tying up valuable inventory and capital without contributing significantly to sales or profit.


### PAYMENT PREFERNECE DISTRIBUTION:

<img width="401" height="214" alt="Screenshot 2025-10-25 003624" src="https://github.com/user-attachments/assets/2149133f-e311-4d9f-9270-fad817cc8b52" />

1. Mobile transfer constituted **over 44%** of all customer payments, with cash following closely behind at **30%** and POS being at **22%** in Q3

<img width="436" height="238" alt="Screenshot 2025-10-26 223906" src="https://github.com/user-attachments/assets/834fe694-35b5-42d9-b18f-5ccc08fdb218" />

2. POS payments are growing steadily, reaching 34% of all transactions in October alone, signaling a customer trend toward cashless options.


##
   
## RECOMMENDATIONS 

Based on the insights above, the following actions are recommended for **management and operations teams**:

1.	**Optimize Profit Margins**:
   - Adjust the pricing to stabilize margins on high-demand products like door keys and padlocks, modelling them after products like bolts and nuts with margins of over 40%+ to achieve the minimum overall 30% benchmark.
   - Reevaluate supplier contracts to terminate your agreement with those guilty of constantly delivering faulty products that erode customer trust and negatively impact profit margins stability

2.	**Invest in High-Performing Products**:
   - Increase promotions and investments in padlocks, door keys, bolts, and nuts due to their strong sales numbers in Q3 to improve turnover and company bottom line profit.
   - Prioritize restocking high-demand, fast-moving products, specifically black drywall screws (6x1¼", 6x1½", and 6x1"), concrete nails (2", 3", and 4"), and bolts and nuts (10x3/4" and 10x1") to bolster customer foot traffic into the store.

3.	**Reduce Inventory Inefficiencies**:
   - Phase out underperforming items (battery terminals, taps, fasteners) that tie up inventory.

4.	**Digital Payment Integration**:
   - Improve customer payment experience by investing and adopting digital-first strategies (POS upgrades, QR-based transfers).

5.	**Strengthen Supply Chain Management**:
   - Improve supply chain standards by introducing supplier performance tracking to curtail poor supply practices and enforcing product labeling (SKU) standards.

6.	**System Continuity**:
   - Be sure to maintain the Google Sheets database in pristine condition to ensure Power BI integration remains stable.
    


## ASSUMPTIONS AND CAVEATS 

Throughout the project, several challenges and assumptions were made to maintain data accuracy and scalability and ensure smooth system adoption

1.	**Product Categorization**: No pre-existing categories existed; all were created from scratch.

2.	**Product Naming Convention**: 90% of product names were inconsistent, so a standardized product naming convention system (SKU) was designed and manually assigned.
   
3.	**Incomplete Sale Records**: 95% of paper-based sales records (click here) were incomplete, which caused product mismatch and confusion, so I had to build an expansive, adaptable, and scalable product database.
   
4.	**System Performance**: The Google Sheets interface performance degraded with scale; optimization and periodic maintenance were necessary.
   
5.	**Automation Reliability**: Some Google Apps Script automations required manual intervention during system downtime

6.	**Sensitive Connection**: The Power BI connection to Google Sheets was fragile and so dependent on the data in the database being clean before visuals could be refreshed.

7.	**Data Accuracy**: Handwritten data errors occasionally caused price discrepancies, which were flagged and corrected

8.	**System Adoption**: Staff required orientation and gradual adaptation to digital systems.


## IN PROGRESS
Building a sales reporting AI agent to send out daily summarized sales breakdowns to relevant stakeholders, enabling near real-time remote monitoring. View MVP below:

<img width="1632" height="892" alt="paz" src="https://github.com/user-attachments/assets/b6321a98-7e6e-4e01-a081-fde0f25931f7" />


## NEXT STEPS
1. Transition from Google Sheets to MySQL/PostgreSQL backend for scalability.
2. Implement live Power BI dashboards with automated refresh triggers.
3. Develop a mobile interface for daily digital entry.
4. Introduce predictive analytics for demand forecasting.
5. Expand the system to serve other SMEs


