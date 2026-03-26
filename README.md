# diabetes_random_forest_tutorial
Interactive tutorial exploring Random Forest classification with focus on n_estimators hyperparameter optimization. Uses UCI Diabetes Dataset to demonstrate ensemble learning, achieving 85.9% accuracy with 100 trees. Includes complete Python code, visualizations, and analysis of the "wisdom of crowds" effect in machine learning.

# Random Forest Diabetes Prediction Tutorial

## Overview
This repository contains a comprehensive tutorial on Random Forest classification, focusing on the `n_estimators` hyperparameter and its impact on model performance. The tutorial uses the CDC Diabetes Health Indicators Dataset to demonstrate ensemble learning principles.

## Repository Contents
- `Diabetic_RF.ipynb` - Complete Jupyter notebook with all code and analysis
- `README.md` - This file
- `LICENSE` - MIT License
- `/images` - Contains all visualization plots:
  - `wisdom_of_crowds_plot.png` - Training vs testing accuracy across different tree counts
  - `confusion_matrix.png` - Final model confusion matrix
  - `feature_importance.png` - Top 10 most important features
  - `roc_curve.png` - ROC curve with AUC score

## Tutorial Focus

**Main Question:** How many trees are necessary to build an effective Random Forest?

**Key Findings:**
- Single decision trees overfit severely (12% accuracy gap)
- Ensemble learning reduces overfitting significantly
- ~100 trees provide optimal performance
- Beyond 100 trees shows diminishing returns
- BMI and Age identified as most important predictors

## Dataset

| Property | Details |
|----------|---------|
| **Source** | UCI Machine Learning Repository |
| **Dataset ID** | 891 |
| **Name** | CDC Diabetes Health Indicators Dataset |
| **Records** | 253,680 patient records |
| **Features** | 21 health and demographic indicators |
| **Target** | Binary classification (Diabetes/No Diabetes) |

## Requirements

```text
Python 3.12+
scikit-learn 1.5.0
pandas 2.2.2
matplotlib 3.10.0
numpy 2.0.2
seaborn (latest)
ucimlrepo 0.0.7
```

## Installation

```bash
git clone https://github.com/[your-username]/diabetes-random-forest-tutorial
cd diabetes-random-forest-tutorial
pip install -r requirements.txt
```

## Usage

```bash
jupyter notebook Diabetic_RF.ipynb
```

Run all cells to reproduce the analysis and generate visualizations.

## Results

**Final Model (n_estimators=100):**
- **Accuracy:** 85.94%
- **ROC AUC:** 0.7948
- **Training Records:** 202,944
- **Testing Records:** 50,736

## Key Concepts Covered

- Bootstrap sampling and bagging
- Ensemble learning principles
- Hyperparameter tuning (n_estimators)
- Feature importance analysis
- Model evaluation (ROC curves, confusion matrices)
- Overfitting vs generalization

## Accessibility

All visualizations use colorblind-friendly palettes to ensure accessibility for users with color vision deficiencies.

## Ethical Considerations

This tutorial addresses:
- Fairness in healthcare ML models
- Transparency and interpretability
- Privacy concerns with patient data
- Appropriate use of predictive models in clinical settings

## License

MIT License - See LICENSE file for details

## Author

[Your Name]  
MSc Cybersecurity/Data Science Student  
University of Hertfordshire

## Acknowledgments

- UCI Machine Learning Repository for providing the dataset
- Scikit-learn developers for the excellent ML library
- Original Random Forest paper by Leo Breiman (2001)

## References

1. Breiman, L. (2001). Random Forests. Machine Learning, 45(1), 5-32.
2. Kelly, M., et al. CDC Diabetes Health Indicators Dataset. UCI ML Repository.
3. Pedregosa, F., et al. (2011). Scikit-learn: Machine Learning in Python. JMLR, 12, 2825-2830.

## Contributing

This is an educational project. Feel free to fork and adapt for your own learning purposes.

## Contact

For questions or feedback: [your-email@example.com]

---

**Note:** This tutorial was created as part of a Neural Networks and Machine Learning course assignment (March 2026).
