# Student Marks Prediction Using Logistic Regression

## 📖 Overview
This project predicts the **average marks (mean score)** of students based on their **demographic and educational background** data.  
Using **Logistic Regression**, the aim is to analyze how various factors such as **gender**, **race/ethnicity**, **lunch type**, **parental level of education**, and **test preparation course** impact student performance.

---

## 🧩 Methodology

### 1. Data Loading & Exploration
- Loaded dataset (`StudentsPerformance.xlsx`) and explored its structure and basic statistics.  
- Created a new feature **"mean score"** by averaging the math, reading, and writing scores.  
- Visualized data using **count plots**, **bar plots**, **pie charts**, **pair plots**, and **heatmaps** to understand relationships and correlations.

### 2. Data Preprocessing
- Converted categorical columns (`gender`, `race/ethnicity`, `parental level of education`, `lunch`, `test preparation course`) into numerical format using `LabelEncoder`.  
- Dropped individual scores (`math`, `reading`, `writing`) to focus solely on predicting the **mean score**.

### 3. Model Building
- Split the dataset into **training (80%)** and **testing (20%)** sets.  
- Built a **Logistic Regression model** using `liblinear` solver.  
- Trained the model and made predictions on the test data.

### 4. Evaluation
- Compared predicted mean scores with actual values.  
- Calculated **average error ≈ 11.03 marks**.

---

## 📊 Key Insights
- Students who **completed test preparation courses** achieved higher mean scores.  
- Those who **brought their own lunch** performed better than students receiving free/reduced lunch.  
- Students with **parents having higher education (e.g., Master’s degree)** tended to score better.  
- **Gender** showed minimal correlation with performance.

---

## 📈 Visualization Examples
- **Count plots** for gender and race/ethnicity distribution.  
- **Pie chart** for test preparation completion rates.  
- **Bar plots** showing mean score differences by lunch type and parental education.  
- **Heatmap** showing correlations among variables.  
- **Pair plots** to explore relationships across all features.

---

## ⚙️ Technologies Used
- **Python 3.x**
- **Pandas**, **NumPy** – data handling  
- **Matplotlib**, **Seaborn** – visualization  
- **Scikit-learn** – preprocessing, model building, evaluation  

---

