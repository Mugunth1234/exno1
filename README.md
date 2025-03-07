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
```
import pandas as pd
df=pd.read_csv("SAMPLEIDS.csv")
df
```
![Screenshot 2025-03-07 160821](https://github.com/user-attachments/assets/46a02c8a-73ce-465d-9fca-9d3735c6b12e)
```
df.isnull().sum()
```
![Screenshot 2025-03-07 161046](https://github.com/user-attachments/assets/5c9395e5-9981-4413-bc18-f6ac0a6846dc)
```
df.isnull().any()
```
![Screenshot 2025-03-07 161200](https://github.com/user-attachments/assets/7e91ea45-2efa-4d0f-a29d-b4806f2f91ee)
```
df.dropna()
```
![Screenshot 2025-03-07 161331](https://github.com/user-attachments/assets/6403ba30-885d-4c07-a8be-e426a7be5833)
```
df.fillna(0)
```
![Screenshot 2025-03-07 161509](https://github.com/user-attachments/assets/9cc299cd-d1df-40c8-a395-46654cc52196)
```
df.fillna(method = 'ffill')
```
![Screenshot 2025-03-07 161652](https://github.com/user-attachments/assets/5cc055b7-5e6a-4d0c-9201-e45faf1587f2)
```
df.fillna(method = 'bfill')
```
![Screenshot 2025-03-07 161843](https://github.com/user-attachments/assets/59fb0212-c661-497d-9e84-8ea34c54e365)
```
df_dropped = df.dropna()
df_dropped
```
![image](https://github.com/user-attachments/assets/64cf2bbf-9b1b-4a11-828f-5da156c7b023)
```
df.fillna({'GENDER':'MALE','NAME':'SRI','ADDRESS':'POONAMALEE','M1':98,'M2':87,'M3':76,'M4':92,'TOTAL':305,'AVG':89.999999})
```
![image](https://github.com/user-attachments/assets/cc0db8df-6fc5-49ec-b384-92b1ae094f24)

              IQR(Inter Quartile Range
```
import pandas as pd
ir=pd.read_csv('iris.csv')
ir
```
![Screenshot 2025-03-07 162640](https://github.com/user-attachments/assets/92584654-db08-44bd-96cb-baf9f38d1ee0)
```
ir.describe()
```
![Screenshot 2025-03-07 162801](https://github.com/user-attachments/assets/29f8482a-1590-428a-861c-939af65281eb)
```








         
# Result
          <<include your Result here>>
