# Descriptive Statistics & Bio-Metric EDA — The Smartwatch Health Tracker

## 📝 Executive Summary
This project focuses on **Physiological Exploratory Data Analysis (EDA)** using beta-tester data from the "AuraFit" next-gen fitness wearable. The primary objective was to audit the mathematical relationship between biological metrics (Resting Heart Rate) and health outcomes (Health Scores). By performing a "post-mortem" on sensor datastreams, I established frameworks for hardware validation, detected sensor malfunctions, and cross-validated training modalities (Cardio vs. Strength).

---

## 🔑 Weekly Glossary (Bio-Metric Metrics)

| Metric Dimension | Technical Role in Wearable Tech | Evaluation Tools |
| :--- | :--- | :--- |
| **Central Tendency** | Defines the "Biological Baseline" for a user's resting state. | Mean, Median, Mode. |
| **Dispersion** | Measures physiological volatility and training intensity zones. | Variance, Std Deviation, Range. |
| **Shape** | Evaluates the health distribution and identifies systematic biases. | Skewness, Kurtosis. |

---

## 🧪 Fundamental Labs: Central Tendency & Dispersion

### 1. Establishing the Physiological Baseline
* **Mean (The Golden Health Average):** Measures the average fitness level of beta-testers. While it represents the "Golden Index," it is easily skewed by hardware glitches.
* **Median (The Biological Anchor):** The most reliable metric for true human physiology. It remains "bulletproof" against sensor noise, such as vibrations that create fake high scores.
* **Mode (Typical Heartbeat):** Identifies the most common biometric base, revealing the natural resting state of the majority of users.

### 2. Mapping Metabolic Variance
* **Standard Deviation:** Defines the **Safe Training Zone** (Mean ± 1 SD). Data points outside this band may indicate arrhythmia, extreme stress, or dangerous over-training.
* **Interquartile Range (IQR):** Focuses on the middle 50% "Core Athletes." This helps in understanding the typical biological width of the test population.



---

## 🏢 B3 Case Study: AuraFit Beta-Tester Data Audit (30 Labs Breakdown)

In this industry simulation, I acted as the Lead Data Scientist performing a forensic audit of hardware sensor datastreams.

### Phase 1: 20 Core EDA Missions (Bio-Metric Essentials)
* **Sensor Initialization & Baseline (Lab 01-02):** Binding raw Bluetooth sink data (Resting_HR) into the visual engine to assess the initial distribution of tester health.
* **Hardware Glitch Diagnostic (Lab 03-05):** We identified a **Gyroscope Malfunction (Score: 9999)** caused by external vibration. This lab demonstrated how visual distortion acts as a direct debug tool for hardware failure.
* **Physiological Risk Tracking (Lab 06-15):** * **Bradycardia Flagging (`.min()`):** Using the minimum value to identify at-risk users with abnormally low health or heart rate metrics.
    * **Elite Athlete Threshold (`.max()`):** Isolating the "Maximum Potential Output" of top-tier endurance runners.
    * **Quantile Segmentation:** Using **Q1** to filter sedentary "Couch Potatoes" and **Q3** to isolate "Elite Endurance Athletes."
* **Clinical Trial Dissection (Lab 16-20):** * Calculating **Total Combined Heartbeats** (`.sum()`) to audit battery strain.
    * Using **Boxplots** and **Swarmplots** to cross-compare clinical outcomes between **Cardio** vs. **Strength** training groups.

### Phase 2: 10 Advanced EDA Missions (Hardware & Feature Analytics)
* **Hardware Cutoff Quarantine (Adv 01-03):** Implementing **Tukey’s Fences** ($Q3 + 1.5 \times IQR$) to create an automated "Anomaly Detector" that terminates sensor errors or over-clocked biological readings.
* **Metabolic Tracking & Smoothing (Adv 04-06):** * **Cumulative Burn (`.cumsum()`):** Geometrically mapping the total calories/metabolic mass accumulated throughout a workout cycle.
    * **Biological Smoothing (`.rolling()`):** Applying **Moving Averages** to eliminate "Jitter Noise" caused by erratic movements (e.g., sneezes) from the wearable sensors.
* **Physiological Relationships (Adv 07-10):** * **Pearson Matrix Analysis:** Proving the negative correlation between Resting_HR and Fitness—validating that a deeper resting rate signals superior cardiovascular performance.
    * **Clinical Output Matrix:** Using **Crosstabs** and **Multi-Engine Aggregations (`.agg()`)** to blast simultaneous metrics (min, mean, max) for an executive dashboard.



---

## 💡 Student Life Transformation (Reflection)
Integrating Bio-Metric EDA into my technical professional toolkit:
1. **Hardware Integrity:** I now utilize **Boxplots** and **Outlier Detection** as mandatory diagnostic tools to distinguish between true human data and sensor hardware glitches.
2. **Clinical Validation:** Moving beyond guesswork to use **Quantiles (Q1/Q3)** to objectively separate sedentary users from elite athletes based on data distribution.
3. **Feature Development:** Utilizing **Correlation Matrices** to understand physiological relationships, enabling the development of tailored features for specific user groups (e.g., tailoring metrics based on Cardio vs. Strength dynamics).

