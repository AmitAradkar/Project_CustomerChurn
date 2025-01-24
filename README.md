# Customer Churn Analysis

This project aims to analyze customer churn data for the telecom company "Neo" to understand and reduce customer attrition. By applying data manipulation, visualization, and machine learning techniques, insights are extracted to help the company retain customers.

## Problem Statement

The company faces challenges with customers switching to competitors. As a data scientist, your task is to analyze customer data, identify trends, and develop predictive models to mitigate churn.

## Dataset

The project uses the `customer_churn` dataset, which contains customer demographics, payment methods, contract types, and churn status. Details of the dataset are provided in the accompanying data dictionary.

## Environment

- Python (Anaconda)
- Jupyter Notebook

## Tasks Performed

### 1. Data Manipulation
- Extract the 5th column into `customer_5`.
 ![image](https://github.com/user-attachments/assets/a967afa6-f69b-475e-8834-ebab5cb909c2)

- Extract the 15th column into `customer_15`.
 ![image](https://github.com/user-attachments/assets/6d13cd55-ed92-4cd0-b9ce-4fbf19779a16)

- Filter male senior citizens using electronic check as the payment method and store in `senior_male_electronic`.
  ![image](https://github.com/user-attachments/assets/69bd9293-a3ec-46a5-8d76-0c15651ab666)

- Retrieve customers with tenure > 70 months or monthly charges > $100 into `customer_total_tenure`.
  ![image](https://github.com/user-attachments/assets/de240724-ab7d-4ebf-990f-2e0dca695c8e)

- Extract customers with two-year contracts, payment via mailed check, and churn status as "Yes" into `two_mail_yes`.
  ![image](https://github.com/user-attachments/assets/9a4ce9b6-daf9-42fc-83c0-e334d607bf93)

- Randomly select 333 records into `customer_333`.
  ![image](https://github.com/user-attachments/assets/61ece6bd-6e30-4d03-89db-45062a5e6c78)

- Count the unique levels in the `Churn` column.
  ![image](https://github.com/user-attachments/assets/eb3d9b72-f8b1-46c0-9563-74d6686c95f3)


### 2. Data Visualization
- **Bar Plot**:
  - Column: `InternetService`
  - X-axis: Categories of Internet Service
  - Y-axis: Count of Categories
  - Bar color: Orange
  - Title: Distribution of Internet Service
    ![image](https://github.com/user-attachments/assets/4a600147-d2c7-4472-9be0-50bf6ff5c039)

- **Histogram**:
  - Column: `tenure`
  - Bins: 30
  - Color: Green
  - Title: Distribution of Tenure
    ![image](https://github.com/user-attachments/assets/c39bb94b-2da8-427d-bdd5-66635ecd19ce)

- **Scatter Plot**:
  - X-axis: `tenure`
  - Y-axis: `MonthlyCharges`
  - Point color: Brown
  - Title: Tenure vs Monthly Charges
    ![image](https://github.com/user-attachments/assets/fba1922d-1a60-41c0-b3d0-a6880df4790c)

- **Box Plot**:
  - X-axis: `Contract`
  - Y-axis: `tenure`
    ![image](https://github.com/user-attachments/assets/2fcf9808-2ba1-4ee8-86dc-5f9274a505d2)


### 4. Logistic Regression
- **Simple Logistic Regression**:
  - Dependent Variable: `Churn`
  - Independent Variable: `MonthlyCharges`
  - Split: 65:35
  - Evaluate using confusion matrix and accuracy score.
    ![image](https://github.com/user-attachments/assets/5ff76b37-be7a-4086-9737-85cb996b7aca)

- **Multiple Logistic Regression**:
  - Dependent Variable: `Churn`
  - Independent Variables: `tenure`, `MonthlyCharges`
  - Split: 80:20
  - Evaluate using confusion matrix and accuracy score
    ![image](https://github.com/user-attachments/assets/163f7297-cb74-4658-999c-2157106298b4)


### 5. Decision Tree
- Dependent Variable: `Churn`
- Independent Variable: `tenure`
- Split: 80:20
- Evaluate using confusion matrix and accuracy score.
  ![image](https://github.com/user-attachments/assets/3655b640-743d-48b0-a114-58112b97a3da)
  ![image](https://github.com/user-attachments/assets/a143cca3-f80a-4240-bd3a-2ada19d4426b)


### 6. Random Forest
- Dependent Variable: `Churn`
- Independent Variables: `tenure`, `MonthlyCharges`
- Split: 70:30
- Evaluate using confusion matrix and accuracy score.
  ![image](https://github.com/user-attachments/assets/d27c885e-cc3d-43f6-9863-97448828b4ad)
  ![image](https://github.com/user-attachments/assets/45231d78-6765-4bba-855f-7335aa0e5373)


## Conclusion

This project demonstrates effective use of Python for data manipulation, visualization, and machine learning to address customer churn. The insights and models developed provide actionable strategies for retaining customers and improving business outcomes.

---
