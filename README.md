# A GUIDE INTO LOW RISK AIRCRAFTS FOR A-Z COMPANY

# OVERVIEW

A-Z company is expanding in to new industries to diversify its portfolio.
They are interested in purchasing and operating airplanes for commercial and private enterprises.
This project aims at analysing the potential risks associated with aircrafts business.

# BUSINESS UNDERSTANDING #
The main objective (goal) of this project is to determine which aircrafts are the lowest risk for the company to venture into this new business.
The lowest risks will be determined by among other factors;the least number of accidents and the durability of the aircrafts. 
This will be guided by the engine types, the weather conditions and the countries the aircraft operates in
The findings will give insights and guide the company and its shareholders(stakeholders) on which aircrafts to buy.

# DATA UNDERSTANDING AND ANALYSYS
## Import libraries
## Loading dataset
df1 = pd.read_csv('AviationData.csv', encoding='ISO-8859-1')
df2 = pd.read_csv('USState_Codes.csv', encoding='ISO-8859-1')
Display the content of df1
print(df1)
Data visualization

# CONCLUSION
From above:
Boeing had the highest number of fatal injuries
Cessna had the highest number of accidents
The highest number of accidents were non fatal
The number of accidents were fairly constant until 1980 when it sharply increased to 3500
Highest number of accidents recorded at VMC weather conditions
# RECOMMENDATIONS

A-Z company should avoid purchasing Cessna, Boeing as indicated in the above findings
Though not common,boeing accidents are more fatal than any other aircraft accident
A-Z company may choose to use it's aircrafts in regions where less accidents are reported
A-Z company can venture into new routes not dominated by major airlines


