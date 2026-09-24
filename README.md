🏥 Healthcare Patient & Hospital Analytics Dashboard

An interactive **Power BI Healthcare Analytics Dashboard** developed using a dataset containing **50,000 patient records**.  
The project focuses on analyzing patient information, hospital performance, treatment outcomes, admissions, and financial data to generate meaningful business insights.

---

## 📊 Project Overview

The objective of this project is to transform raw healthcare data into an interactive dashboard that helps analyze:

- Patient demographics
- Medical conditions
- Admission types
- Hospital performance
- Treatment outcomes
- Patient length of stay
- Billing and financial performance
- Healthcare trends and patterns

---

## 📁 Dataset

The dataset contains **50,000 healthcare records** with information such as:

- Patient ID
- Age
- Gender
- Blood Type
- Medical Condition
- Admission Type
- Admission Date
- Discharge Date
- Length of Stay
- Hospital Name
- Attending Doctor
- Systolic BP
- Diastolic BP
- Cholesterol
- Glucose Level
- Insurance Provider
- Billing Amount
- Treatment Outcome

---

# 📌 Dashboard Pages

## 1️⃣ Healthcare Overview

This page provides an overall summary of the healthcare dataset.

### Key Metrics

- 👥 Total Patients
- 💰 Total Billing
- 💵 Average Billing
- 🎂 Average Age
- 🏥 Average Length of Stay
- 🚑 Emergency Patients

### Analysis

- Patient demographics
- Admission type distribution
- Medical condition analysis
- Treatment outcome overview
- Age and gender analysis

---

## 2️⃣ Hospital & Financial Analysis

This dashboard focuses on hospital performance and financial insights.

### Key Analysis

- 🏥 Hospital-wise patient count
- 💰 Hospital-wise billing
- 📈 Average billing by hospital
- 💳 Insurance provider analysis
- 📊 Financial performance
- 🏥 Hospital admission trends

### Business Insights

The dashboard helps understand differences in patient volume, billing amounts, and financial performance across hospitals and insurance providers.

---

## 3️⃣ Patient & Treatment Analysis

This page focuses on patient health information and treatment outcomes.

### Key Analysis

- 🧑‍⚕️ Medical condition analysis
- 💊 Treatment outcome analysis
- 📊 Treatment outcome by medical condition
- 🩺 Average blood pressure
- 🧪 Average glucose level
- 🧬 Average cholesterol
- ⏱️ Length of stay analysis

### Treatment Insights

The dashboard helps identify patterns between medical conditions, patient characteristics, treatment outcomes, and hospital stays.

---

# 📈 Key Performance Indicators (KPIs)

| KPI | Description |
|---|---|
| Total Patients | Total number of unique patients |
| Total Billing | Total healthcare billing amount |
| Average Billing | Average billing per patient |
| Average Age | Average patient age |
| Average Length of Stay | Average hospital stay |
| Emergency Patients | Number of emergency admissions |
| Improved Patients | Patients with improved outcomes |
| Cured Patients | Patients with cured outcomes |

---

# 🧮 DAX Measures

Some important DAX measures used in the project:

```DAX
Total Patients = DISTINCTCOUNT(Healthcare[Patient_ID])

Total Billing = SUM(Healthcare[Billing_Amount_USD])

Average Billing = AVERAGE(Healthcare[Billing_Amount_USD])

Average Length of Stay = AVERAGE(Healthcare[Length_of_Stay_Days])

Average Age = AVERAGE(Healthcare[Age])

Emergency Patients = CALCULATE([Total Patients], Healthcare[Admission_Type] = "Emergency")

Improvement Rate = DIVIDE([Improved Patients],[Total Patients], 0)

---

🔄 Data Preparation
The data was prepared using Power Query.
Data Preparation Steps
Imported the CSV dataset
Checked column data types
Cleaned and transformed data
Handled missing/invalid values where required
Verified numerical and categorical columns
Created relationships where required
Loaded the cleaned data into Power BI
Created DAX measures
Developed interactive dashboards

---

📊 Power BI Features Used
Cards
Bar Charts
Column Charts
Pie/Donut Charts
Matrix
Slicers
Conditional Formatting
Filters
DAX Measures
Tooltips
Interactive Visualizations
Dashboard Navigation

---

🎯 Skills Demonstrated
Data Analytics
Data Cleaning
Data Transformation
Exploratory Data Analysis
KPI Analysis
Business Insights
Power BI
Power Query
DAX
Data Modeling
Interactive Dashboards
Data Visualization
Conditional Formatting
Filters & Slicers

---

💡 Key Insights
The dashboard provides an interactive way to explore:
Patient volume and demographics
Common medical conditions
Admission patterns
Treatment outcomes
Hospital performance
Insurance provider distribution
Billing and financial trends
Patient length of stay
Health indicator averages

---

🚀 Project Outcome
This project demonstrates how Power BI can be used to convert raw healthcare data into meaningful visual insights.
It combines data preparation, DAX calculations, data visualization, KPI tracking, and interactive dashboard development to create a complete healthcare analytics solution.

---

📝 Conclusion
The Healthcare Patient & Hospital Analytics Dashboard provides a comprehensive view of patient, hospital, treatment, and financial data.
By using Power Query, DAX, and Power BI visualizations, the project transforms 50,000 healthcare records into an interactive analytical solution. The dashboard makes it easier to identify patterns in patient demographics, medical conditions, admissions, treatment outcomes, hospital performance, and billing.
Overall, this project demonstrates practical data analytics, data visualization, and business intelligence skills that can be applied to real-world healthcare datasets.

---

👩‍💻 Author
Pooja Etcherla
Aspiring Data Analyst | Power BI | SQL | Python | Tableau | Excel

### 📁 Recommended GitHub folder structure

```text
Healthcare-PowerBI-Analytics/
│
├── 📊 Dashboard/
│   └── Healthcare_Analytics.pbix
│
├── 📂 Dataset/
│   └── cleaned_healthcare_dataset_50k.csv
│
├── 🖼️ images/
│   ├── healthcare-overview.png
│   ├── hospital-financial-analysis.png
│   └── patient-treatment-analysis.png
│
└── 📄 README.md
