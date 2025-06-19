# 📈 Statistical Comparison of Evaluation Metrics in Credit Risk Research

This repository contains a statistical analysis of five widely used evaluation metrics for credit risk model performance. The analysis does **not use raw datasets**, but is based on a **summarized metric value table** created from experimental results reported across multiple published research papers.  

We apply the **Friedman test** followed by **post-hoc Conover analysis** to determine if metric-based model rankings differ significantly across various experimental conditions.

---

## Objective

To assess whether the choice of evaluation metric significantly affects model ranking outcomes in credit risk studies, using statistical evidence from a synthesized metric summary table.

---

## Metrics Compared

- **AUC ROC**  
- **Matthews Correlation Coefficient (MCC)**  
- **Precision**  
- **Brier Score**  
- **Cost-Efficient Accuracy (%)** (based on domain-specific cost assumptions: FN = 5× FP)

---

## Methodology Overview

1. **Data Source**  
   Metric values were curated and summarized from multiple academic studies involving credit risk models.

2. **Friedman Test**  
   A non-parametric test used to detect statistically significant differences in metric rankings across models and conditions.

3. **Post-Hoc Analysis**  
   Pairwise comparisons using **Conover’s post-hoc test** to identify which metric pairs differ significantly.

4. **Visualizations**  
   - Mean metric rankings  
   - P-value heatmaps for pairwise comparisons  
   - Interpretation of metric consistency and significance

---

## Outputs

- Friedman chi-square test statistic and p-value  
- Full post-hoc comparison table  
- Visual metric ranking and comparison heatmaps

---

## File Structure
├── Metric_Analysis.ipynb # Jupyter Notebook with full analysis  
├── README.md # This file


> 📌 Note: No raw datasets are used. All input is based on a manually created metric summary table grounded in published research.

---

## 📦 Dependencies

```bash
pip install pandas numpy scipy seaborn matplotlib scikit-posthocs
```

The notebook can be executed in Google Colab or a Jupyter environment.

## Use Case
This project is ideal for:  
Researchers comparing evaluation metrics for classification models  
Credit scoring practitioners selecting appropriate model comparison criteria  
Statisticians performing non-parametric ranking comparisons  

## Future Scope
Include additional domain metrics like F1-score, specificity, or Sharpe ratio  
Extend to regression-based credit scoring settings  
Analyze metric sensitivity under different cost configurations  
