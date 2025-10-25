# PAZ-PAZ-TECHNICAL-STORE-SALES-DATA-ANALYSIS
This project report documents this end-to-end process with the objective of transitioning the business from analog to digital data management, uncovering insights that would help the company make informed decisions on inventory control, sales performance, and profitability optimization.

# TABLE OF CONTENTS
- [BACKGROUND](#background)
- [DATA STRUCTURE](#data-structure)
- [EXECUTIVE SUMMARY](#executive-summary)
- [INSIGHTS DEEP DIVE](#insights-deep-dive)
- [RECOMMENDATIONS](#recommendations)
- [ASSUMPTIONS AND CAVEATS](#assumptions-and-caveats)


## BACKGOUND

Paz & Paz Technical Tool Store is a Nigerian-based retailer specializing in building materials and household tools, serving a wide range of customers from construction professionals to everyday homeowners in Lagos, Nigeria. They have been in operation for over a decade and are a traditionally analog business, managing their sales documentation through handwritten paper records.

They experience a fairly common challenge many Nigerian SMEs encounter, which is an inability to track trends in sales and measure profit performance of the business in near real time or at all, as well as the inability to understand which products are driving growth due to fragmented handwritten sales records.

As the Business Data Consultant, my goal was to digitize their analog record-keeping, build a structured sales database, and perform an in-depth data analysis to uncover actionable insights on sales, profit margins, and inventory efficiency.
This project report documents this end-to-end process with the objective of transitioning the business from analog to digital data management, uncovering insights that would help the company make informed decisions on inventory control, sales performance, and profitability optimization.



#### Insights and recommendations are provided on the following key areas:

1.	Sales Performance Analysis: Analyzing the prevalent sales trends and uncovering the existing profit margin driving the business
   
2.	Product Performance: Evaluating key products that significantly contribute to the business's bottom line and customer foot traffic in form of sales volumes 
   
3.	Payment Method Distribution: An evaluation of customer behavior towards the available payment options.
   


For data privacy reasons limited access was granted to display a subset of records from the source data in the internal database used for my analysis 

A sample of the Google Sheets sales management system I built to digitize and analyze the data can therefore be accessed [HERE](https://docs.google.com/spreadsheets/d/1mCrLAiVWT02X35kcTT25Vh2haDWBIYO-xDRTetjax2Q/edit?usp=sharing)

An Interactive PowerBI dashboard used to report and explore key metrics and KPIs can be accessed [HERE](https://app.fabric.microsoft.com/view?r=eyJrIjoiMWY5MTc3OGMtNWE0Yy00ZWZkLWEwY2MtNTViMGQyOWU3YjMzIiwidCI6IjI5ZTg2YjVlLTVkMDctNGExNC1hZDQ0LWFiOTQ3NmUwZGE4NyJ9&pageName=30f08ec51ecdb0303240)


## DATA STRUCUTRE 

Paz and Paz’s main database structure consists of four interconnected tables in Google Sheets: SALES, PRODUCTS, SUPPLIERS, and INVENTORY, spanning 6 months with a total combined row count of 5000+ records. 

A description of each table is as follows:

SALES DATABASE: This consists of 22 unique columns and 4000+ records, from real-time data entries and digitized from the handwritten sales book, described below

<img width="827" height="610" alt="Screenshot 2025-10-24 221724" src="https://github.com/user-attachments/assets/61075b7e-f37b-4ecf-a597-210487f1c5e9" />


 ![2024 tender jpeg ](https://github.com/user-attachments/assets/3f403d88-5b29-47e0-a702-f255d7e902e3)


- CLIENT – Names of respective clients who send out tenders i.e. IOCs (International oil companies) and NOCs (National oil companies)
-	TENDER DESCRIPTION – Detailed names of tender received 
-	YEAR – Year the tracker was compiled 
-	DATE REC'D – Date tender was received by Makais 
-	DUE DATE dd/mm/yyyy – Deadline for submission of the tender 
-	TENDER DURATION – Difference between the due date and the received date indicating the length of time in days given to submit said tender.
-	DUE TIME – Time of day the tender submission expires 
-	CONTRACTING ENTITY (See Note 2) – The entity that received the tender 
-	PLATFORM RECEIVED	- The platform on which the tender is received 
-	TYPE OF PARTNERSHIP – The type of partnership leveraged to qualify to submit a bid for the received tender 
-	NIPEX NO. – Unique identifier for tender on NIPEX platform 
-	ITT NO.	- Unique identifier for the tender given by the client issuing the tender 
-	FORM OF ACKNOWLEDGEMENT DUE DATE – Deadline for submission of the form of acknowledgement document to confirm interest of Makais in bidding for the tender 
-	PRETENDER CLARIFICATION MEETING – Indicating whether the meeting set up to give further details on received tender would hold.
-	PRETENDER SITE VISIT - Whether there will be a facility inspection 
-	TENDER TYPE- Indicates the type of tender that was received 
-	RANK / NO OF DAYS LEFT – Tracks the number of days left to deadline  
-	BID STATUS – Indicates whether a bid was submitted or not 
-	PROJECT STATUS – Indicates whether a project was awarded or not.

## EXECUTIVE SUMMARY 

### Overview of findings

Over the years, Makais' bid submission rates were at an average of about 51% but dropped significantly below the statues quo to 32% in 2024 most probably due to operational inefficiencies or an experience gap caused by unavailable of the necessary product codes. 
CHEVRON stood out as a high-potential partner, having advertised 8 tenders in 2024 alone—44% of their historical total (18). 

Additionally, tender opportunities historically peak during the months of March, May, and July, a trend that held true in 2024 with the average tender duration at 52 days historically dropping to 23 days in 2024 alone. 

Below is an overview page from my PowerBI dashboard, more examples are included throughout the report. The dashboard can be previewed [HERE](https://app.powerbi.com/view?r=eyJrIjoiNzAyZTcyMmItZDY0ZS00MDM4LWJiZDItOWNiNzE3Y2NmODRhIiwidCI6IjI5ZTg2YjVlLTVkMDctNGExNC1hZDQ0LWFiOTQ3NmUwZGE4NyJ9)

![MAKAIS 2](https://github.com/user-attachments/assets/23ce382e-036f-4e09-a6a5-e1658030fae4)


## INSIGHTS DEEP DIVE 

### AVERAGE TENDER DURATION:
   
The average time between tender advertisement and the corresponding bid submission deadline is 52 days which dropped even lower to 23 days in 2024.
This insight underscores the importance of optimizing internal workflows to meet submission timelines.


![AVERAGE BID DURATION ](https://github.com/user-attachments/assets/89a1fcb2-f671-40f6-ac3d-6b5a23c593ab)

### TENDER OPPORTUNITY YEARLY AND MONTHLY TRENDS:
   
On record 2023 had the highest tender influx volume (63), showing consistent recovery since the COVID pandemic-induced low of 16 in 2020. This growth may be attributed to Makais’ increasing expertise and expanded product code inventory.

In 2024, on a month-on-month basis, July recorded he highest volume of tender opportunities at 12 closely followed by peaks in March (9) and May (8) this pattern conforms to monthly historical peaks in the months of May (30), March (30) and July (25).

![2023 most active year ](https://github.com/user-attachments/assets/1c9605ca-98bc-4fd2-9677-18be4e6c1be0)

![2024 year peaks  ](https://github.com/user-attachments/assets/c6d4bfe8-bb3f-47d7-9afb-c5dffe60184d)

![TENDER OPPORTUNITY DISTRIBUTION TREND ](https://github.com/user-attachments/assets/068c8f8c-6b31-44e7-bcf9-6b08bc3ec932)

### BID SUBMISSION RATE:
   
Makais has submitted bids for 52% of advertised tenders, with 37% not addressed and 5% left blank due to incomplete documentation.

In 2024 submitted bids for advertised tenders dropped significantly to 32%, while 61% of received tenders were not addressed. This deviation from the historical trend warrants deeper analysis to identify operational bottlenecks or external influences.

![BID STATUS BY % SUBMITTED ](https://github.com/user-attachments/assets/137f862d-8ff7-440e-831b-82eb20992067)

![BID STATUS BY % SUBMITTED 2024](https://github.com/user-attachments/assets/a6d3c393-a6b9-4b30-abea-1743d127a5e0)

### CLIENT ANALYSIS:
   
NPDC (Nigerian Petroleum Development Company) has been the most active client over the years with 40 bids advertised till date closely followed by SPDC at 28 and CHEVRON ranking the least at just 18. IOCs are seen more active than NOCs overall as 3 out of the top 5 oil companies are international based. 

In 2024 alone CHEVRON showed significant activity, advertising 8 tenders (44% of its historical total). This positions it as a key client with considerable growth potential. the IOCs still advertised more tender opportunities overall probably due to having more infrastructure in the oil sector.

![CLIENT BY NO OF BIDS RECEIVED ](https://github.com/user-attachments/assets/b573aa95-fe9b-4a77-a26b-e67cd06eda06)

![CLIENT BY NO OF BIDS RECEIVED 2024](https://github.com/user-attachments/assets/a055fc96-44e7-43c6-818b-1fdc3d31b487)

### CONTRACTING ENTITY ACTIVITY LEVELS:
   
Makais Synergy has been the most active entity over the years, by receiving a total of 196 tenders (70% of the total tenders ever received) demonstrating its extensive expertise in form of products codes over the other entities like Makais Engineering and International Limited (MEEIL) with just 69 tenders (just over 24% of the total)

In 2024 Makais Synergy retained its lead with 26 (59%) tenders, reinforcing its role as the flagship entity

 ![TENDER RECEIVED BY CONTRACTING ENTITY ](https://github.com/user-attachments/assets/7cf72d26-4ae0-4704-9b82-6ef5eb724266)


### PLATFORMS ACTIVITY:
   
The NIPEX portal accounts for 62% of all tenders received, solidifying its role as Makais’ primary source of opportunities. However, with a large number of blank data (31% incomplete entries) it introduces some uncertainty in the analysis.

In 2024, NIPEX usage surged to 81%, confirming its dominance. Other platforms like INFO and SYNERGY Mail remain marginal contributors.

![TENDER RECEIVED BY PLATFORM ](https://github.com/user-attachments/assets/f584b594-37d7-4095-860d-442c58c58007)


### TENDER TYPE EVALUATION:
   
Double envelope tenders are the predominant type though records started in 2020, it likely represents the industry tender standard. While blanks exist in the data, it is reasonable to assume double envelope tenders account for the majority.

In 2024 the trend was not any different as double envelope tenders remained dominant (91% of all tenders received), aligning with historical patterns.

![TENDER RECEIVED BY TYPE ](https://github.com/user-attachments/assets/b2e174d6-0990-467c-962e-db4cd5daa966)

## RECOMMENDATIONS 

Based on the uncovered insights, the following recommendations have been provided:
1.	With IOCs ranking higher than NOCs based on the volume of opportunities they provide, focusing on strengthening relationships with the key IOCs and growing partnerships with high-potential clients like CHEVRON have a higher likelihood for substantial financial returns due to access to more opportunities to pick from.
   
2.	The average tender duration shows a potential of shrinking (52 to 23 days) and should be used to set benchmarks for how strategies put up to optimize and streamline the bidding process are structured.

3.	The poor submission rates need to be addressed to identify operational bottlenecks in bid submission processes by revising submission workflows to improve its rates and reduce missed opportunities.

4.	Maintain resource readiness and optimize bidding capacity during high-opportunity months (March, May, July) to capitalize on cyclical trends.

5.	Further strengthening of Synergy’s capabilities while enhancing the capacity of less active entities like MEEIL by investing in purchasing product codes to diversify Makais’ capabilities and potential revenue streams.

6.	Prioritize NIPEX as the main platform for tender opportunities tracking while improving data entry processes for better documentation completeness to ensure accurate usage tracking of other platforms.
    
7.	Optimize and align operational workflows to handle the nuances of the dominant double-envelope tender type, to ensure compliance, operational efficiency and competitiveness.


## ASSUMPTIONS AND CAVEATS 

Throughout the analysis, multiple assumptions were made to manage challenges with the data. These assumptions and caveats are noted below:

1.	A disproportionate number of missing data in key columns 
  - 32% of platform received
  - 45% of tender type 
  - 23% of Tender duration columns

Which could potentially affect the final analysis; I went ahead with it nonetheless but prefixed the issue in my insights’ the higher the percentage of missing values the less reliable the final analysis would be.

2.	A fair amount of nonsensical data (scenarios where the due date is earlier than the tender received date) i.e. in the date received and due date columns which affected 23% of the tender duration column and had to be excluded from the analysis as a result.
   
3.	Conflicting information from other similar datasets like ‘GENERAL TENDER - NPDC ONLY (SUBMITTED)
   
4.	There were a lot of redundant data sets that carried very slightly different but incomplete information I had to reconcile with the source data before discarding.
   
5.	Bloated use of similar names in the Clients name column 





