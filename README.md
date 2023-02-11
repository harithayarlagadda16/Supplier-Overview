# Supplier-Overview
 Interactive Dashboard representing the overview of Raw Material Supply chain of Tier 1 and Tier 2 suppliers and Volume analysis of the Business involved in Manufacturing with sevaeral units all over india. The dashboard helps to understand the Business metrics and helps the Business team to understand make the Data driven decisions in risk management, cost cutting etc... 
# Business Case: 
The Accounts Department of the Company maintains the invoice level details of all vendors for each part procured. The Business Planner receives invoice data from the Accounts Department for each vendor and collects the supplier and part level information separately from the Purchase Department. The Business Planner has to study the relevant data and identify the Procurement trends, Supplier limitations, Product based supplier consolidation and minimise cost impact to company.

# Problem Statement: 
As the collected Data is of different years for multiple Plants grouped by different Business Units. The parts are either made of Aluminium or Ferrous of different raw material grade alloys, with the source being either Tier 1 supplier or Tier 2 supplier. Considering all these factors, create a dashboard which is insightful on all these factors and can help the Procurement Department make better supply chain strategic decisions.
# Steps:
The Data was in Excel Format connected to Power BI, Data Formatting and Preparation were done in Power Query Editor.
# Scenario: 1
Our task is to build a dashboard page and name it as “Supplier Overview”, which gives us a supplier status and its capabilities. Also, categorizing them as per the data provided in the data set. This will help the responsible Purchase Group (Buyer) get a focused quick insight for the suppliers.
# Approach:
-	This page of the report was completely dedicated to understand the supplier behaviour and overview of the supply chain. The individual tables were imported into BI and Data Model was created by creating the Key columns to Design the relationship. 
-	Visuals like Gauge chart for the supplier count, Donut chart to know the MSME type and Pie chart for the Strategy status were designed. Along with those to understand the demographics Map chart was used.
-	A table chart gave the detailed outlook on relationship between the Buyer, Payments terms and supplier information. Slicers with Business Unit, Part Group, were used to slice and understand the criteria.
-	Conditional Column was created using **DAX** to divide the materials into Ferrous and Non- Ferrous categories. To make the Commodity Column more personalised Chiclet Slicer was used and Images were used asper data.

# Scenario: 2
We would need another dashboard page and name it as “Volume Movement” to help analyse the Purchase volume and Tonnage volume movement throughout different years for past comparisons and business planning upcoming demands. We would need multiple filtering options as per business units, purchasing groups, Manufacturing plants, Part Family, supplier names, and raw materials.
# Approach:
-	This page of the report was used to understand the Volume analysis and Demand. A Master Report Table was created appending two tables and a relationship was established.
-	The slicers from the first page were synced and few more additional slicers like Plant, Mcr.mrt group, were created Commodity and Supplier name were used.
-	Visuals were plotted to understand the distribution with Purchase Volume against the Supplier name, Part family and Business Unit.
-	Tonnage was also calculated (DAX) with predefined Lookup value. Visuals were plotted to understand the Tonnage distribution.
-	Features like Edit Interactions, Tooltips, Buttons, Bookmarks were created and used to understand the story behind the Visuals.

# Learnings:
-	**Non-MSME** suppliers are basically the ones which have a **Turnover > 100cr (1000 million)**, lower than this will be classified into different types of MSME category. We have almost **5 suppliers where we cannot grow** business.
-	We have a forecast that the business for ferrous casting will reduce year on year, we would need to stop business in future with four **(AAPL, PAPL, MNI, ICPL)** of our ferrous casting suppliers as the demand starts coming down.
-	The Management wants us to minimize the risk with our suppliers, the **biggest NoGo Suppliers** that we have are **FBMPL** where the purchase volume is more with payment terms in 90 days.
-	We want to declutter the supply chain for our top 5 suppliers, we can decide to buy from one single source and negotiate for cost saving. **SPCIP group have more than one casting supplier**.
