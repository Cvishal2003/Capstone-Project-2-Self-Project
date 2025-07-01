
## 📊 Capstone Project 2 – AI Tool Usage by Indian College Students (2025)

This capstone project investigates the **usage patterns of AI tools** (such as ChatGPT, Gemini, and GitHub Copilot) among Indian college students, specifically for academic purposes. The dataset was collected through a survey conducted in **May 2025**, featuring responses from **496 students** across various academic streams and years.

---

### 📁 Dataset Overview

* **Total Records:** 496 students
* **Features:** 16
* **Source:** Google Forms Survey (May 2025)
* **File Used:** `Students.csv`

**Key Features:**

* `Year_of_Study`, `Daily_Usage_Hours`, `Trust_in_AI_Tools`, `Awareness_Level`, `Impact_on_Grades`
* Type of AI tools used, academic use cases, professor approval, device type, internet quality

---

### 🧪 Project Workflow

The project follows a complete **data science pipeline**, from data cleaning to model building and visualization:

#### 1. **Data Exploration & Cleaning**

* Loaded and inspected the raw dataset
* Handled missing values using **median/mode imputation**
* Removed duplicate entries
* Applied **one-hot encoding** to categorical variables

#### 2. **Data Visualization** (Matplotlib / Seaborn)

* Distribution plots: histograms, boxplots
* Categorical visualizations: bar charts, pie charts
* Correlation heatmap and pair plots

#### 3. **Feature Engineering**

* Created interaction and polynomial features
* Skipped binary columns during scaling
* Applied **StandardScaler** to numerical features

#### 4. **Model Building & Evaluation**

**Models Applied:**

* Linear / Logistic Regression (baseline)
* Decision Tree
* Random Forest
* K-Nearest Neighbors

**Performance Metrics:**

* **Regression:** RMSE, R² Score
* **Classification:** Accuracy, F1-Score
* Visual comparison using **bar plots**

#### 5. **Hyperparameter Tuning**

* Used **RandomizedSearchCV** for regression models
* Applied **GridSearchCV** for classification models
* Tuned models compared against baseline for performance gains

---

### 📈 Power BI / Tableau Visualization

Due to GitHub size limitations, the cleaned dataset (`cleaned_preprocessed_students_data.csv`) could not be uploaded.

However, this file was used to build interactive dashboards in **Power BI** / **Tableau**, covering:

* Trust level vs. daily usage hours
* Distribution of preferred AI tools
* Awareness trends by academic year
* Influence of device type and internet quality on grades

---

### 📝 Key Findings

* **2nd-year students** reported the highest AI tool usage.
* **ChatGPT** was the most popular tool, with high trust levels (Trust score = 5).
* The **Random Forest (tuned)** model achieved the best predictive performance.
* Positive correlation observed between **AI awareness/usage** and **grade improvement**.

---

### 📂 Repository Structure

```
Capstone_Project_2/
├── Capstone2_AI_Student_Usage.ipynb           # Main analysis notebook
├── Students.csv                                # Raw dataset
├── cleaned_preprocessed_students_data.csv     # Cleaned data (used for BI dashboards)
├── README.md                                   # Project overview and documentation
```

