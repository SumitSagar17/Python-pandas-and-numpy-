Ques. #titanic 
import pandas as pd
a=pd.read_csv(r"C:\Users\HP\Downloads\Titanic-Dataset.csv")
a.columns
c=0
d=0
for i in a.index:
    if a.loc[i,"Age"]<30:
        c=c+1
print("TOTAL PASSENGERS LESS THAN 30 YEARS:",c)
pclass=a[a["Pclass"]==1]

pclass["Fare"].sum()

pclass2=a[a["Pclass"]==2]
pclass3=a[a["Pclass"]==3] 
print("NUMBER OF SURVIVALS IN 1ST CLASS:",pclass["Survived"].sum())
print("NUMBER OF SURVIVALS IN 2ND CLASS:",pclass2["Survived"].sum())
print("NUMBER OF SURVIVALS IN 3RD CLASS:",pclass3["Survived"].sum())

Ques 
