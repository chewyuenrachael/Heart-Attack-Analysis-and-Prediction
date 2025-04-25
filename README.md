# ❤️ Heart Attack Analysis and Prediction

This repository investigates the relationship between age and **maximum heart rate (HRmax)** in men, based on data from the **Cleveland Heart Disease Dataset**. It applies **correlation analysis**, **linear regression modeling**, and **hypothesis testing** to assess whether increasing age is associated with a decrease in HRmax, a known risk factor for post-heart attack mortality.

📍 **Key Question**: Is there a statistically significant negative linear association between age and HRmax in men from the Cleveland heart disease population?

---

## 📊 Project Highlights

- ✔️ **Data Source**: Cleveland Clinic Foundation dataset via UCI Machine Learning Repository (1988)
- 🔍 **Focus**: Males only (207 entries)
- 📈 **Techniques Used**:
  - Summary statistics & data visualizations (histograms, scatterplots, Q-Q plots)
  - Pearson correlation coefficient
  - Linear regression (slope, intercept, R²)
  - Residual and normality analysis
  - T-tests for significance of regression coefficients

---

## 📁 File Structure

```
Heart-Attack-Analysis-and-Prediction/
├── Correlation and Regression Code.ipynb   # Main notebook with analysis and visualization
├── Statistical Inference Code.ipynb        # Supplementary statistical testing and interpretation
├── heartattack.csv                         # Cleaned dataset with selected variables
├── Heart Attack Analysis and Prediction.pdf # Full report with discussion and conclusions
└── README.md                               # Project overview
```

---

## 🧠 Key Findings

| Analysis Element | Summary |
|------------------|---------|
| 📉 **Correlation (r)** | -0.409 — A weak negative linear relationship between age and HRmax |
| 📈 **Regression Line** | `HRmax = -1.11 * Age + 208.625` |
| 🔍 **R² (Explained Variance)** | 0.167 — Only ~17% of variation in HRmax is explained by age |
| 🧪 **Hypothesis Test** | Slope is statistically significant (p ≈ 9.44e-10), allowing rejection of H₀ |
| ⚠️ **Limitations** | Non-normal residuals, unknown randomness of sampling, weak explanatory power |

---

## 🔬 Methods

1. **Preprocessing**
   - Filtered data for males only (`sex == 1`)
   - Checked for missing values (none found)
   - Selected variables: `age` and `thalachh` (HRmax)

2. **Visualizations**
   - Histograms for Age & HRmax
   - Scatterplots with least-squares regression line
   - Residual plots and Q-Q plot for normality checks

3. **Linear Regression**
   - Verified regression conditions: linearity, independence, equal variance
   - Regression model constructed: age as predictor, HRmax as response
   - Evaluated fit using R² and visual spread around regression line

4. **Hypothesis Testing**
   - H₀: Slope of age = 0 (no relationship)
   - HA: Slope of age < 0 (negative association)
   - t-score: -6.41, p-value < 0.05 → statistically significant

---

## 📦 Installation

You can run this project with the following dependencies:

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/Heart-Attack-Analysis-and-Prediction.git
cd Heart-Attack-Analysis-and-Prediction
```

### 2. Install Requirements
You likely have all required libraries, but to be safe:
```bash
pip install pandas matplotlib numpy
```

### 3. Launch Jupyter Notebook
```bash
jupyter notebook
```
Open the files:
- `Correlation and Regression Code.ipynb` (main analysis)
- `Statistical Inference Code.ipynb` (detailed testing)

---

## 💡 Use Cases

- 📚 Educational tool for teaching **statistical inference** and **regression modeling**
- 🩺 Baseline predictor for **cardiovascular screening** in public health settings
- 🧪 Reference for analyzing **real-world health data** with simple ML techniques

---

## 🧾 Attribution

- 📊 Dataset: [Kaggle - Heart Attack Analysis & Prediction Dataset](https://www.kaggle.com/rashikrahmanpritom/heart-attack-analysis-prediction-dataset)
- 🏥 Original source: Cleveland Clinic Foundation (via UCI ML Repository)
- ✍️ Report authored by Rachael Chew (Minerva University, CS51 - Formal Analyses)

---

## 🙋‍♀️ Want to Contribute?

Suggestions, corrections, or enhancements are welcome! Feel free to open a pull request or create an issue.
