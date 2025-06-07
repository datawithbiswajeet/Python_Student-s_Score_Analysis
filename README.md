# 📊 Student Score Analysis In Python

Welcome to the **Student Score Analysis** project!  
This project demonstrates a complete **data science workflow** — from data cleaning and preprocessing to generating **insightful visualizations** using Python. The goal is to uncover patterns and draw meaningful conclusions from student performance data.

---
## 🛠️ Tools & Libraries Used

- **Python 3.x**
- **Pandas** – for data manipulation
- **Matplotlib** & **Seaborn** – for data visualization
- **Google Colab**
- **Git & GitHub** – for version control and sharing

## Dataset Used
 <a href="https://github.com/datawithbiswajeet/Python_Student-s_Score_Analysis/blob/main/dataset%20student_scores.csv"> Student Score Analysis </a>

 ## Project Pyhton File 
  <a href="https://github.com/datawithbiswajeet/Python_Student-s_Score_Analysis/blob/main/student_score.ipynb"> Python All Code Details of Data Cleaning, Preprocessing & Visualizations </a>

## 🧹 Data Cleaning & Preprocessing

- Loaded `.csv` dataset using pandas
- Using pandas, we cleaned the dataset by: Dropping unnecessary columns (Unnamed: 0)
- Replacing or removing missing values (fillna, dropna, median)
- Standardizing categorical entries (e.g., replacing "05Oct" with "5-10" in WklyStudyHours)
  --- This step ensured that the dataset was consistent and readyfor analysis

## 1. Importing Required Libraries
 import pandas as pd
## 2. Load the dataset
 df = pd.read_csv("student_scores.csv")
## 3. Drop unnecessary index column
 df.drop(columns=["Unnamed: 0"], inplace=True)
## 4. Replace incorrect value in WklyStudyHours column
 df["WklyStudyHours"] = df["WklyStudyHours"].replace("05-Oct", "5-10")
## 5. Check for missing values
 df.isnull().sum()
## 6. Fill missing categorical values
 df["EthnicGroup"].fillna("unknown", inplace=True)
## 7. Fill missing numerical values with median
 df["NrSiblings"] = df["NrSiblings"].fillna(df["NrSiblings"].median())
## 8. Drop any remaining rows with missing values (optional/if needed)
 df.dropna(inplace=True)
 

## EXPLORATORY DATA ANALYSIS
      Using pandas, matplotlib, and seaborn, I explored relationships and patterns in the data. 
      
## Key insights included:

### 1. Distribution of diffrent scores with number of student
### 2. Distribution by Ethnic group
### 3. Reading score by parents education
### 4. Maths Score By Gender 
### 5. Maths Score By Study Hour

## Visualizations 📈📈📈📈📈
-- 
![9](https://github.com/user-attachments/assets/ce5f7534-95a4-40a2-81a1-439a11550073)
![16](https://github.com/user-attachments/assets/6b0a4a35-7b06-4965-b5d4-0d51374c703b)
![15](https://github.com/user-attachments/assets/08264f59-4acd-4b46-a1eb-3cb7c488492d)
![14](https://github.com/user-attachments/assets/33587c49-9040-41ca-87ea-d914ccbe1f9c)
![13](https://github.com/user-attachments/assets/eba5918b-268a-4345-a836-93425af9b4df)
![12](https://github.com/user-attachments/assets/78c0832d-ec1f-4e5f-9c1f-be09ffea6321)
![11](https://github.com/user-attachments/assets/c6b475c7-594a-4c27-b236-18b298969556)
![10](https://github.com/user-attachments/assets/ce8f2117-3ff0-4885-b635-61ed2c813cc2)

## 📌 Key Insights

### 1. Students who completed test preparation scored significantly higher.
### 2. Writing, reading, and math scores are strongly correlated.
### 3. Parental level of education has a positive impact on student scores.
### 4. Gender and race group show score variations worth exploring further.

## ✅ Final Summary
   This project showcases a complete journey of data analysis using Python — from raw data to valuable insights. Through effective data cleaning and visual storytelling, we explored how factors like gender, parental education, and test preparation influence student performance.
   By leveraging tools like Pandas, Matplotlib, and Seaborn, we transformed a basic dataset into a clear, data-driven narrative. This analysis not only enhances our understanding of student success metrics but also builds a strong foundation in real-world data science practices.

# 🔗 Connect with Me
    Let’s connect and collaborate!

### 📧 Email: datawithbiswajeet@email.com

### 💼 LinkedIn: (https://www.linkedin.com/in/datawithbiswajeet/)












 





