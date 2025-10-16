# Specialty_tea_demand_forecasting
This application aims to forecast demand of specialty tea by choosing best statistical model. This forecasted demand is needed to place orders with warehouse in advance to avoid last minute hassles. Also, goods receipt process can be completed on time ensuring timely payment to vendors

SITUATION:
Specialty tea orders are placed to the warehouse close to production date and so this causes last minute hassles and possible stock outs & mistakes. Also, goods receipts and tea pallet labelling at warehouse is done close to the production date, causing incorrect pallet labelling and delivery delays.

TASK:
There is a need to accurately forecast demand so that last minute hassles can be avoided. Tea labelling and goods receipt can be prioritized according to the forecast

ACTION:
1. From SAP HANA, availability data for last 10 years and requirement for last 10 years is extracted using SQL queries to load directly to Power BI using direct query connection
   
   <img width="1842" height="858" alt="image" src="https://github.com/user-attachments/assets/9613db47-c832-46ff-99d4-f0003e32a197" />

   <img width="1856" height="878" alt="image" src="https://github.com/user-attachments/assets/d468942c-6c0a-4e81-90f6-5f03bc52fef2" />

   <img width="1916" height="1029" alt="image" src="https://github.com/user-attachments/assets/fe4c915a-12ed-4bac-ab20-fd20218c2021" />

2. Power Query Transformations are done to load the data in batches and then append it to a table. Then requirment and availability are merged to obtain the need of the material and this is displayed in a line chart.
   
   <img width="1350" height="544" alt="image" src="https://github.com/user-attachments/assets/eaee3c2d-e71d-4a86-b6f7-130e8e8de7a9" />

3. Python Script visual is used in Power BI and python code is used to compare different forecast models and obtain the most accurate one using Mean Absolute Percentage Error and Root Mean Square Errors.
   
   <img width="1403" height="902" alt="image" src="https://github.com/user-attachments/assets/e64897f6-af36-41d1-8f08-272dbd8177a8" />

   <img width="1785" height="984" alt="image" src="https://github.com/user-attachments/assets/c550854c-00de-48fd-b23f-81f9e99acae6" />

RESULT:
Forecast accuracy is enhanced by selection of best statistical model dynamically based on ERP data and this is used to improve on time material delivery of tea to the factory.






