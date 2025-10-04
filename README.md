# 🚗 Ford Car Price Prediction using Linear Regression

### 🧰 Libraries Used

* **NumPy**
* **Pandas**
* **Matplotlib**
* **Seaborn**
* **Scikit-Learn**

---

## 📘 About the Dataset

| Column Name      | Description                                                |
| ---------------- | ---------------------------------------------------------- |
| **model**        | Ford Car Model                                             |
| **year**         | Production Year                                            |
| **price**        | Price of the Car (in $)                                    |
| **transmission** | Type of Transmission (Automatic / Manual / Semi-Auto)      |
| **mileage**      | Number of Miles Traveled                                   |
| **fuel_Type**    | Type of Fuel (Petrol / Diesel / Hybrid / Electric / Other) |
| **tax**          | Annual Tax                                                 |
| **mpg**          | Miles per Gallon                                           |
| **engineSize**   | Car’s Engine Size                                          |

**Target Variable:** `price`
**Independent Variables:** All other columns

---

## 🧪 Project Workflow

### 1️⃣ Data Loading

Loaded the dataset using **Pandas** and performed initial inspection.

### 2️⃣ Exploratory Data Analysis (EDA)

* Checked for **null values** and **duplicate records**.
* Analyzed the relationship between each independent variable and the dependent variable (`price`) using visualizations.

### 3️⃣ Data Cleaning

* Removed duplicate entries.

### 4️⃣ Data Processing

* Encoded categorical features using **Label Encoding** and **One-Hot Encoding**.
* Standardized numerical variables using **StandardScaler**.

### 5️⃣ Splitting the Dataset

* Split the data into **training (80%)** and **testing (20%)** sets.

### 6️⃣ Model Training

* Trained a **Linear Regression** model using `X_train` and `y_train`.

### 7️⃣ Model Testing

* Tested the model on `X_test` and generated predictions (`y_pred`).

### 8️⃣ Model Evaluation

* Evaluated model performance using:

  * **R² Score**
  * **Adjusted R² Score**

---

## 📊 Results

| Encoding Technique   | R² Score | Adjusted R² Score |
| -------------------- | -------- | ----------------- |
| **One-Hot Encoding** | 0.86     | 1.82              |
| **Label Encoding**   | 0.80     | 0.67              |

✅ **Conclusion:**
The Linear Regression model achieved better performance with **One-Hot Encoded data**, indicating that detailed categorical representation improves accuracy.

---

## 💡 Key Takeaways

* Proper **data preprocessing** (encoding & scaling) significantly impacts model accuracy.
* **One-Hot Encoding** works better for categorical data with non-ordinal relationships.
* **Linear Regression** serves as a good baseline model for price prediction problems.
