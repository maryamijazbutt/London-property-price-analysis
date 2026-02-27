<h1 align="center">London-property-price-analysis</h1>
Data analysis project showcasing: Using Python (Pandas, Matplotlib) to depict time series analysis, data visualisation, statistical computation and market segmentation. Analyses 10 years of London property data with borough level insights. 
Analysis Of London Property Prices From 2015-2025 

The data was downloaded from the following link https://landregistry.data.gov.uk/app/ppd/?relative_url_root=%2Fapp%2Fppd   
This data that was analysed includes the sales of all the properties in London for the past ten years.  
<h2 align="center"> ⚙️ How to Run This Notebook </h2>  
1. Download your own copy of the data:  <br>

- Go to https://landregistry.data.gov.uk/app/ppd/?relative_url_root=%2Fapp%2Fppd  <br>
- Set Town/City = London  <br>
- Set date range: 30/11/2015 to 30/11/2025  <br>
- Click "Get all results as CSV with a header"  <br>    
2. Upload the CSV file to your Google Drive   <br>
3. Open the notebook in Google Colab <br> 
4. Update the file path in the data loading cell (e.g. `/content/drive/MyDrive/pp-complete.csv`)  <br>
5. Run all cells  <br>

<h2 align="center"> 📊 Project Overview </h2>  

This project uses the data from UK's land registry website and provides a data-driven analysis of London's residential property market over the last decade, examining price trends, property type distribution, and borough-level variations. It uncovers key insights about London's housing landscape, identifies growth patterns, price disparities and market segmentation across different property categories and boroughs. 

<h2 align="center"> 🎯 Key Objectives </h2>

- Analyse the evolution of London's property market from 2015 to 2025 
- Understand the distribution of property types(Detached, Semi-Detached, Terraced and Flat) 
- Identify price trends and growth patterns across years 
- Compare market dynamics across different borough price segments
- Analyse the data of buroughs in three different price ranges
- Provide data-driven insights
  
<h2 align="center"> 🔍 Exploratory Data Analysis (EDA) </h2>

The EDA was started with Python methods <br>
hsd.head(20)<br>
hsd.tail()<br>
## Summary Statistics
hsd.describe()

<img width="496" height="369" alt="image" src="https://github.com/user-attachments/assets/262b7cc8-0bcf-4908-826c-31ee5697682e" />
