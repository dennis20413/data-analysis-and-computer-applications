# 🛒 Descriptive Statistics & Forensic EDA — The Black Friday Bot Autopsy

## 📝 Executive Summary
This project focuses on **Forensic Exploratory Data Analysis (EDA)** within a high-pressure e-commerce environment. By analyzing server traffic logs from a simulated Black Friday crash, I utilized descriptive statistics to distinguish organic human shoppers from malicious bot activity. The primary objective was to establish traffic baselines and identify anomalies that threaten system integrity and marketing data accuracy.

---

## 🔑 Weekly Glossary (Forensic Metrics)

| Metric Dimension | Role in Cyber Security & E-Commerce | Evaluation Tools |
| :--- | :--- | :--- |
| **Central Tendency** | Defines the "Normal" human engagement baseline for the site. | Mean, Median, Mode. |
| **Dispersion** | Measures the volatility and chaos of traffic surges during peak events. | Variance, Std Deviation, Range. |
| **Shape** | Detects non-human patterns (e.g., rapid-fire requests) via distribution skewness. | Skewness, Kurtosis. |

---

## 🧪 Fundamental Labs: Central Tendency & Dispersion

### 1. Establishing the Organic Baseline
* **Mean (The Golden Mean):** Measures the site's average attention span. While useful for general trends, it is vulnerable to "Poisoning" by high-frequency bot requests.
* **Median (The Forensic Anchor):** The most reliable metric for human behavior. It remains "bulletproof" against bot-driven outliers, providing the true middle-point of organic traffic.
* **Mode (Core Audience Behavior):** Identifies the most frequent session length, revealing the primary "heartbeat" of the platform's user base.

### 2. Measuring Network Volatility
* **Standard Deviation:** Defines the **Stability Band** (Mean ± 1 SD). Anything outside this band during a surge is flagged as a potential DDoS or scalper bot attempt.
* **Interquartile Range (IQR):** Focuses on the middle 50% of "Normie" shoppers. This metric is critical for isolating the core workforce of the website from extreme high-engagement anomalies.

---

## 🏢 B2 Case Study: The Black Friday Bot Autopsy (30 Labs Breakdown)

In this industry simulation, we acted as the Lead Data Analyst Team performing a post-mortem on **ShopZen** server logs.

### Phase 1: 20 Core EDA Missions (Cyber Security Essentials)
These labs focus on filtering out "Bot Noise" and establishing human-centric benchmarks.
* **Traffic Quality Baseline (Lab 01-02):** Initializing server logs and using `.describe()` with **Boxplots** to define the physical limits of human engagement.
* **Scalper Bot Detection (Lab 03-05):** We identified a **Malicious Bot (Score: 9999)**. This lab demonstrated how a bot can destroy the **Mean** while the **Median** successfully anchors the data to organic reality.
* **Engagement Filtering (Lab 06-15):** * **Bouncing Hits (`.min()`):** Flagging immediate exits that indicate link-scrapers or dead-link bots.
    * **VIP Whales (`.max()`):** Identifying high-value human users for retention marketing.
    * **Quantile Slicing:** Using **Q1** to remove low-engagement "Landing Bouncers" and **Q3** to isolate top-tier spenders.
* **Network Segmentation (Lab 16-20):** * Calculating total **Compute-Hours** (`.sum()`) to audit server burden.
    * Using **Swarmplots** and **Boxplots** to compare site performance across Free vs. Premium account tiers.

### Phase 2: 10 Advanced EDA Missions (Advanced Pattern Recognition)
These labs utilize complex statistical logic to catch sophisticated, stealthy bots.
* **Firewall Anomaly Protocols (Adv 01-03):** Implementing **Tukey’s Fences** ($Q3 + 1.5 \times IQR$) to mathematically isolate "Micro-bots" that were designed to bypass simple filters.
* **Compounding & Signal Processing (Adv 04-06):** * **Cumulative Traffic (`.cumsum()`):** Geometrically mapping the total traffic mass accumulation over the Black Friday window.
    * **Signal Smoothing (`.rolling()`):** Applying **Moving Averages** to flatten chaotic API ping noise and reveal the true human heartbeat of the site.
* **Correlation & Decision Matrices (Adv 07-10):** * **Correlation Heatmaps:** Proving the relationship between session duration and engagement.
    * **Conversion Crosstabs:** Intersecting account tiers with purchase success ratios to audit conversion efficiency under pressure.
    * **Multi-Engine Aggregations (`.agg()`)**: Generating a master "Omni-Report" for the CEO, displaying minimum, average, and peak server capacity pulled by distinct account groups.

---

## 💡 Student Life Transformation (Reflection)
Integrating Forensic EDA into my professional Data Science toolkit:
1. **Cyber Defense:** Moving beyond subjective monitoring to use **Tukey's Fences** and **Z-Scores** as objective, mathematical firewalls against non-human traffic.
2. **Business Intelligence:** Recognizing that a single bot can poison a dataset. I now prioritize the **Median** and **IQR** for accurate strategic planning in e-commerce.
3. **Signal vs. Noise:** Utilizing **Moving Averages** to filter out erratic API spikes, allowing me to focus on true organic trends and customer behavior.

