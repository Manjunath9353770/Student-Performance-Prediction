## 5. Important Dataset Attributes

| Attribute | Description |
|---|---|
| school | Student's school (GP or MS) |
| sex | Student's gender |
| age | Student's age |
| address | Home address type (urban or rural) |
| famsize | Family size |
| Pstatus | Parents' cohabitation status |
| Medu | Mother's education level |
| Fedu | Father's education level |
| studytime | Weekly study time |
| failures | Number of past class failures |
| schoolsup | Extra educational support |
| famsup | Family educational support |
| internet | Internet access at home |
| absences | Number of school absences |
| G1 | First-period grade |
| G2 | Second-period grade |
| G3 | Final-period grade (prediction target) |

## 6. Dataset Structure

- Total records: 395
- Total original columns: 33
- Input features used: 30
- Target column: G3
- Data type: Structured tabular data
- Problem type: Supervised learning – Regression

**Important:** G1, G2 and G3 are excluded from the model input in this project. G3 is the target variable being predicted.

## 7. Data Preprocessing

The following preprocessing operations are used:

1. Load the CSV dataset using Pandas.
2. Inspect dataset information and statistical summaries.
3. Check missing values and duplicate records.
4. Separate input features and target variable.
5. Convert categorical variables into numerical columns using one-hot encoding.
6. Split the dataset into training and testing sets.

Training set: 316 records

Testing set: 79 records

Test size: 20%

Random state: 42