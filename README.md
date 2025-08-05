# Student Score Prediction 📚

> **Note**  
> A comprehensive machine learning project that predicts student exam scores based on various performance factors using multiple regression models.

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)](https://python.org)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.0%2B-orange?logo=scikit-learn&logoColor=white)](https://scikit-learn.org)
[![pandas](https://img.shields.io/badge/pandas-1.3%2B-green?logo=pandas&logoColor=white)](https://pandas.pydata.org)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## Results Summary

> **Warning**  
> **Best Model**: Ridge Regression achieves **77.1% accuracy** (R² = 0.7709) with RMSE of 1.80 points

| Model | Test R² | RMSE | Cross-Val R² |
|-------|---------|------|--------------|
| **Ridge Regression** ⭐ | **77.1%** | **1.80** | **72.4%** |
| Linear Regression | 77.1% | 1.80 | 72.4% |
| Polynomial (degree=2) | 76.0% | 1.84 | 70.5% |
| Random Forest | 66.6% | 2.17 | 62.4% |
| Lasso Regression | 61.8% | 2.32 | 56.5% |

## Dataset Overview
**6,607 student records** with 20 features analyzing academic performance predictors.

### Feature Categories

#### Study-Related Factors
- Hours_Studied
- Attendance  
- Previous_Scores
- Tutoring_Sessions

#### Personal Factors
- Sleep_Hours
- Motivation_Level
- Physical_Activity
- Learning_Disabilities

#### Environmental Factors
- Parental_Involvement
- Access_to_Resources
- Teacher_Quality
- Family_Income

#### Demographics & Social
- Gender, School_Type, Distance_from_Home
- Peer_Influence, Extracurricular_Activities, Internet_Access

## Key Findings

### Top 5 Predictors of Academic Success

> **Important**  
> These factors show the strongest correlation with exam scores:

1. **Attendance** (`0.581` correlation) 🎯
2. **Hours_Studied** (`0.445` correlation) 📖
3. **Previous_Scores** (`0.175` correlation) 📊
4. **Access_to_Resources** (`0.170` correlation) 💻
5. **Parental_Involvement** (`0.157` correlation) 👨‍👩‍👧‍👦

### Model Insights

#### Linear Regression Feature Importance (Top 5)
1. Access_to_Resources: `1.0483`
2. Parental_Involvement: `1.0052`
3. Internet_Access: `0.9558`
4. Learning_Disabilities: `-0.8540` (negative impact)
5. Extracurricular_Activities: `0.5777`

#### Random Forest Feature Ranking
1. Attendance: `37.96%` importance
2. Hours_Studied: `24.02%` importance
3. Previous_Scores: `8.66%` importance
4. Tutoring_Sessions: `3.49%` importance
5. Parental_Involvement: `3.38%` importance

## Installation

### Prerequisites
```bash
Python 3.8+
```

### Quick Start
```bash
# Clone repository
git clone https://github.com/habiba-226/student-score-prediction.git
cd student-score-prediction

# Install dependencies
pip install -r requirements.txt

# Run analysis
python student_score_prediction.py
```

### Dependencies
```txt
pandas>=1.3.0
numpy>=1.21.0
scikit-learn>=1.0.0
matplotlib>=3.4.0
seaborn>=0.11.0
```

## Visualizations Generated

> **Tip**  
> The analysis produces comprehensive visualizations:

- **Correlation Heatmap** - Feature relationships
- **Feature Importance Charts** - Key predictors identification
- **Model Comparison Plots** - Performance across algorithms
- **Residual Analysis** - Model validation
- **Actual vs Predicted Plots** - Prediction accuracy visualization

## Educational Insights

### What Drives Academic Success? 🎓

> **Important**  
> **Attendance is the #1 factor** - Students with higher attendance rates consistently achieve better exam scores.

### Key Takeaways:
- **Study Time Quality > Quantity**: Hours studied matters, but attendance has stronger impact
- **Resources Matter**: Access to educational materials significantly affects outcomes
- **Family Support**: Parental involvement shows measurable positive correlation
- **Tutoring Works**: External academic support provides clear benefits

### Surprising Findings:
- Sleep hours have minimal correlation (`-0.017`) with exam performance
- Gender shows negligible impact (`-0.002`) on academic outcomes
- School type (Public vs Private) has minimal influence (`0.009`)

## Model Performance Analysis

### Why Ridge Regression Won? 

> **Note**  
> Ridge Regression outperformed other models by effectively handling multicollinearity while maintaining simplicity.

**Advantages:**
- ✅ Handles correlated features well
- ✅ Prevents overfitting through L2 regularization
- ✅ Maintains interpretability
- ✅ Stable cross-validation performance

**Random Forest Limitations:**
- ⚠️ Overfitting on training data (94.85% vs 66.61% test)
- ⚠️ Higher complexity with marginal benefit
- ⚠️ Less interpretable feature relationships

## Contributing

> **Warning**  
> Please ensure all contributions include proper testing and documentation.

1. Fork the repository
2. Create feature branch (`git checkout -b feature/improvement`)
3. Commit changes (`git commit -am 'Add improvement'`)
4. Push to branch (`git push origin feature/improvement`)
5. Create Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

> **Note**  
> Dataset source: [Student Performance Factors - Kaggle](https://www.kaggle.com/datasets/lainguyn123/student-performance-factors)

- Original dataset contributors
- Scikit-learn community for ML algorithms
- Educational research community for insights validation

---
