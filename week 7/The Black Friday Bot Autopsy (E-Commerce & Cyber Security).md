# 🛒 Unit 05: Descriptive Statistics & Forensic EDA — The Black Friday Bot Autopsy

## 📝 Executive Summary
This unit focuses on **Exploratory Data Analysis (EDA)** within the context of E-commerce and Cyber Security. By analyzing server event logs from a simulated Black Friday traffic surge, I implemented descriptive statistical methods to distinguish between organic human engagement and malicious bot activity. The goal was to perform a data "post-mortem" to establish traffic baselines, identify anomalies, and restore data integrity.

---

## 🔑 Weekly Glossary (Forensic Metrics)

| Dimension | Technical Role in Cyber Security | Evaluation Tools |
| :--- | :--- | :--- |
| **Central Tendency** | Defines the "Normal" human behavior baseline. | Mean, Median, Mode. |
| **Dispersion** | Measures the volatility and chaos of traffic surges. | Variance, Std Deviation, Range. |
| **Shape** | Detects non-human patterns and distribution skewness. | Skewness, Kurtosis. |

---

## 🧪 Fundamental Labs: Central Tendency & Dispersion

### 1. Establishing the Human Baseline
* **Mean (The Golden Mean):** Used to calculate the site's average attention span. While useful, the mean is highly susceptible to "Poisoning" by extreme bot values.
* **Median (Organic Middle):** The "Bulletproof" metric that represents the typical human shopper, effectively ignoring the noise created by rapid-fire bot requests.
* **Mode (Core Behavior):** Identifies the most frequent session length, helping marketing teams understand the typical user's "heartbeat" on the platform.

### 2. Measuring Traffic Chaos
* **Standard Deviation:** Defines the **Stability Band** (Mean ± 1 SD). Data points falling far outside this band during peak sales indicate either a viral human surge or a DDoS attempt.
* **Interquartile Range (IQR):** Filters out the middle 50% of "Normie" traffic, allowing analysts to focus on the extreme ends of the distribution where bots usually hide.



---

## 🏢 B2 Case Study: The Black Friday Bot Autopsy (30 Labs)

In this high-stakes forensic audit of **ShopZen**, the analytics team was tasked with hunting for anomalies after a temporary system crash.

### Phase 1: 20 Core EDA Missions (Forensic Essentials)
* **Traffic Quality Audit (Lab 01-02):** Initializing server logs and using `.describe()` to set the physical baseline for what "Normal" engagement looks like.
* **Scalper Bot Detection (Lab 03-05):** We identified a **Malicious Bot (Score: 9999)** that physically destroyed the data visualization scale. This demonstrated the vital importance of using the **Median** to maintain an organic baseline during a cyber attack.
* **User Behavior Segmentation (Lab 06-15):**
    * **Bouncing Hits (`.min()`):** Flagging immediate exits that indicate potential link-scraper bots.
    * **VIP Whales (`.max()`):** Identifying high-value human shoppers for re-targeting.
    * **Quantile Slicing:** Using **Q1** to remove low-engagement "Bargain Hunters" and **Q3** to isolate the heavy spenders driving revenue.
* **System Load Analytics (Lab 16-20):** Calculating total **Compute-Hours** (`.sum()`) and using **Swarmplots** to analyze the engagement gap between Free and Premium account tiers.

### Phase 2: 10 Advanced EDA Missions (Advanced Pattern Recognition)
* **Firewall Anomaly Protocols (Adv 01-03):** Implementing **Tukey’s Fences** ($Q3 + 1.5 \times IQR$) to mathematically isolate "Micro-bots" that were sneaky enough to bypass basic filters.
* **Compounding Mass & Signal Smoothing (Adv 04-06):** * **Cumulative Traffic (`.cumsum()`):** Geometrically mapping how the server burden accumulated over the 15-minute Black Friday window.
    * **Moving Averages (`.rolling()`):** Applying 3-period smoothing to flatten erratic API ping noise and reveal the true human heartbeat of the site.
* **Decision Matrices (Adv 07-10):**
    * **Correlation Heatmaps:** Proving whether longer session lengths actually correlate with higher engagement scores.
    * **Conversion Crosstabs:** Intersecting account tiers with purchase success ratios to see which demographics survived the system crash.
    * **Multi-Engine Aggregations (`.agg()`)**: Generating a master "Omni-Report" for the CMO, displaying minimum, average, and peak server capacity side-by-side.



---

## 💡 Student Life Transformation (Reflection)
Integrating Forensic EDA into my professional data toolkit:
1. **Cyber Defense:** Moving beyond subjective observations to use **Tukey's Fences** and **Z-Scores** as objective, mathematical firewalls against non-human traffic.
2. **Business Intelligence:** Understanding that a single outlier (like a bot or a whale) can corrupt the **Mean**, making the **Median** and **IQR** more reliable tools for strategic planning.
3. **Signal Processing:** Utilizing **Moving Averages** to filter out "noise" (API spikes) and focus on the "signal" (true organic growth), ensuring marketing budgets are spent on real humans.

---

## 🛠️ Tech Stack & Skills
* **Programming:** Python (Pandas, NumPy, Scipy.stats).
* **Visualization:** Matplotlib, Seaborn.
* **Core Competencies:** Forensic Data Auditing, Anomaly Detection, Time-Series Smoothing, Categorical Matrix Analysis, Statistical Imputation.

---

### 📸 Lab Execution Gallery
