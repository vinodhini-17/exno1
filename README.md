# Exno:1
Data Cleaning Process

# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# Algorithm
STEP 1: Read the given Data

STEP 2: Get the information about the data

STEP 3: Remove the null values from the data

STEP 4: Save the Clean data to the file

STEP 5: Remove outliers using IQR

STEP 6: Use zscore of to remove outliers

# Coding and Output
import pandas as pd
df=pd.read_csv('/content/SAMPLEDS.csv')
print(df)     
![image](https://github.com/vinodhini-17/exno1/assets/145742741/fc3169cd-c318-4b2b-a31e-854e53fc2643)
print(df.info())
![image](https://github.com/vinodhini-17/exno1/assets/145742741/3f4500b2-69c6-48e4-96cf-798b29c90922)
df.describe()
![image](https://github.com/vinodhini-17/exno1/assets/145742741/9ae9faff-23da-4a71-953f-dee77c9a016d)
print(df.head())
![image](https://github.com/vinodhini-17/exno1/assets/145742741/e9e92aea-055d-482c-adc3-cf54998f9738)
print(df.tail())
![image](https://github.com/vinodhini-17/exno1/assets/145742741/31bfb578-1e48-4353-bf59-a10280c6d030)
x=df.dropna(how='any')
print(x)
![image](https://github.com/vinodhini-17/exno1/assets/145742741/b53447eb-e839-4ee5-bf61-91fa4001522a)
tot=df.dropna(subset=['TOTAL'],how='any')
print(tot)

![image](https://github.com/vinodhini-17/exno1/assets/145742741/2f9e3890-69df-470a-8123-817fb8ba405f)
print(df.fillna(0))

![image](https://github.com/vinodhini-17/exno1/assets/145742741/ba828a0c-6530-4e2b-9cc3-a214fef93da7)
df.TOTAL.fillna(mn,inplace=True)
print(df)
![image](https://github.com/vinodhini-17/exno1/assets/145742741/782a2409-865b-488a-8b95-d653f9ca0209)

import pandas as pd
import seaborn as sns
age=[1,3,28,27,25,92,30,39,40,50,26,24,29,94]
af=pd.DataFrame(age)
print(af)

![image](https://github.com/vinodhini-17/exno1/assets/145742741/187ac048-bd12-4dbf-b1ca-38c0126a0195)

sns.boxplot(data=af)

![image](https://github.com/vinodhini-17/exno1/assets/145742741/503018cb-5c20-425a-b2a0-2c61c52bbd52)


![image](https://github.com/vinodhini-17/exno1/assets/145742741/0e1a1c21-1481-414c-b00e-584f92ed9925)

![image](https://github.com/vinodhini-17/exno1/assets/145742741/5b3b56d2-9357-47f7-93f3-ec0a7bd38cb4)

![image](https://github.com/vinodhini-17/exno1/assets/145742741/eca352c3-e1a9-48d1-b36d-9539f19be5c7)

![image](https://github.com/vinodhini-17/exno1/assets/145742741/760f07d7-eedd-43ae-b019-0e2e817039cf)


![image](https://github.com/vinodhini-17/exno1/assets/145742741/fe393ccf-386f-44ef-af21-24f467e72c1b)




import pandas as pd
import numpy as np
import pandas as pd
from scipy import stats
data={'weight':[12,15,18,21,24,27,30,33,36,39,42,45,51,54,57,60,63,66,69,202,72,75,78,81,84,232,87,90,93,96,99,258]}
df=pd.DataFrame(data)
print(df)

![image](https://github.com/vinodhini-17/exno1/assets/145742741/608b34dc-2d9e-49c9-a5b1-52a54e69fec9)

# Result
Thus To read the given data and perform data cleaning and save the cleaned data to a file done successfully.