---

## 🛠️ Tech Stack & Skills
* **Programming:** Python (Pandas, NumPy, Scipy.stats).
* **Visual Engines:** Matplotlib, Seaborn.
* **Core Competencies:** Forensic Data Auditing, Anomaly Detection, Time-Series Smoothing, Categorical Matrix Analysis, Statistical Imputation.

---

### 📸 Lab Execution Gallery
<img width="758" height="254" alt="image" src="https://github.com/user-attachments/assets/b89d6fbb-082a-45bc-bb54-71eef2b7d998" />
<img width="836" height="703" alt="image" src="https://github.com/user-attachments/assets/6b3d2bdd-1a58-4b81-9be1-6db72e86d879" />
<img width="930" height="684" alt="image" src="https://github.com/user-attachments/assets/eeab902b-1acc-485c-8b4e-0ef46498849f" />
<img width="1402" height="737" alt="image" src="https://github.com/user-attachments/assets/d5d14422-1ea8-4971-863d-33ba5351e134" />
<img width="928" height="673" alt="image" src="https://github.com/user-attachments/assets/ca6bc485-00bf-408d-8901-5725992d1f4c" />
<img width="941" height="634" alt="image" src="https://github.com/user-attachments/assets/4bc282b4-ff0e-4df1-8b70-63abd0230fa6" />
<img width="842" height="663" alt="image" src="https://github.com/user-attachments/assets/2311fa42-5037-41ee-8b41-8c78cebd410e" />
<img width="863" height="655" alt="image" src="https://github.com/user-attachments/assets/e9e3e543-b699-4bf5-b32e-9c76618fb303" />
<img width="880" height="671" alt="image" src="https://github.com/user-attachments/assets/36ef7a8a-b328-4fdb-ba16-cf31ab61ccd7" />
<img width="840" height="641" alt="image" src="https://github.com/user-attachments/assets/bdebb7e6-5e22-462b-8b2f-133665f7670a" />
<img width="945" height="689" alt="image" src="https://github.com/user-attachments/assets/19482ad7-77df-4e47-8ea3-de850ab299c4" />
<img width="1404" height="694" alt="image" src="https://github.com/user-attachments/assets/8eea2569-7839-4f13-b770-c925b2592ea7" />
<img width="882" height="616" alt="image" src="https://github.com/user-attachments/assets/9258b829-02e0-4973-b6f6-fa594ac4c7eb" />
<img width="874" height="661" alt="image" src="https://github.com/user-attachments/assets/b161cd98-a5d9-4dc3-a9fe-799dcb18985f" />
<img width="956" height="651" alt="image" src="https://github.com/user-attachments/assets/5aaf1bb5-2f0e-4c21-b122-bffa75eb9370" />
<img width="1137" height="566" alt="image" src="https://github.com/user-attachments/assets/3d3148bd-f699-476d-8ee7-cfe6314647d2" />
<img width="1436" height="714" alt="image" src="https://github.com/user-attachments/assets/27affbe3-f209-4fc7-8a44-9a540efc8c7d" />
<img width="898" height="649" alt="image" src="https://github.com/user-attachments/assets/b97ee84d-f3f8-4584-b7f6-9727846394c3" />
<img width="850" height="630" alt="image" src="https://github.com/user-attachments/assets/ef818bde-3f1d-4bb3-bb68-8e7ad7eda213" />
<img width="867" height="592" alt="image" src="https://github.com/user-attachments/assets/5dfeb5a0-1dd3-49fb-a925-7be7fbd87de1" />
<img width="892" height="626" alt="image" src="https://github.com/user-attachments/assets/a5315f70-ff0e-4870-abf4-aa49d7bd12ad" />
<img width="840" height="566" alt="image" src="https://github.com/user-attachments/assets/cb9d7a66-cb25-492a-a33c-31db3a2f193a" />
<img width="870" height="745" alt="image" src="https://github.com/user-attachments/assets/b89b1bc1-e221-4897-a4f4-8cf56097c81f" />
<img width="1106" height="558" alt="image" src="https://github.com/user-attachments/assets/ba4468bc-660c-48ce-a699-e75d9b569fd5" />
<img width="871" height="635" alt="image" src="https://github.com/user-attachments/assets/c28e7887-59f4-4fdf-babc-eaaad00fe47a" />
<img width="953" height="656" alt="image" src="https://github.com/user-attachments/assets/182a5922-e0c5-4ebb-b104-53990d369536" />
<img width="935" height="763" alt="image" src="https://github.com/user-attachments/assets/54bdb2bc-bd73-4bb7-aff5-a6d293c224ae" />
<img width="921" height="602" alt="image" src="https://github.com/user-attachments/assets/eeadc327-b16e-4fb9-bd82-1940f8adc7c9" />
<img width="845" height="656" alt="image" src="https://github.com/user-attachments/assets/d24c909e-0ab8-4655-88d1-05759913c169" />
<img width="840" height="664" alt="image" src="https://github.com/user-attachments/assets/3ac8d4dd-454e-4138-8a5d-073ed8a4f087" />
