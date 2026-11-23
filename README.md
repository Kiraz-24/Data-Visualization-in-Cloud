# Data-Visualization-in-Cloud
Introduction 
This project has involved using Microsoft Azure and Power BI to gain an understanding of sales 
performance across regions in New Zealand. Azure was used to structure our cloud resources, and to 
store the Excel sales data. We then played around with the data in Power BI to make a dashboard 
displaying the revenue, profit, profit margin, sales channels, cities, and products. The primary goal 
was to understand and learn how cloud services and business intelligence tools could be combined. 
Azure allowed us to manage the data in the cloud and Power BI allowed us to transform sales into 
charts that were easier to comprehend.  
The objectives of the project are to:  
• Setup and develop a resource group, virtual machine and storage account on Azure.  
• Upload New Zealand Sales Excel file to Azure Blob Storage.  
• Link the data stored in azure blob to Power BI and make the data ready for analysis.  
• Create a dashboard and determine valuable sales and profitability information.  
Tools and dataset  
We used Azure for Students subscription, Azure Resource Manager, an Ubuntu virtual machine, 
Azure Blob Storage and Power Query Editor and Power BI Desktop. Orders, Customers, Regions and 
Products sheets are included in the Excel workbook.
Creating the Azure Resource Group 
We had opened a resource group, which is the first task in Azure. It is a folder that helps to organize 
various cloud services. This makes it easier to manage as the virtual machines and storage resources 
are at one place.  
out 
the 
We logged into the Microsoft Azure portal, searched for Resource group, clicked on Create, and 
filled 
necessary 
details. 
The name of the resource group was 
New_Zealand_Regional_Sales_Performance. We had chosen the Azure for Students subscription and 
East Asia location.  
The resource group helps to track resources, control access, and monitor costs. So, by creating a 
resource group for our project, we were able to keep all the related Azure services under one name, 
making the project easier to handle. 
Creating the Virtual Machine 
Next, we had created a virtual machine (VM) in Azure. A virtual machine is a virtual computer 
located in the cloud. It can be used to execute software, test applications and perform computer 
operations without requiring a separate computer.  
We started the Azure virtual machine creation process and chose our resource group and named the 
VM as NZ-RegionalSales-VM. The VM was set up to have Linux (Ubuntu 22.04) and the Standard 
B2ats v2 size, with 2 virtual CPUs and 1 GiB of memory. VM was moved to East Asia. Azure 
indicated that the deployment was successful, and the VM overview indicated that its status was 
Running. A VM is helpful as it gives flexibility in working. It can be started, stopped and controlled 
via Azure.
Creating the StorageAccount and uploading data 
We created the storage account named nzregionalsales, which is of StorageV2 storage type, located 
in East Asia. Within the storage account, we created a Blob Storage container called nz-regionalsales. 
The box is used to store files in Azure. We uploaded the Excel workbook to the container: New 
Zealand Regional Sales.xlsx.  
This was essential because it transferred the sales information from a local file to cloud storage. 
Cloud storage allows us to keep all our project files in one place and access them whenever needed 
with the required permissions. It also helps us share data easily and manage files throughout the 
project.
Connecting Azure data to Power BI 
The data was stored in the cloud, the next step is to connect them into Power BI. Power BI is a tool 
that helps us to create interactive charts from tables of data. Using Power BI's data connection 
process, we've connected to Azure Blob Storage. Next, the data was opened using Power Query 
Editor to view the file and ready for reporting.  
The project data was divided into four tables in Power Query: Sales_Data, Customer_Data, 
Regions_Table and Products_Data. These represent the sales transactions, customers, locations and 
products. Power BI relied on the imported columns and data types to work with the data. 
Create data models and dashboards 
Once the data has been prepared, we connected the sales table with the supporting tables in the Power 
BI Model view. The model shows "deliveryregion" and "region" in the Sales_Data to Regions_Table 
relationship, which is set to be many-to-one. This will enable values to be aggregated by the right city 
or region. 
In addition to this, Customer_Data and Products_Data are also shown in the model. Having separate 
tables for sales, customers, products and regions allows us to organize the information, and create 
different visuals without having to include all the information in one large table. 
We then developed a Retail Sales and Profitability Dashboard, so we had added the following cards 
to the top: Total Revenue, Total Profit, Profit Margin %. We then created charts below these that 
showed revenue by city, profit by product and revenue by sales channel. There are also channel filters 
on the dashboard to make comparisons with various segments of the business. 
The dashboard is a combination of both overall and detailed comparisons. This is helpful because an 
individual first gets the overview and then takes a look at the cities or products and/or sales channels 
that have produced the outcomes.
Dashboard Analysis, Findings and Conclusion 
Overall, the dashboard shows total revenue to be $154.57 million, total profit $57.79 million, and a 
profit margin of 37.39%. This shows that the business made approximately $37.39 in profit from 
$100 in revenues. The findings indicate that the business made a significant profit over the period 
analysed. 
Revenue by sales channel 
Wholesale generated more than any other source (around $83 million). This was followed by 
Distributor sales of approximately $49 million and Export of approximately $23 million. Therefore, 
wholesale is the biggest sales channel and very significant to overall revenues. 
Profit: by product, Revenue: by city 
Product 1 was the highest earning product at approximately $9.6 million with Product 7 just under 
about $9.5 million. Product 2 was next at about $8.7 million. The difference between the top products 
and the smaller products demonstrates that profits are not distributed equally among the range of 
products. 
In addition to showing differences in revenue, the city chart also shows differences in revenue by 
location. The top three cities had revenue of about $12.5 million, $12.0 million and $11.0 million, 
with several smaller cities having revenue close to $2 million. This implies that certain places are 
more significant to sales than others. The business may examine successful retail sites and identify 
how to enhance less successful types.
This project gave us a better idea of the process of setting up resources in the cloud to reporting to the 
sales team. We had learned how to create Azure resources, store an Excel file in Blob Storage, 
transform data in Power Query and use relationships and charts in Power BI. The dashboard helped to 
understand and gave insights about what are the best channels, products and locations for sales and 
profit.  
Recommended actions to improve profitability or sales performance 
• The company should focus on products like Product 1 and Product 7, as they are getting in 
higher profits. Keeping these products in stock and promoting them more can help increase sales. 
• The company should pay more attention in cities where sales were low. They can offer 
discounts and do promotions to attract more customers and improve sales. 
Benefits of using Cloud 
• Cloud storage makes it easier for businesses to store and access their data from anywhere 
without depending on a single computer. 
• The cloud works on a pay-as-you-use basis, so a company does not need to buy its own 
servers and can increase storage when the data grows. 
Risk of using Cloud 
• There is a chance that the data being accessed by unauthorized people if proper security 
measures are not taken. 
• Cloud services depend on internet connectivity, so a poor connection can make it difficult to 
access data or update reports on time.
