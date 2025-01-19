# task2
 TASK - 02  Perform data cleaning and exploratory data analysis (EDA)  on a dataset of your choice, such as the Titanic dataset from Kaggle. Explore the relationships between variables and identify patterns and trends in the data
 import pandas as pd
df=pd.read_csv('gender_submission.csv'
df=pd.read_csv('gender_submission.csv')
print(df.head())
print(df.columns)
print(df.isnull().sum())
print(df['Survived'].value_counts())
import matplotlib.pyplot as plt
import seaborn as sns
sns.countplot(x='Survived', data=df)
plt.title('Distribution of Survival Predictions')
plt.show()
sns.lineplot(x='PassengerId', y='Survived', data=df)
plt.title('Survival Prediction Across Passengers')
plt.show()
