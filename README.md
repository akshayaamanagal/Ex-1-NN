<H3>NAME: AKSHAYAA M</H3>
<H3>REGISTER NO: 212222230009</H3>
<H3>EX. NO.1</H3>
<H3>DATE</H3>
<H1 ALIGN =CENTER> Introduction to Kaggle and Data preprocessing</H1>

## AIM:

To perform Data preprocessing in a data set downloaded from Kaggle

## EQUIPMENTS REQUIRED:
Hardware – PCs
Anaconda – Python 3.7 Installation / Google Colab /Jupiter Notebook

## RELATED THEORETICAL CONCEPT:

**Kaggle :**
Kaggle, a subsidiary of Google LLC, is an online community of data scientists and machine learning practitioners. Kaggle allows users to find and publish data sets, explore and build models in a web-based data-science environment, work with other data scientists and machine learning engineers, and enter competitions to solve data science challenges.

**Data Preprocessing:**

Pre-processing refers to the transformations applied to our data before feeding it to the algorithm. Data Preprocessing is a technique that is used to convert the raw data into a clean data set. In other words, whenever the data is gathered from different sources it is collected in raw format which is not feasible for the analysis.
Data Preprocessing is the process of making data suitable for use while training a machine learning model. The dataset initially provided for training might not be in a ready-to-use state, for e.g. it might not be formatted properly, or may contain missing or null values.Solving all these problems using various methods is called Data Preprocessing, using a properly processed dataset while training will not only make life easier for you but also increase the efficiency and accuracy of your model.

**Need of Data Preprocessing :**

For achieving better results from the applied model in Machine Learning projects the format of the data has to be in a proper manner. Some specified Machine Learning model needs information in a specified format, for example, Random Forest algorithm does not support null values, therefore to execute random forest algorithm null values have to be managed from the original raw data set.
Another aspect is that the data set should be formatted in such a way that more than one Machine Learning and Deep Learning algorithm are executed in one data set, and best out of them is chosen.


## ALGORITHM:
STEP 1:Importing the libraries<BR>
STEP 2:Importing the dataset<BR>
STEP 3:Taking care of missing data<BR>
STEP 4:Encoding categorical data<BR>
STEP 5:Normalizing the data<BR>
STEP 6:Splitting the data into test and train<BR>

##  PROGRAM:
```python
#import libraries
from google.colab import files
import pandas as pd
import io
from sklearn.preprocessing import StandardScaler
from sklearn.preprocessing import MinMaxScaler
from sklearn.model_selection import train_test_split

#Read the dataset from drive
df=pd.read_csv("/content/Churn_Modelling.csv")
df

#split the dataset
X=df1.iloc[:,:-1].values
print(X)
y=df1.iloc[:,-1].values
print(y)

#Finding Missing values
print(df.isnull().sum())

#Check for Duplicates
df.duplicated()

print(df['Exited'].describe())
df.info()

df=df.drop(['Surname','Geography','Gender'],axis=1)
df

scaler=MinMaxScaler()
df1=pd.DataFrame(scaler.fit_transform(df))
print(df1)

X_train,X_test,y_train,y_test=train_test_split(X,y,test_size=0.2)
print(X_train)
print(len(X_train))
print(X_test)
print(len(X_test))
```
## OUTPUT:
### Read the datase
![image](1.png)
### Split the dataset
![image](2.png)
### Finding Missing values
![image](3.png)
### Checking Duplicates
![image](4.png)
### Describe a column
![image](5.png)
### Info
![image](6.png)
### Dropping columns
![image](7.png)
### Normalizing the data
![image](8.png)
### X_train
![Screenshot 2024-08-23 093907](https://github.com/user-attachments/assets/536de344-6a5f-45f9-88cc-bb13ecab057c)

### X_test
![Screenshot 2024-08-23 093913](https://github.com/user-attachments/assets/9cc63c61-beb5-4616-a8c7-3221f588175a)

## RESULT:
Thus, Implementation of Data Preprocessing is done in python  using a data set downloaded from Kaggle.


