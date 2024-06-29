# 🙋Customer Dispute Prediction

## Introduction
This project aims to predict whether a customer will dispute an issue with the bank based on given data. By leveraging various machine learning models and performing thorough data analysis, we aim to provide actionable insights to the business team for better customer service management.

## Objectives
- Predict whether a customer will dispute an issue with the bank.
- Utilize Python libraries for data operations, visualization, and model building.
- Use the best-performing model to predict outcomes for the test dataset and save the results.

## Dataset Description
The dataset includes information on customer complaints and disputes with the bank. Key features include:
- **Date received**: The day the complaint was received.
- **Product**: Different products offered by the bank (e.g., credit cards, debit cards).
- **Sub-product**: Specific options like loans and insurance.
- **Issue**: Description of the customer's complaint.
- **Company public response**: Company's response to the complaint.
- **Company**: Name of the company.
- **State**: State where the customer resides.
- **ZIP code**: Customer's ZIP code.
- **Submitted via**: Platform used to register the complaint (e.g., online, phone).
- **Date sent to company**: Date the complaint was sent to the company.
- **Timely response?**: Whether the company responded in a timely manner (yes/no).
- **Consumer disputed?**: Target variable indicating if the customer disputed (yes/no).
- **Complaint ID**: Unique identifier for each complaint.

## Methodology
### Data Preparation
1. **Import Libraries and Load Dataset**:
   - Import necessary libraries such as pandas, seaborn, matplotlib, sklearn, and nltk.
   - Load the dataset into a pandas DataFrame.

2. **Data Wrangling and Feature Engineering**:
   - Handle missing values and perform data cleaning.
   - Create new features if necessary to improve model performance.

3. **Text Pre-processing**:
   - Use Natural Language Processing (NLP) techniques to clean and preprocess the text fields (e.g., 'Issue').

### Exploratory Data Analysis (EDA)
1. **Visualize Data**:
   - Use seaborn and matplotlib to create various plots (e.g., histograms, bar charts) to understand feature distributions and relationships.

### Model Building
1. **Train and Evaluate Models**:
   - Train multiple classifiers and evaluate their performance:
     - Logistic Regression
     - Decision Tree Classifier
     - Random Forest Classifier
     - AdaBoost Classifier
     - Gradient Boosting Classifier
     - K-Neighbors Classifier
     - XGBoost Classifier
   - Compare models based on test and validation accuracy.

2. **Select Best Model**:
   - Logistic Regression gave the most accurate results.

3. **Predict and Save Results**:
   - Use the Logistic Regression model to predict outcomes for the test dataset.
   - Save the predictions in the test file's 'dispute' column.

## Folder Structure
- `data/`: Contains the dataset files.
- `notebooks/`: Jupyter notebooks for data analysis, modeling, and testing.
- `src/`: Python scripts for data processing and model building.
- `models/`: Saved models and their performance metrics.
- `api/`: Saved api code (if any).
- `docs/`: Output files including predictions and evaluation results.

## Installation and Usage
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/MariahFerns/Customer-Dispute-Prediction.git
   cd Customer-Dispute-Prediction

2. **Install the required libraries**:
   ```bash
   pip install -r requirements.txt

3. **Run Jupyter Notebooks**:
   Navigate to the notebooks/ folder and open the notebooks to explore data analysis and model development.

## Results and Findings
- EDA Insights:
  - Visualizations provided insights into feature distributions and potential correlations.
- Model Performance:
  - Logistic Regression outperformed other models with the highest accuracy.
- Predictions:
  - The final predictions were saved in the test file, ready for business action.

## Conclusion
This project successfully developed a predictive model for customer disputes. The Logistic Regression model was the most effective, providing accurate predictions to help the business team manage customer complaints efficiently.
