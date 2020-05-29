(thanks to Tolgahan Türkoğlu for support)

                       Visual Programming Course Project 
The project summary: 
Corona Outbreak Data Visualization
Software Design:
The software receives daily data on the coronavirus pandemic (COVID-19) provided by the European Center for Disease Prevention and Control (ECDC). EU Open Data Portal COVID-19 Coronavirus data set updated daily (https://opendata.ecdc.europa.eu/covid19/casedistribution/xml/) uses.
Getting Information from the User
**The URL of the user's XML file https://opendata.ecdc.europa.eu/covid19/casedistribution/xml/ main window that can enter properly**
Adding interactions (tag, text field and buttons) to interact with the user to get the URL of the data set as shown in Figure 1.
 ![j1](https://user-images.githubusercontent.com/45681252/83247457-3c84bb80-a1ac-11ea-916b-146e048e064c.PNG)

Figure 1 Getting the dataset URL from the user
Extracting Data from the EU Open Data Portal
The European Center for Disease Prevention and Control (ECDC) provides daily data on the coronavirus pandemic (COVID-19) through the EU Open Data Portal. Downloadable data files are updated daily and contain the latest public data in COVID-19. As you can see in the example below, the data is provided in XML format:
XML: https://opendata.ecdc.europa.eu/covid19/casedistribution/xml/ 
 
<record>  
          <dateRep>07/05/2020</dateRep>  
          <day>7</day>  
          <month>5</month>  
          <year>2020</year> 
          <cases>2253</cases>  
          <deaths>64</deaths> 
          <countriesAndTerritories>Turkey</countriesAndTerritories>  
         <geoId>TR</geoId>  
         <countryterritoryCode>TUR</countryterritoryCode> 
         <popData2018>82319724</popData2018>  
         <continentExp>Asia</continentExp> 
</record>

Select its XML, surrounded by two tags <record> and </record>, apply a specific date date, daily COVID-19 case, and includes their deaths and information within this country. The application parses the XML document provided to extract all records and then keep them in a correct Collection application.
Visualization of Data
After extracting the data from the specified XML file, the program visualizes the data using tables and graphics. The program includes the following tables and graphics.
Cases and deaths reported by country table:
![j2](https://user-images.githubusercontent.com/45681252/83247494-48707d80-a1ac-11ea-8a43-821df64f4f6e.PNG)

 
includes linechart and barchart tables such as:


![j4](https://user-images.githubusercontent.com/45681252/83247387-21b24700-a1ac-11ea-8e8f-7044da46b9de.PNG)

![j3](https://user-images.githubusercontent.com/45681252/83247409-2a0a8200-a1ac-11ea-8fdd-f1e03759a72f.PNG)

