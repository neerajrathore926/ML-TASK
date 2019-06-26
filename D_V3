import pandas as pd
import matplotlib.pyplot as plt
import numpy as np

df=pd.read_csv("http://13.234.66.67/summer19/datasets/bank.csv").head(10)
dfs=df.iloc[:,[3,7,8,12]]                                   #dataframe containing columns Balance, CreditScore,Tenure, EstimatedSalary
dfs_label=dfs.columns
df_label=df.columns
for i in range(len(dfs_label)):                             #Pie Chart
    plt.title("Bank-"+dfs_label[i])
    plt.pie(dfs.iloc[:,i],labels=df.iloc[:,1])
    plt.legend(title=df_label[1],bbox_to_anchor=(2,1))
    plt.show()
clr=["red","green","yellow","black"]
for i in range(len(dfs_label)):                               #Bar Graph
    plt.title("Bank-"+dfs_label[i])
    plt.xlabel("Emp_Names")
    plt.ylabel(dfs_label[i])
    xbar=np.arange(len(df))
    plt.bar(xbar,dfs.iloc[:,i],color=clr[i])
    plt.xticks(xbar,df.iloc[:,2],rotation=90)
    plt.grid()
    plt.show()
clr=["red","green","yellow","black"]
for i in range(len(dfs_label)):                               #Histogram
    plt.title("Bank-"+dfs_label[i])
    plt.xlabel("Emp_Names")
    plt.ylabel(dfs_label[i])
    plt.hist(dfs.iloc[:,i],color=clr[i])
    plt.grid()
    plt.show()
j=3
for i in range(len(dfs_label)):                               #Plot and Scatter
    if(i!=1):
        plt.title("Bank-"+dfs_label[i])
        plt.xlabel(dfs_label[1])
        plt.ylabel(dfs_label[i])
        plt.scatter(dfs.iloc[:,1],dfs.iloc[:,i],color=clr[i])
        plt.plot(dfs.iloc[:,1],dfs.iloc[:,i],color=clr[j])
        plt.grid()
        j=j-1
plt.show()
