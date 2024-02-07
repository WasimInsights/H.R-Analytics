# H.R Analysis-Dashboard
### Dashboard Link : https://app.powerbi.com/groups/me/reports/0005924e-56c2-4a0c-8e17-1fae260fffcd/ReportSection?experience=power-bi

## Problem Statement

Average Attrition rate for all Departments

Average Hourly rate of Male Research Scientist

Attrition rate Vs Monthly income stats

Average working years for each Department

Job Role Vs Work life balance

Attrition rate Vs Year since last promotion relation

## Tools Used for Analysis 🛠️
- Excel
- Power BI

# Unique DAX Functions Used 📊

- New custom labels were created in order to manage data lables 

Following DAX expression was written for the same,
        
        Custom Label4 = CONCATENATEX(
    VALUES(HR2[Wrk life bal cat]),
    HR2[Wrk life bal cat] & ": " & FORMAT(
        sum(HR2[WorkLifeBalance]),
        "#,.00"
    ) & "K")

See the below bar chart for better understanding.

![Screenshot 2024-02-07 162019](https://github.com/WasimInsights/Power-Bi/assets/158030674/abe26312-3938-4d29-b115-afd5d0b85a34)

- New measure created in order to manage data lables for Hourlyrate of Male Research scientists

Following DAX expression was written for the same,
        
     Kpi 2 = CALCULATE(AVERAGE(HR1[HourlyRate]),HR1[Gender] = "Male",HR1[JobRole] = "ResiSci")
See the below card visual and also a custom visual for better understanding.

![Screenshot 2024-02-07 162642](https://github.com/WasimInsights/Power-Bi/assets/158030674/5f367f69-a51f-40b3-aa8d-f8404f074eba)

visual

![Screenshot 2024-02-07 162742](https://github.com/WasimInsights/Power-Bi/assets/158030674/82de5453-c1d5-43c9-ac76-39f7767aa53d)

We’ve used a Tornado Chart to vividly display the average monthly income based on job level and gender. A fascinating dive into income disparities! 📊🌪️

![Screenshot 2024-02-07 163839](https://github.com/WasimInsights/Power-Bi/assets/158030674/5116a837-8bba-4192-90cc-754e9d8be3f6)


## Insights 🧠

1. **Attrition Rate for All Departments**
   - Varied rates across departments. Higher attrition in managerial roles in hardware and R&D. 🏢

2. **Working Years for Each Department**
   - Disparity across departments. Sales staff have longer tenure. ⏳

3. **Attrition Rate vs Monthly Income**
   - Attrition consistent despite income variation. Non-monetary factors play a crucial role. 💰

4. **Attrition Rate vs Year Since Last Promotion**
   - Inverse relationship between promotion and attrition. Timely recognition and career progression are key. 📈

5. **Hourly rate of Male Research Scientist**
   - Female scientists outearn male counterparts. Job satisfaction, commute stress, and OT pay are factors to consider. 👩‍🔬👨‍🔬

## Recommendations 📝

1. **Attrition Rate for All Departments** 🏢
   - **Recommendation**: Implement targeted retention strategies for departments with high attrition, especially for managerial roles in hardware and R&D. 🎯

2. **Working Years for Each Department** ⏳
   - **Recommendation**: Develop tailored HR strategies acknowledging the diverse tenure across departments. Initiate special retention initiatives for experienced sales staff. 📋

3. **Attrition Rate vs Monthly Income** 💰
   - **Recommendation**: Implement holistic strategies that address diverse employee needs beyond just competitive compensation. Consider factors like work-life balance, job satisfaction, and career growth opportunities. 💼

4. **Attrition Rate vs Year Since Last Promotion** 📈
   - **Recommendation**: Emphasize timely recognition and career progression to reduce attrition rates. Consider implementing a clear and transparent promotion policy. 🏅

5. **Hourly rate of Male Research Scientist** 👨‍🔬
   - **Recommendation**: Regularly check job satisfaction levels among employees. Consider introducing flexi-work or ride assists to reduce commute stress. Ensure equal pay for overtime and maintain transparency about pay scales. Deep dive into data to spot and fix pay gaps. 📊

Remember, these are just recommendations based on the Insights.

### **Datasets**
[HR_2.xlsx](https://github.com/WasimInsights/Power-Bi/files/14193031/HR_2.xlsx)
[HR_1.xlsx](https://github.com/WasimInsights/Power-Bi/files/14193029/HR_1.xlsx)

Absolutely! Feel free to dive into this data and explore your own insights. Remember, every data point has a story to tell. Happy analyzing! 📊🔍






