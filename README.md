# Cultural Representation in Video Games: Impact on Player Anxiety & Engagement
*Analyzing the psychological effects of culturally relevant video games through statistical modeling and data-driven insights.*

## Table of Contents
- [Project Overview](#project-overview)
- [Research Questions & Hypotheses](#research-questions--hypotheses)
- [Methodology](#methodology)
- [Data Collection & Preprocessing](#data-collection--preprocessing)
- [Statistical Analysis](#statistical-analysis)
- [Power Analysis](#power-analysis)
- [Results & Key Findings](#results--key-findings)
- [Technologies & Tools Used](#technologies--tools-used)
- [Repository Structure](#repository-structure)
- [How to Use This Repository](#how-to-use-this-repository)
- [Future Work](#future-work)
- [References](#references)

---

## Project Overview
This study investigates **how cultural representation in video games influences player anxiety and engagement**. The research examines whether culturally relevant gaming content affects players differently based on their cultural background.

### Key Objectives:
✅ Understand if **culturally aligned video games reduce player anxiety** compared to non-cultural games.  
✅ Analyze **engagement levels** in culturally relevant vs. non-relevant games.  
✅ Identify **statistically significant predictors** of player anxiety and engagement using **ANOVA, regression, and power analysis**.  
✅ Provide **data-driven insights** to inform culturally inclusive game design.  

---

## Research Questions & Hypotheses

### Primary Research Question:
- Do video games with **cultural representation** influence **player anxiety and engagement**, particularly when the player’s cultural background matches the game’s content?

### Hypotheses:
- **H1:** Players will exhibit **lower anxiety levels post-gameplay** if the game aligns with their cultural background.
- **H2:** Players from **Indian cultural backgrounds will show higher engagement** with Indian-themed games compared to non-Indian participants.
- **H3:** Cultural background and game type will significantly interact to predict **both anxiety reduction and engagement levels**.
- **H4:** Age and prior gaming experience will influence **both anxiety and engagement levels**, with younger players showing stronger effects.

---

## Methodology

### Study Design:
- **Experimental setup:** 2×2 and 2×2×2 **Mixed Factorial ANOVA**
- **Conditions:**
  - **Cultural Game Condition**: Participants exposed to an **Indian culturally relevant game**.
  - **Non-Cultural Game Condition**: Participants exposed to a **game without specific cultural elements**.
- **Participants:** 27 total (23 Indian, 4 Non-Indian)
- **Data Collection Tools:** State-Trait Anxiety Inventory (STAI) & Likert Scale for Engagement

---

## Data Collection & Preprocessing

### Collected Data Variables:
| Variable | Type | Description |
|----------|------|-------------|
| **Age** | Continuous | Participant's age in years |
| **Cultural Background** | Categorical | Indian / Non-Indian |
| **Game Type** | Categorical | Cultural / Non-Cultural |
| **Pre-Session Anxiety Score** | Continuous | Measured using STAI |
| **Post-Session Anxiety Score** | Continuous | Measured using STAI |
| **Engagement Score** | Continuous | Measured using a 5-point Likert scale |

### Preprocessing Steps:
✅ **Missing Data Handling**: Mean imputation for missing values.  
✅ **Outlier Detection**: Boxplots used to detect extreme values in anxiety scores.  
✅ **Standardization**: Likert-scale engagement scores normalized for analysis.  
✅ **Data Validation**: Ensured values were within the STAI and Likert scale ranges.  

---

## Statistical Analysis

### 1. 2×2 Mixed ANOVA – Anxiety Reduction
- **Factors**: Time (Pre vs. Post) × Game Type (Cultural vs. Non-Cultural)
- **Significant Interaction Effect**:  
  - **F(1, 25) = 5.266, p = .030, partial η² = .174**
  - **Conclusion**: Cultural games significantly reduced anxiety levels.

### 2. 2×2×2 Mixed ANOVA – Cultural Background Effects
- **Factors**: Time × Game Type × Cultural Background
- **Key Findings:**  
  - **Main Effect of Cultural Background**: **F(1, 23) = 18.902, p < .001, partial η² = .451**  
  - **Main Effect of Game Type**: **F(1, 23) = 10.577, p = .004, partial η² = .315**  
  - **Interaction Effect**: Cultural background influences anxiety reduction.

### 3. Independent Samples t-Test – Cultural Engagement
- **Significant difference**: **t(25) = 3.301, p = .003, d = 1.788**
- **Conclusion**: Indian participants had **higher engagement** with culturally relevant games.

### 4. Multiple Regression – Predictors of Anxiety Reduction & Engagement
- Anxiety Reduction Model: **Not significant** *(p = .179, R² = .189)*, but game type was a key predictor *(β = .412, p = .043)*.
- Cultural Engagement Model: **Highly significant** *(p < .001, R² = .540)*, cultural background and game type were strong predictors.

---

## Power Analysis
- Conducted using **G*Power**.
- **Effect Size (Partial η² = .174) → Cohen’s d = 0.92**.
- **Achieved Power = 95.07%**, ensuring confidence in the results.

---

## Technologies & Tools Used
✅ **Python (Pandas, NumPy, SciPy, Statsmodels)** – Data preprocessing & analysis.  
✅ **SPSS** – Advanced statistical modeling (ANOVA, regression).  
✅ **G*Power** – Power analysis for effect size calculations.  
✅ **Excel** – Data cleaning & visualization.  

---

<!-- ## Repository Structure

📂 CulturalGamingImpact
│── 📜 README.md (Project Overview & Documentation)
│── 📂 Data (Raw & Processed Experimental Data)
│── 📂 Notebooks (Jupyter Notebooks for Analysis)
│── 📂 SPSS_Outputs (Statistical Test Results)
│── 📂 Power_Analysis (G*Power screenshots & calculations)
│── 📜 cultural_gaming_analysis.ipynb (Main Python Script)
│── 📜 results_summary.pdf (Formatted Report with Findings) -->

## Future Work
- 🚀 Expanding the study to a larger & more diverse participant pool.
- 🚀 Integrating Machine Learning to predict player engagement based on cultural alignment.
- 🚀 Exploring real-time anxiety measurement techniques using biometric data.