# Topic: Thailand Export Trends (Jan2020 - Jul2022)
# Creator:
ID: 6420412008<br/>
NAME: Sirirat Lueprasert<br/>
Subject: DADS5001 (Tools)
# Dataset Details:
Source: https://www.customs.go.th/statistic_report.php?<br/>
Main Data information: All export data since Jan2020 to Jul2021 from Thai Customs Website<br/>
Main Data filename: '2020_202207_All_Country_by_statistic_code.rar' > Due to the file is larger than 25 MB, so I compressed the file.<br/>
Main Data have 325632 rows × 12 columns (getting from combining each monthly file together as the website allow downloading the data 1 month/time/file > coding using selenium library to help pulling the data from website then combining all files together)<br/> 
Support data information:<br/>
Filename:HS_Code_First_2_digits (97 rows × 4 columns), Unit_RMTS_Customs (22 rows × 2 columns)<br/> 
# Questions: <br/> 
1.Which product type that Thailand exported the most?<br/> 
2.Which product that Thailand exported the most?<br/> 
3.Which country that Thailand exported the top exported good to?
# Challenges:
- The source website can pull data only 1 month/time/file
- Understanding the dataset > mainly about HS Code (categorized code)
- Searching for the data of grouping HS Code
- Large data to work with including in detail of HS Code
- HS Code data need to be adjusted to work with
- Adjust date data format in dataset
- Data need to be cleaned (e.g. data with space, setting data type to work with)
- Choosing the chart type to represent obtained data
- Creating the desired chart
- How to put the appropriate information into 1 slide of presentation
# Information to understand the dataset:
File name:
- พระราชกําหนด พิกัดอัตราศุลกากร (ฉบับที่ 6) พ.ศ.2559
- Unit_RMTS_Customs
- Text of AHTN 2017 with Corrigendum (พิกัดฉบับภาษาอังกฤษเพื่อการอ้างอิง)<br/>
Website explain about incoterm (In case you would  like to know more about the terminology of import/export in TH) : https://www.customs.go.th/content.php?ini_content=customs_valuation_03&ini_menu=menu_customs_value&lang=th&left_menu=menu_customs_value_03<br/>

FOB Meaning: https://www.freightquote.com/blog/what-does-fob-mean-in-freight-shipping/<br/>
FOB stands for “free on board” or “freight on board” and is a designation that is used to indicate when liability and ownership of goods is transferred from a seller to a buyer.

Free on Board:
Free on board indicates whether the seller or the buyer is liable for goods that are damaged or destroyed during shipping. When used with an identified physical location, the designation determines which party has responsibility for the payment of the freight charges and at what point title for the shipment passes from the seller to the buyer.

In international shipping, for example, “FOB [name of originating port]” means that the seller (consignor) is responsible for transportation of the goods to the port of shipment and the cost of loading. The buyer (consignee) pays the costs of ocean freight, insurance, unloading, and transportation from the arrival port to the final destination. The seller passes the risk to the buyer when the goods are loaded at the originating port.<br/>

To sum up FOB is the cost of the goods + others (transportation+insurance+etc.) until the goods is loaded on board for exporter's (Seller) responsibility.<br/>

HS Code Meaning: https://www.trade.gov/harmonized-system-hs-codes<br/>
Harmonized System (HS) Codes is a standard commodity classification.<br/>
Grouping HS Code into 21 Sections:<br/>
For more info.:https://www.cybex.in/hs-codes/machinery-mechanical-appliances-electrical-equipment-section-16.aspx
# Charts
- Figure1: Trends of all goods categorized by 21 sections<br/>
The top exported section is section 16 (Machinery and Mechanical Appliances; Electrical Equipment; Parts thereof; sound Recorders and Reproducers, Television Image and Sound Recorders and reproducers, Television Image and sound Recorders and Reproducers, and Parts and Accessories of such article)<br/>
![image](https://user-images.githubusercontent.com/111365836/195888256-a9fd2b01-3aca-4153-a6c2-f0a4ead6537c.png)<br/>
- Figure2: Trends of sections 16 (Machinery and Mechanical Appliances; Electrical Equipment; Parts thereof; etc.) By HS Chapter>Heading<br/>
To go further in section 16 into the first 4 digit of HS Code (By Chapter>Heading), the result shows that 8471 (Automatic data processing machines and units thereof; magnetic or optical readers, machines for transcribing data onto data media in coded form and machines for processing such data, not elsewhere specified or included.) is the top export.<br/>
![image](https://user-images.githubusercontent.com/111365836/195888456-c0f7687a-d17c-4628-bb3a-ec887c28b973.png)<br/>
- Figure3: Trends of 8471 (the top export from figure2)<br/>
Exploring further in 8471, the result shows that 847170 (Storage units) is the top export which data from dataset shows that the HDD is the top export goods in 847170.<br/>
![image](https://user-images.githubusercontent.com/111365836/195888916-495e6779-c84b-40ec-84f0-016784f04fec.png)<br/>
- Figure4: Export Percentage of 847170 comparing to others:<br/>
The figure is to get you more understanding view in export percentage of 8471 showing percentage of 847170 comparing with others.<br/>
![image](https://user-images.githubusercontent.com/111365836/195889241-8175a852-db5b-4cc9-924c-46450bb85e8d.png)<br/>
- Figure5: 847170 > top export by country:<br/>
After get information that the electronic storage unit is the top exported goods, so looking deeper to know which country that Thailand export to the most. The results shows that it is United Arab Emirates(AE).<br/>
![image](https://user-images.githubusercontent.com/111365836/195889583-716f1275-0d3f-4a51-8712-f3eaea68b881.png)<br/>
# Summary
- Section 16 (Machinery and Mechanical Appliances; Electrical Equipment; Parts thereof; etc.) is the most exported section.
- The top exported good in section 16 is 847170 which is an electronic storage units (mainly exported goods is HDD (Hard Disk Drive).
- The country which Thailand export an electronic storage units (847170) the most is UNITED ARAB EMIRATES (AE) > Y2020:99.94%, Y2021:99.90%, Y2022:99.88%.
From the obtained information in dataset since 2020, it presents that 30.15% of all Thailand export goods (main export) is the electronical equipments/parts. And the main exported product is HDD which Thailand exported most of it to United Arab Emirates. This information shows that Thailand should pay attention to develop in this industry by maintaining/keep improving the quality of the product, or support Thailand businesses including valuable workforces. The information also shows that Thailand is at risk by depending on just 1 country (mostly) to export the HDD, so Thailand should actively find the new market to minimize the risk in case the main exported country stop buying the goods. Lastly, this information might help for the decision making of the logistic businesses as well to help they decide which industry that they should pay attention to gain the reliable customer.<br/>
# Presentation:
![image](https://user-images.githubusercontent.com/111365836/195891370-31ca8e20-c99e-456c-b56c-11cc544c0d54.png)

