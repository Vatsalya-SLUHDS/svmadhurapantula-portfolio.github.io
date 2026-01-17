
# Gastric Cancer: Biomarker Association & Incidence Mapping
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](YOUR_COLAB_LINK_HERE)

## 📌 Project Overview
This research-driven project explores the clinical biomarkers of Gastric Cancer and maps them against regional incidence rates in Missouri. By integrating clinical patient data with public health statistics, the analysis aims to identify key risk factors and correlations that inform early diagnosis and personalized treatment strategies.

## Links to the datasets
* Dataset 1 (gastric_cancer): https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/AC79EP
* Dataset 2 (incidence_mo): https://statecancerprofiles.cancer.gov/incidencerates/index.php?stateFIPS=29&areatype=county&age=001&cancer=018&stage=999&race=00&sex=0&year=0&type=incd&sortVariableName=count&sortOrder=desc
These two datasets are in two different formats (excel and csv).
This topic is choosen with an intention of identifying biomarker for the disease and find associations between various factors related to the disease.

## 📊 Key Insights
* **Biomarker Synergy:** Discovered a high Spearman correlation between **CEA** and **CA19-9**, identifying them as a potent dual-marker cluster for screening.
* **Survival Determinants:** Quantitative analysis confirmed a negative linear trend between age and survival time, with a median survival of 27 months.
* **Clinical Indicators:** Engineered new features for **Diabetes** and **Anemia**, finding that pre-operative anemia is a significant factor in prognosis.

## 🛠️ Technical Stack
* **Language:** Python 3.10
* **Libraries:** Pandas (Data Wrangling), Seaborn/Matplotlib (Visualization), NumPy (Numerical Analysis).
* **Data Sources:** Harvard Dataverse (Clinical) & National Cancer Institute (Incidence Rates).

## 🗂️ Analysis Workflow
1.  **ETL & Cleaning:** Handled missing values via mean imputation and handled data type conversions for medical staging (TNM).
2.  **Feature Engineering:** Created clinical logic to identify Diabetic and Anemic status based on Glucose and Hemoglobin thresholds.
3.  **Statistical Mapping:** Performed hierarchical clustering (Clustermaps) to identify patterns in tumor markers (AFP, CEA, Ca125).
4.  **Survival Analysis:** Developed Kaplan-Meier curves and regression plots to visualize survival trajectories.

## 📈 Visual Highlights
*(Tip: Export your best plot as a PNG and upload it here)*
![Age vs Survival](visuals/age_survival_plot.png)

## 🏁 Conclusion
The study reinforces the importance of multi-marker panels over single-marker screening. Identifying these associations supports the move toward personalized medicine and more accurate drug development targets.
