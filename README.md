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
- Understand the transaction volume by property types (Detached, Semi-Detached, Terraced and Flat) in London and the boroughs
- Identify price trends and growth patterns across years 
- Compare market dynamics across different borough price segments
- Analyse the data of buroughs in three different price ranges
- Provide data-driven insights
  
<h2 align="center"> 🔍 Exploratory Data Analysis (EDA) </h2>

### Data Loading and Overview
It is a clean dataset with 100,000 rows.
This data has 100,000 rows. The  null values are checked. The null values in some of the address columns are not required to locate the property. They do not affect this analysis. 
The EDA was started with Python methods: <br>
hsd.head(20)<br>
hsd.tail()<br>
### Summary Statistics
hsd.describe()

<img width="496" height="369" alt="image" src="https://github.com/user-attachments/assets/262b7cc8-0bcf-4908-826c-31ee5697682e" /> <br>
 
The districts in the dataset refer to the 32 borroughs of London. The districts have been used to segment the property analysis.  

<img width="872" height="568" alt="image" src="https://github.com/user-attachments/assets/cbb85d09-6dee-4f6d-a0e2-407b9c8ef9ab" />  

From the image generated above, the boroughs with the highest transaction volume can be seen. <br>
Highest Sales Volume by Property Types: Flats  
Then terraced, then semi-detached and the least sales are that of detached houses. <br>

The average price of a property is then compared.

<img width="852" height="579" alt="image" src="https://github.com/user-attachments/assets/9f92406f-d0de-42a0-9941-414690be2ef4" />

To achieve the objective of comparing the market dynamics across different borough price segments, first thing was to choose three different boroughs which represent the different socio-economic zones in London.
The above two charts were used in conjunction to decide which three boroughs should be analysed to get a sense of the property market in London. The boroughs are chosen such that one lies in low socio-economic area, seccond one in a middle socio-economic area and the third in a high socio-economic area in London.  
Greenwhich was chosen as it has a large sales volume and has properties in the comparatively lower socio-economic area as shown by the price graph above.  
The second borough chosen was Barnet in the middle socio-economic area, it has sizeable sales volume and I live here!  
The third borough chosen is Kensinton and Chelsea which has one of the most expensive properties in London. <br>

### Filter Data for Greenwich

Most expensive property (Detached House) in Greenwich: £ 3,300,000  
Least expensive property (flat) in Greenwich: £ 78,000 <br>
Some statistical data regarding the property sales filtered for Greenwich:  <br>

<img width="157" height="224" alt="image" src="https://github.com/user-attachments/assets/c6f00f6a-5d77-4935-bd43-33d766f08546" /> <br>

<img width="840" height="416" alt="image" src="https://github.com/user-attachments/assets/a0ebf695-04a7-42cf-9e65-e6b4e9add74c" />  

The sales volume in each year split up by property type.

### Filter Data for Barnet

Most expensive property (Detached House) in Barnet: £18,300,000  <br>
Least expensive property (semi-detached House) in Barnet: £20,000  <br>
Some statistical data regarding the property sales filtered for Barnet: <br>

<img width="167" height="227" alt="image" src="https://github.com/user-attachments/assets/e2105586-f236-4844-b17e-4be9c0026e19" /> <br>

<img width="729" height="366" alt="image" src="https://github.com/user-attachments/assets/68e1f180-4eff-4c57-8fb2-1a739c380b97" /> <br>

The sales volume in each year split up by property type. <br>

### Filter Data by Kensinton and Chelsea  

Most expensive property (Terraced House) in Kensinton and Chelsea: £33,000,000  <br>
Least expensive property (Flat) in Kensinton and Chelsea: £13,500  <br>
Some statistical data regarding the property sales filtered Kensinton and Chelsea: <br>

<img width="168" height="233" alt="image" src="https://github.com/user-attachments/assets/4acd6652-00fc-43bd-afe3-d6a71e740412" /> <br>


<img width="814" height="416" alt="image" src="https://github.com/user-attachments/assets/fcb665db-9641-458f-ad4a-cc06502c99cb" />

The sales volume in each year split up by property type. <br>

### Historical Property Price Trends in London and Chosen Boroughs

**Average London Property Sales Price in the Last Decade** <br>
GBP vs Year <br>
<img width="833" height="426" alt="image" src="https://github.com/user-attachments/assets/4b05a1b4-b2c5-4edb-83f0-3b302d6ffe42" /> <br>

**Average Greenwich Property Sales Price in the Last Decade** <br>
GBP vs Year <br>
<img width="839" height="436" alt="image" src="https://github.com/user-attachments/assets/77fd570a-0517-41a2-aefc-27e1357b8d58" /> <br>

**Average Barnet Property Sales Price in the Last Decade** <br>
GBP vs Year <br>

<img width="876" height="439" alt="image" src="https://github.com/user-attachments/assets/6bbbd68c-5947-4d5d-9954-4055a91e4ad3" /> <br>

**Average Kensinton and Chelsea Property Sales Price in the Last Decade** <br>
GBP vs Year <br>

<img width="870" height="428" alt="image" src="https://github.com/user-attachments/assets/3778e1cf-f198-4923-8d5c-14a15fe1450e" /> <br>

The above four line graphs show the average property price trends in the last decade. The graph which depicts average London prices shows stable growth throughout.
However, there's a fall in the average price from 2023 onwards. In the Borough of Greenwich, there's stable growth till 2022 and after that there's volatility.
In the Borough of Barnet, the property market shows a lot more volatility in the earlier years till 2019, after which there's sharp growth, the a decline in process from 2024 onwards.
In Kensington and Chelsea, there is the most amount of fluctuation with prices decreasing from 2018 to 2021, an increase till 2022, then there's been a decrease ever since.

<h2 align="center">🗝️ Key Insights </h2>

- Property market is dominated with flats- 68% of the total sales, followed by terraced houses which are 23.7%, then semi-deatched houses which make up 6.6% and only 1.8% of total houses make up for the sale of detached houses.
- There is a sizeable variation between the prices of the properties in different boroughs in London. The Central Boroughs have significantly higher priced properties. the maximum price of a property in Greenwich is 10 times less than the maximum price in Kensington and Chelsea.  
- 



