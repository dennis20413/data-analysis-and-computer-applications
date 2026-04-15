# 🛒 Unit 05: Descriptive Statistics & Forensic EDA — The Black Friday Bot Autopsy

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
*(The execution results of the Bot Anomaly Detector and Server Load Dashboard are attached below)*

---