---

## 🛠️ Tech Stack & Skills
* **Programming:** Python (Pandas, NumPy, Scipy.stats).
* **Visualization:** Matplotlib, Seaborn.
* **Competencies:** Bio-Metric Data Auditing, Sensor Hardware Troubleshooting, Imputation, Correlation Mapping, Multi-Engine Aggregate Pipelines.

---

### 📸 Lab Execution Gallery
<img width="722" height="255" alt="image" src="https://github.com/user-attachments/assets/5ca75d9c-d1d4-4937-930c-c870e4f52521" />
<img width="799" height="714" alt="image" src="https://github.com/user-attachments/assets/5c8e9a57-3c1c-40ad-93f0-9fe5817ffaba" />
<img width="806" height="676" alt="image" src="https://github.com/user-attachments/assets/87df70f9-c7e8-4c6b-ad65-4f9c7d3329c3" />
<img width="1388" height="714" alt="image" src="https://github.com/user-attachments/assets/3f302c97-d701-4a7d-8d04-4d0b29943a24" />
<img width="829" height="676" alt="image" src="https://github.com/user-attachments/assets/b0fda591-395d-4218-8efa-0968a99b48cd" />
<img width="869" height="635" alt="image" src="https://github.com/user-attachments/assets/2d64e8b1-7589-4a3d-8f03-a085ec3d236c" />
<img width="827" height="646" alt="image" src="https://github.com/user-attachments/assets/5f0f8192-c7cf-4294-9635-1e42805bff08" />
<img width="749" height="646" alt="image" src="https://github.com/user-attachments/assets/7d7f17a4-a459-44a5-910e-da7507152fc2" />
<img width="812" height="674" alt="image" src="https://github.com/user-attachments/assets/4f4442d1-c82c-4647-99f4-35c080bed4ce" />
<img width="793" height="622" alt="image" src="https://github.com/user-attachments/assets/90281678-7ed2-45e8-b5e1-b38ed351cc8d" />
<img width="1046" height="696" alt="image" src="https://github.com/user-attachments/assets/55a2b169-b8f6-4917-aa6b-bc7c8d128dfe" />
<img width="1419" height="696" alt="image" src="https://github.com/user-attachments/assets/15f48ca7-c29d-4d6d-a439-991de6124f97" />
<img width="899" height="623" alt="image" src="https://github.com/user-attachments/assets/93407e3c-792b-41e6-8262-8415f87ad467" />
<img width="812" height="659" alt="image" src="https://github.com/user-attachments/assets/c05cc050-f793-4f2c-a8ea-51388cde792c" />
<img width="876" height="647" alt="image" src="https://github.com/user-attachments/assets/a4763061-30d2-43ce-a384-3e811b68cdd0" />
<img width="1138" height="568" alt="image" src="https://github.com/user-attachments/assets/858a36c3-7701-4137-beb7-7292d16c5cf8" />
<img width="1389" height="701" alt="image" src="https://github.com/user-attachments/assets/43086898-dc69-4c3e-b7f8-b5ca07552ea6" />
<img width="841" height="635" alt="image" src="https://github.com/user-attachments/assets/6b6a6541-8c11-46f4-9aa6-ba823ea9aaea" />
<img width="820" height="639" alt="image" src="https://github.com/user-attachments/assets/8d95e43e-f63d-4b6c-b158-f8b921252e5f" />
<img width="913" height="587" alt="image" src="https://github.com/user-attachments/assets/a85e3263-d8a7-4ee6-9c05-4606e7b853c6" />
<img width="877" height="627" alt="image" src="https://github.com/user-attachments/assets/867041fd-ab04-45d1-bb47-9612541abf47" />
<img width="863" height="578" alt="image" src="https://github.com/user-attachments/assets/f65f9f5c-a171-4d11-a7e7-af8be2b203e2" />
<img width="850" height="732" alt="image" src="https://github.com/user-attachments/assets/4f95ce75-c37f-4a4e-a5a7-18f7c3c23ad6" />
<img width="1142" height="560" alt="image" src="https://github.com/user-attachments/assets/76995e97-2343-4a53-a4e7-bab752b59f4c" />
<img width="842" height="622" alt="image" src="https://github.com/user-attachments/assets/4c0e7aa5-fe4a-4fbc-80f9-a6cfb3054ee0" />
<img width="897" height="644" alt="image" src="https://github.com/user-attachments/assets/8be0ab58-2eb3-4dc2-8041-e32b394a3455" />
<img width="889" height="627" alt="image" src="https://github.com/user-attachments/assets/a14e3d7b-9455-4ea3-a90f-f786439f0195" />
<img width="856" height="594" alt="image" src="https://github.com/user-attachments/assets/a6f9c148-9fd9-4b6b-ab6c-4b4c585e8c4b" />
<img width="795" height="648" alt="image" src="https://github.com/user-attachments/assets/b4fc5d69-6994-4e38-9500-d0aaffb573a6" />
<img width="848" height="664" alt="image" src="https://github.com/user-attachments/assets/3eb5d80e-8e84-4f0b-8f81-d85a94d5dfe7" />
