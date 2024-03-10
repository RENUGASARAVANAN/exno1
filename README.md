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

# CODE
## DATA CLEANING PROCESS

import pandas as pd
df=pd.read_csv("/content/Data_set.csv")

df.head(5)

df.tail(3)

df.info()

df.describe()

df.isnull()

df.notnull()

df.dropna(axis=1)

dfs=df[df['rating']>3]
dfs

df.iloc[[1,3,5],[1,3]]

df=df.fillna(0)
df

# OUTPUT

![Screenshot 2024-03-10 093215](https://github.com/RENUGASARAVANAN/exno1/assets/119292258/8e715481-595b-4e10-8540-ec5836cb243f)

![Screenshot 2024-03-10 093230](https://github.com/RENUGASARAVANAN/exno1/assets/119292258/a41990cd-8d00-4ef9-b2ae-98bc3a45749e)

![Screenshot 2024-03-10 093245](https://github.com/RENUGASARAVANAN/exno1/assets/119292258/987f028a-548a-4cda-9cfb-0420bacfe047)

![Screenshot 2024-03-10 093306](https://github.com/RENUGASARAVANAN/exno1/assets/119292258/d0f8f1aa-53e1-434b-9c7f-b92bd1558318)

![Screenshot 2024-03-10 093338](https://github.com/RENUGASARAVANAN/exno1/assets/119292258/d99e3f0c-dc12-4cbe-a306-a771eaa74c13)

![Screenshot 2024-03-10 093351](https://github.com/RENUGASARAVANAN/exno1/assets/119292258/e64c05a4-3e26-4ce9-bbb9-f964f8ead676)

![Screenshot 2024-03-10 093414](https://github.com/RENUGASARAVANAN/exno1/assets/119292258/86c075ff-d528-487b-8193-9217a262fcaa)

![Screenshot 2024-03-10 093452](https://github.com/RENUGASARAVANAN/exno1/assets/119292258/cf436a07-1215-47d8-a2bb-e42145949276)

![Screenshot 2024-03-10 093619](https://github.com/RENUGASARAVANAN/exno1/assets/119292258/8d3a6060-413d-4d21-87d6-8e4533b4447b)

![Screenshot 2024-03-10 093755](https://github.com/RENUGASARAVANAN/exno1/assets/119292258/7f8a2595-147a-4af9-9745-56529f2dee6b)


# Result
 Thus the given data is read,cleansed and the cleaned data is saved into the file.
