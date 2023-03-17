# dashboard for America Bank Dataset
data analytics projects 

AmericaBankNew.csv is the dataset to be imported
A dashboard is prepared using PowerBI 
This explains the balance amount to be paid by different groups of customers 

# Various dax functions are included

The following measures were created.

1.TOTAL BALANCE = SUM(AmericaBankNew[Balance])

2.MALE BALANCE = CALCULATE([TOTAL BALANCE],'AmericaBankNew'[Gender]="Male")

3.FEMALE BALANCE = CALCULATE([TOTAL BALANCE], 'AmericaBankNew'[Gender]="Female")

4.House owner balance = calculate([TOTAL BALANCE],'AmericaBankNew'[houseloan]="yes")

5.Renters balance = calculate([TOTAL BALANCE],'AmericaBankNew'[houseloan]="no")

6.blue collar = CALCULATE([TOTAL BALANCE],'AmericaBankNew'[Job Classification]="blue collar")

7.white collar = CALCULATE([TOTAL BALANCE],'AmericaBankNew'[Job Classification]="white collar")

# Charts Used

----Cards to show the balance amount in dashboard

----Column chart and Pie chart to show Total balance grouped by education

----Doughnut chart to show Total balance by Job Classification

----Bar Chart to show Total Balance by Marital Status

A slicer is used to filter the visualizations in dashboard with the type of education

# Interpretations from Dashboard


Total Male Balance is $128.59M

Total Female Balance is $108.34M

Total House Owner Balance is $131.81M

Total Renters Balance is $105.12M

Total White collar Balance is $116.11M

Total Blue Collar Balance is $61.26M

People under the category of secondary education are responsible for nearly 50% of the balance amount 

When analysing the marital status, Married category have more balance and divorced category tend to much less balance

When analysing the job classification, people with white collar maintain more balance than people with blue collar jobs.

From this dashboard we get a clear view on which category needs more work to receive the balance amount.

