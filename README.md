# Pump-it-Up-Data-Mining-the-Water-Table
**Goal**
The primary objective of this project is to predict which water pumps are faulty to promote better access to clean, potable water across Tanzania. The dataset provides information on various factors influencing the functionality of waterpoints, such as the funder, installation date, geographic location, and water quality. Understanding these elements helps prioritize maintenance efforts, ensuring continuous access to clean water in affected areas
**Dataset Description**
The dataset contains various features that provide critical insights into the functionality of waterpoints. Here's a summary of key columns:
1) amount_tsh - Total static head (amount water available to waterpoint)
2) date_recorded - The date the row was entered
3) funder - Who funded the well
4) gps_height - Altitude of the well
5) installer - Organization that installed the well
6) longitude - GPS coordinate
7) latitude - GPS coordinate
8) wpt_name - Name of the waterpoint if there is one
9) num_private -
10) basin - Geographic water basin
11) subvillage - Geographic location
12) region - Geographic location
13) region_code - Geographic location (coded)
14) district_code - Geographic location (coded)
15) lga - Geographic location
16) ward - Geographic location
17) population - Population around the well
18) public_meeting - True/False
19) recorded_by - Group entering this row of data
20) scheme_management - Who operates the waterpoint
21) scheme_name - Who operates the waterpoint
22) permit - If the waterpoint is permitted
23) construction_year - Year the waterpoint was constructed
24) extraction_type - The kind of extraction the waterpoint uses
25) extraction_type_group - The kind of extraction the waterpoint uses
26) extraction_type_class - The kind of extraction the waterpoint uses
27) management - How the waterpoint is managed
28) management_group - How the waterpoint is managed
29) payment - What the water costs
30) payment_type - What the water costs
31) water_quality - The quality of the water
32) quality_group - The quality of the water
33) quantity - The quantity of water
35) quantity_group - The quantity of water
36) source - The source of the water
37) source_type - The source of the water
38) source_class - The source of the water
39) waterpoint_type - The kind of waterpoint
40) waterpoint_type_group - The kind of waterpoint

**Distribution of Labels**
The labels in this dataset are simple. There are three possible values:
1) functional - the waterpoint is operational and there are no repairs needed
2) functional needs repair - the waterpoint is operational, but needs repairs
3) non functional - the waterpoint is not operational

**Missing Values and Imputation**
One of the challenges of working with this dataset is handling missing data. Several columns, such as funder, installer, and scheme_name, have missing values, which can significantly impact the analysis and model predictions. To address this, imputation techniques were used:

1) Numerical Variables: Missing values in numerical fields (like amount_tsh or gps_height) were replaced with median values or other 
   relevant statistics depending on the variable distribution.
2) Categorical Variables: For missing categorical data (like funder or installer), the mode or a category called "Unknown" was used to 
   handle missing values effectively.

These imputation strategies ensured that no critical data points were lost during analysis while maintaining the integrity of the dataset for predictive modeling.
   
