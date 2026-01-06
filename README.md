
# Spatio-Temporal Analysis of PM2.5 and Respiratory Health in Scotland

This repository contains the **full reproducible Python analysis code** used in the MSc Data Science dissertation titled:

**“Spatio-Temporal Modelling of Air Pollution Exposure and Respiratory Diseases in Scotland: A Data-Driven Case Study.”**

The code reproduces all tables, figures, spatial analyses, and predictive models reported in the dissertation and its appendices.

---

## 📂 Repository Contents

- `Appendix_Dissertation_Analysis.py`  
  Complete Python script converted from the Jupyter Notebook used in the dissertation.

- `Scotland_PM25_Respiratory_Analysis.ipynb`  
  Original Jupyter Notebook containing step-by-step analysis.

- `outputs/`
  - `tables/` – Generated CSV tables for dissertation appendices  
  - `figures/` – Generated figures (histograms, scatter plots, hotspot maps, model diagnostics)

- `requirements.txt`  
  Python dependencies required to run the analysis.

---

## 📊 Analyses Covered

### Descriptive & Exploratory Analysis
- Mean PM2.5 by Local Authority  
- Respiratory rate distributions by age group and sex  
- Histograms and boxplots of PM2.5 and respiratory rates  

### Spatial Analysis
- Global Moran’s I  
- Local Indicators of Spatial Association (LISA)  
- Getis–Ord Gi* Hotspot Z-score maps for PM2.5 and respiratory rates  

### Predictive Modelling
- Linear Regression (Observed vs Predicted log rates)
- Random Forest Regression
- Model performance metrics and residual diagnostics
- Random Forest feature importance and dominant predictors

---

## ⚙️ How to Run the Code

### 1️⃣ Install Required Packages
```bash
pip install -r requirements.txt
```

### 2️⃣ Set Data Path
The analysis expects the merged dataset CSV.

Default path used in the script:
```text
C:\Users\Lenovo\Merged_file_pollution25 original data.csv
```

You may update the `DATA_PATH` variable in the script or set an environment variable:

**Windows (PowerShell):**
```powershell
setx DISSERTATION_DATA "C:\path\to\Merged_file_pollution25 original data.csv"
```

### 3️⃣ Run the Script
```bash
python Appendix_Dissertation_Analysis.py
```

All tables and figures will be generated automatically in the `outputs/` folder.

---

## 🔁 Reproducibility
- Fixed random seeds for models
- Standalone plotting scripts
- Clear separation of data loading, analysis, and output generation

---

## 🎓 Academic Use
This repository is provided for dissertation examination, reproducibility, and academic reference.

Please cite appropriately if reused.

---

## 👤 Author
**Julius Adebayo John**  
MSc Data Science, University of East London

---

## 📜 License
Shared for academic and non-commercial use.
