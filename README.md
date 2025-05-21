# Optimizing Warehouse Supply Allocation for FMCG Instant Noodles Company 🍜
This project analyzes the mismatch between demand and supply in FMCG warehouses using a combination of Python and Power BI. The analysis is done using descriptive, diagnostic, and prescriptive analytics approaches to optimize product distribution and warehouse efficiency. The results are visualized in an interactive dashboard as a management decision-making tool.
## 1. Background Information 📋
FMCG companies that have only been in the instant noodle business for two years are experiencing a mismatch between demand and supply of products in various warehouses. When demand is high, supply is low, and vice versa. This causes significant inventory cost losses. 
Therefore, management wants to understand more deeply the demand patterns and warehouse conditions in 
various regions in order to optimize product distribution.
## 2. Project Objective 🎯
Perform historical data analysis to: <br>
• Identify product demand patterns by region, location type, and 
warehouse characteristics. <br>
• Diagnose factors causing demand and supply mismatch. <br>
• Provide data-driven recommendations to optimize supply allocation and 
support managerial decision making through interactive dashboards. <br>
## 3. Business Questions & Analysis Method 🤔❓
### A. Zone and Location 🗺️  
• Q: Which zone or region most often experiences mismatch between warehouse capacity and product weight shipped?  
→ Descriptive + Diagnostic  
• Q: Does the location of the warehouse in a village or city affect the amount of product distribution?  
→ Descriptive + Diagnostic  
### B. Warehouse Capacity & Utilization 🏛️  
• Q: How optimally is the warehouse utilized (calculated from the ratio of product_wg_ton to 
WH_capacity_size)?  
→ Prescriptive  
• Q: Which warehouses are overused (exceeding ideal capacity) or underused?  
→ Diagnostic + Prescriptive  
### C. Logistics and Transportation 🚚  
• Q: Do warehouses with a history of transportation issues (transport_issue_l1y) have
lower shipments?  
→ Diagnostic  
• Q: How much does dist_from_hub affect the weight of products shipped?  
→ Diagnostic  
### D. Environment & Infrastructure  🏢
• Q: Do flood-impacted or non-flood-proof warehouses tend to have lower shipments?  
→ Diagnostic  
• Q: Is the presence of electric_supply or temp_reg_mach related to warehouse performance in product distribution?  
→ Diagnostic  
### E. Warehouse Activity 🏪  
• Q: Do warehouses that experience frequent refills (num_refill_req_l3m) also receive 
greater supplies?  
→ Descriptive + Diagnostic  
• Q: Does the number of distributors (distributor_num) have an impact on the total shipments 
of products to the area?  
→ Diagnostic  
• Q: How much influence does wh_breakdown_l3m have on the decline in supplies to the warehouse?  
→ Diagnostic  
### F. Market Competition 🛒  
• Q: Does the number of competitors (Competitor_in_mkt) affect the number of products shipped to an area?  
→ Diagnostic  
• Q: Which areas have market potential (few competitors, many retailers) but supply is still low?  
→ Prescriptive (opportunity mapping)  
### G. Certification and Compliance 📜  
• Q: Do warehouses with a certain approved_wh_govt_certificate have higher distribution performance?  
→ Descriptive  
• Q: Does the number of government inspection visits (govt_check_l3m) affect the supply to that warehouse?  
→ Diagnostic  
### H. Warehouse Eligibility & Age 📆  
• Q: Do warehouses built longer (wh_est_year) tend to have more problems and lower deliveries?  
→ Diagnostic  
### I. Combination of Factors 🕵  
• Q: What combination of factors (location, capacity, number of distributors, transportation) is most ideal
to support high shipments?  
→ Multivariate Diagnostic  
• Q: Zones with ideal conditions (safe from flooding, adequate electricity, smooth distribution) but
supply is still low – why?  
→ Prescriptive  
## 4. Data Understanding 📊  
This dataset consists of 25000 rows and 24 columns.  

**Information for each column**

- Ware_house_ID = Product warehouse ID  
- WH_Manager_ID = Employee ID of warehouse manager  
- Location_type = Location of warehouse like in city or village  
- WH_capacity_size = Storage capacity size of the warehouse  
- zone = Zone of the warehouse  
- WH_regional_zone = Regional zone of the warehouse under each zone  
- num_refill_req_l3m = Number of times refilling has been done in last 3 months  
- transport_issue_l1y = Any transport issue like accident or goods stolen reported in last one year  
- Competitor_in_mkt = Number of instant noodles competitor in the market  
- retail_shop_num = Number of retails shop who sell the product under the warehouse area  
- wh_owner_type = Company is owning the warehouse or they have get the warehouse on rent  
- distributor_num = Number of distributer works in between warehouse and retail shops  
- flood_impacted = Warehouse is in the Flood impacted area indicator  
- flood_proof = Warehouse is flood proof indicators. Like storage is at some height not directly on the ground  
- electric_supply = Warehouse have electric back up like generator, so they can run the warehouse in load shedding  
- dist_from_hub = Distance between warehouse to the production hub in Kms  
- workers_num = Number of workers working in the warehouse  
- wh_est_year = Warehouse established year  
- storage_issue_reported_l3m = Warehouse reported storage issue to corporate office in last 3 months. Like rat, fungus because of moisture etc.  
- temp_reg_mach = Warehouse have temperature regulating machine indicator  
- approved_wh_govt_certificate = What kind of standard certificate has been issued to the warehouse from government regulatory body  
- wh_breakdown_l3m = Number of time warehouse face a breakdown in last 3 months. Like strike from worker, flood, or electrical failure  
- govt_check_l3m = Number of time government Officers have been visited the warehouse to check the quality and expire of stored food in last 3 months  
- product_wg_ton = Product has been shipped in last 3 months. Weight is in tons
## 5. Exploratory Data Analysis 📈  
## 6. Data Cleaning & Transformation 🧹🧼✨  
## 7. Visualization Strategy (Power BI Dashboard) 📊📈  
## 8. Insights & Recommendations ✨💡  
## 9. Conclusion & Next Step ✅➡️❓  
