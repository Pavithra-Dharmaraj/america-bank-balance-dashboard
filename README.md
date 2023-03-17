# dashboard for America Bank Dataset
data analytics projects 

AmericaBankNew.csv is the dataset to be imported
A dashboard is prepared using PowerBI 
This explains the balance amount to be paid by different groups of customers 

Various dax functions are included
The following measures were created.
1.TOTAL BALANCE = SUM(AmericaBankNew[Balance])
2.MALE BALANCE = CALCULATE([TOTAL BALANCE],'AmericaBankNew'[Gender]="Male")
3.FEMALE BALANCE = CALCULATE([TOTAL BALANCE], 'AmericaBankNew'[Gender]="Female")
4.House owner balance = calculate([TOTAL BALANCE],'AmericaBankNew'[houseloan]="yes")
5.Renters balance = calculate([TOTAL BALANCE],'AmericaBankNew'[houseloan]="no")
6.blue collar = CALCULATE([TOTAL BALANCE],'AmericaBankNew'[Job Classification]="blue collar")
7.white collar = CALCULATE([TOTAL BALANCE],'AmericaBankNew'[Job Classification]="white collar")
