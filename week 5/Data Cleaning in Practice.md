# 🏗️ Unit 04: Data Cleaning in Practice

## 📝 Overview: The War Against GIGO
**Data Cleaning** is the process of fixing or removing incorrect, corrupted, incorrectly formatted, duplicate, or incomplete data within a dataset. In Data Science, we follow the principle of **GIGO (Garbage In, Garbage Out)**: even the most advanced AI model will fail if fed with "dirty" data.

This week covers the essential transition from **Raw Data** to **Analysis-Ready Data**.

---

## 🔑 Weekly Glossary (Data Sanitization)

| English Term | Technical Role |
| :--- | :--- |
| `np.nan` | The universal placeholder for "Not a Number" (Missing Data). |
| `df.isnull().sum()` | The "Morning Health Check" for data pipelines—counts errors per column. |
| **Imputation** | The act of "guessing" or replacing missing values with statistical logic. |
| **Type Casting** | Forcing data from one format (e.g., String "100") to another (e.g., Int 100). |
| **Z-Score** | A statistical measure to identify outliers mathematically ($Z > 3$). |

---

## 🧪 Classic Labs: The Data Scrubbing Essentials (01-20)

### 1. Diagnosing Data Corruption
* **The Null Mask:** Using `.isnull()` converts a complex dataset into a simple **Boolean Grid** (True/False). Since computers process 1s and 0s better than empty space, this is the first step in any automated cleaning script.
* **Health Audits:** `.info()` provides a 1-second diagnostic for datasets with millions of rows, showing exactly where the "holes" are.

### 2. Handling Missing Values (NaN)
* **Strict Deletion (`.dropna()`):** Guarantees mathematical purity but risks losing valuable lateral data.
* **Smart Imputation (`.fillna()`):**
    * **Zero Fill:** Best for counts (e.g., "Days Absent").
    * **Statistical Mean:** The gold standard for financial data, preserving the average without shifting the distribution.
    * **Categorical "Unknown":** Essential for Machine Learning, allowing the AI to treat "Missing" as its own unique cluster.

### 3. The Clone Purge (Duplicates)
* Real-world data often suffers from "Double-Billing" or accidental double-clicks.
* **Strategy:** Use `.duplicated()` as a radar to find clones and `.drop_duplicates()` to restore system integrity before performing any `.sum()` operations to avoid corporate fraud.

### 4. String & Type Re-Alignment
* **Invisible White Space:** Computers see "Bob" and "Bob " as two different entities. `.str.strip()` acts as a laser to burn off hidden spaces.
* **Type Camouflage:** If `.info()` says a number is an `object`, math functions will "glue" them together (100 + 200 = 100200). `.astype(int)` is the mandatory fix.

---

## 🔥 Elite Advanced Labs: Professional Wrangling

### 1. RegEx & Advanced Formatting
* **Text Warhead (RegEx):** Using `str.replace('[$,]', '', regex=True)` allows us to annihilate monetary symbols ($ ,) instantly, turning text into calculable integers.
* **Forward Fill (`ffill`):** Critical for **Time-Series** (Stocks/Sensors). It assumes today's value is the same as yesterday's if the sensor blacked out.

### 2. Logical Constraints & Binning
* **Biologically Impossible Records:** Data can be technically perfect but logically wrong (e.g., Age = 305). We use bitwise filtering to enforce **Logic Bounds**.
* **Marketing Cohorts (`pd.cut()`):** Converting "Numerical Noise" (Age 22, 23, 24) into "Categorical Logic" (Young Adult) to help AI models find clearer patterns.

### 3. Machine Learning Readiness
* **One-Hot Encoding (`get_dummies`):** Algorithms cannot multiply "Male" x "Female". This converts categories into binary arrays (0s and 1s), the official language of AI models.
* **Z-Score Anomaly Detection:** Instead of guessing "outliers," we use `scipy.stats` to identify data points that are 3+ standard deviations away from the mean—the mathematical threshold for "Abnormal."


---

## 💡 Student Life Transformation (Reflection)
I am building **"Automated Data Washing Machines"** for my projects:
1.  **League of Legends Scraper:** Automatically stripping "Gold" string symbols ($) and converting them to integers for KDA/Gold analysis.
2.  **IELTS Vocabulary Tracker:** Using `.str.title()` and `.str.strip()` to ensure my English word lists don't have duplicates due to chaotic capitalization.
3.  **Political Gen Z Analysis:** Using `errors='coerce'` in `to_datetime()` to fix garbage date formats from voter registration surveys.

---

## 🛠️ Tech Stack & Skills
* **Libraries:** Pandas, NumPy, Scipy.stats
* **Workflows:** Method Chaining (`\`), ETL Pipelines, Data Imputation.
* **Mindset:** **"Clean once, automate forever."** I now wrap my cleaning logic into `def` functions for industrial-scale processing.

---

### 📸 Lab Execution Gallery
<img width="894" height="775" alt="image" src="https://github.com/user-attachments/assets/7aa1c76c-3a0e-4d94-b770-d5017c2555e7" />
<img width="1001" height="594" alt="image" src="https://github.com/user-attachments/assets/538231e1-9ba5-4edd-8c19-585fc7be73a2" />
<img width="813" height="579" alt="image" src="https://github.com/user-attachments/assets/98ca7235-d336-4e5c-9e36-f28c3a721c2d" />
<img width="832" height="693" alt="image" src="https://github.com/user-attachments/assets/461f51ad-8995-4f08-bd17-31fb9ac224a3" />
<img width="850" height="659" alt="image" src="https://github.com/user-attachments/assets/0b3e9d58-130a-412c-96f5-74e881f4f10d" />
<img width="844" height="634" alt="image" src="https://github.com/user-attachments/assets/5cb13e10-7bc8-4007-9e26-a789c16c0ab8" />
<img width="831" height="748" alt="image" src="https://github.com/user-attachments/assets/947d8b08-8973-4df8-a8ef-50e8c3872d69" />
<img width="1020" height="582" alt="image" src="https://github.com/user-attachments/assets/537e8aac-2c0a-4926-98a0-cbdf2f1948b0" />
<img width="1226" height="602" alt="image" src="https://github.com/user-attachments/assets/2bd85c54-2177-40c2-bff1-8ab734801bbb" />
<img width="926" height="549" alt="image" src="https://github.com/user-attachments/assets/74a3f92f-62dd-41df-81d6-d6cfef7a4115" />
<img width="878" height="551" alt="image" src="https://github.com/user-attachments/assets/3b7f0062-18dc-409b-a27e-58f76bfbd582" />
<img width="951" height="621" alt="image" src="https://github.com/user-attachments/assets/e3e08a98-5d0c-4789-af2d-f855ed63505c" />
<img width="794" height="507" alt="image" src="https://github.com/user-attachments/assets/f968e022-86c4-4e31-a1a8-bc96ba0ce1aa" />
<img width="1205" height="769" alt="image" src="https://github.com/user-attachments/assets/0d087081-0492-40e6-86c6-9b4631d9a379" />

