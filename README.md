# EXNO-6-DS-DATA VISUALIZATION USING SEABORN LIBRARY

# Aim:
  To Perform Data Visualization using seaborn python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```
import seaborn as sns
```
```
df=sns.load_dataset("iris")
```
```

df.head()
```
<img width="630" height="198" alt="Screenshot 2026-03-10 103958" src="https://github.com/user-attachments/assets/749111a9-5d44-4515-a872-e19cf997aded" />

```
df.corr(numeric_only=True)
```
<img width="601" height="195" alt="Screenshot 2026-03-10 104010" src="https://github.com/user-attachments/assets/abe9e7dd-1adc-4939-96c0-61c763cba941" />

```
sns.heatmap(df.corr(numeric_only=True))
```
<img width="701" height="587" alt="Screenshot 2026-03-10 104020" src="https://github.com/user-attachments/assets/47a2f641-23b8-4b71-b95f-98e586ea8545" />

```
sns.jointplot(x='petal_length',y='petal_width',data=df,kind='hex')
```
<img width="766" height="811" alt="Screenshot 2026-03-10 104028" src="https://github.com/user-attachments/assets/6babbd31-1019-4745-9ba5-652a97fedd6a" />

```
sns.jointplot(x='petal_length',y='petal_width',data=df,kind='reg')
```
<img width="787" height="802" alt="Screenshot 2026-03-10 104036" src="https://github.com/user-attachments/assets/8f201881-9f31-4a34-a4c7-8132aced4ff1" />

```
sns.pairplot(df)
```
<img width="986" height="986" alt="output" src="https://github.com/user-attachments/assets/80677d95-d44c-4015-9c67-5826c7fe216e" />

```
sns.pairplot(df,hue='sepal_length')
```
<img width="1084" height="946" alt="Screenshot 2026-03-10 104138" src="https://github.com/user-attachments/assets/f0cb3fb4-be0e-4457-8f07-af0856e6b504" />

```
sns.distplot(df['petal_length'])
```
<img width="804" height="863" alt="Screenshot 2026-03-10 104148" src="https://github.com/user-attachments/assets/af3b7d58-bf66-447e-b2f5-26f8ece6967c" />

```
sns.distplot(df['petal_length'],kde=False,bins=10)
```
<img width="737" height="890" alt="Screenshot 2026-03-10 104156" src="https://github.com/user-attachments/assets/35116895-bd57-4915-b978-a887ceee1d73" />

```
sns.countplot(x='petal_length',data=df)
```
<img width="744" height="610" alt="Screenshot 2026-03-10 104205" src="https://github.com/user-attachments/assets/0a121891-5909-4110-99c7-9d2a4922773a" />

```
sns.countplot(x='species',data=df)
```
<img width="739" height="652" alt="Screenshot 2026-03-10 104210" src="https://github.com/user-attachments/assets/aa95a4b4-9589-46d9-878e-7522662900cd" />

```
sns.countplot(y='species',data=df)
```
<img width="823" height="628" alt="Screenshot 2026-03-10 104216" src="https://github.com/user-attachments/assets/c28f6700-ead5-4252-85e2-78829531c119" />

```
sns.barplot(x='petal_length',y='petal_width',data=df)
```
<img width="777" height="617" alt="Screenshot 2026-03-10 104221" src="https://github.com/user-attachments/assets/74e325f2-b189-42fd-a4c6-74eff21d75e9" />

```
sns.barplot(x='petal_width',y='petal_length',data=df)
```
<img width="746" height="622" alt="Screenshot 2026-03-10 104228" src="https://github.com/user-attachments/assets/8afbd39b-bbbf-49a6-96b5-92bc1585fe51" />

```
df.head()
```
<img width="731" height="267" alt="Screenshot 2026-03-10 104235" src="https://github.com/user-attachments/assets/5fd285a3-eaa5-40ee-b42d-b9c67cc9bd8c" />

```
sns.boxplot(x='species',y='sepal_length', data=df)
```
<img width="820" height="641" alt="Screenshot 2026-03-10 104241" src="https://github.com/user-attachments/assets/9cdf1971-8051-4a6d-bad7-016a65d71ab0" />

```
sns.boxplot(x="species", y="sepal_length", data=df,palette='rainbow')
```
<img width="1168" height="762" alt="Screenshot 2026-03-10 104259" src="https://github.com/user-attachments/assets/b6d2cb9d-f0b9-41a2-a91f-7f388caa7c07" />

```
sns.boxplot(data=df,orient='v')
```
<img width="723" height="585" alt="Screenshot 2026-03-10 104305" src="https://github.com/user-attachments/assets/18d0bbd3-7b84-4479-892d-5bed48a52198" />

```
sns.boxplot(x="sepal_length", y="species", hue="species",data=df)
```
<img width="839" height="635" alt="Screenshot 2026-03-10 104312" src="https://github.com/user-attachments/assets/7685f830-7d9b-4508-afd0-4b975a03512a" />

```
sns.violinplot(x="sepal_length", y="species", data=df,palette='rainbow')
```
<img width="1632" height="791" alt="Screenshot 2026-03-10 104324" src="https://github.com/user-attachments/assets/e48a613d-1c78-48e4-8125-6679e54c7d5b" />

# Result:

 Thus Data Visualisation using seaborn library has been done and verified.
