# Well-Being Index Prediction
## Introduction

This project aims to predict the well-being index of different regions based on various socio-economic and demographic factors. The well-being index is an important measure that reflects the overall quality of life and happiness of the population.

## Table of Contents

- [Introduction](#introduction)
- [Project Overview](#project-overview)
- [Data Preparation](#data-preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Feature Selection](#feature-selection)
- [Modeling](#modeling)
- [Evaluation](#evaluation)
- [Conclusion](#conclusion)
- [Future Work](#future-work)
---
## Project Overview

1. **Data Collection and Cleaning**
2. **Exploratory Data Analysis**
3. **Feature Selection**
4. **Model Training and Evaluation**
5. **Conclusion and Future Work**
---
## Data Preparation

### Handling Missing Values and Duplicates

- Performed imputation for missing values and removed duplicates to ensure data quality.
---
### Correlation Analysis

- Features were selected based on their correlation with the well-being index and statistical significance. The rest of the features were excluded.

| Variable                                                                       | Correlation with Well-Being Index |
| ------------------------------------------------------------------------------- | ---------------------------------: |
| Old age dependency ratio (old age (65 and older) per 100 creatures (ages 15-64))|                            0.740961 |
| Intergalactic Development Index (IDI), Rank                                     |                           -0.705557 |
| Intergalactic Development Index (IDI)                                           |                            0.661725 |
| Education Index                                                                 |                            0.645374 |
| Young age (0-14) dependency ratio (per 100 creatures ages 15-64)                |                           -0.638891 |
| Mean years of education (galactic years)                                        |                            0.611781 |
| Expected years of education (galactic years)                                    |                            0.611651 |
| Income Index                                                                    |                            0.606666 |
| Existence expectancy at birth                                                   |                            0.587930 |
| Existence expectancy index                                                      |                            0.584568 |
| Life expectancy at birth, male (galactic years)                                 |                            0.580025 |
| Life expectancy at birth, female (galactic years)                               |                            0.575104 |

## Insights of Selected Features Based on The Correlation Analysis

Correlation analysis revealed significant insights into the determinants of well-being based on various socio-economic and demographic factors:

- **Old Age Dependency Ratio**
  - With a high positive correlation score of 0.740961, the old age dependency ratio indicates that as the proportion of older individuals relative to the working-age population increases, there is a strong positive impact on well-being. This suggests that societies with a higher proportion of elderly citizens tend to have higher levels of well-being, possibly due to factors such as better healthcare systems and social support for seniors.

- **Education Index, Mean Years of Education, and Expected Years of Education**
  - These variables all show strong positive correlations with well-being, ranging from 0.611651 to 0.645374. Higher levels of education are typically associated with improved health outcomes, higher income potential, and greater access to opportunities, all of which contribute to overall well-being.

- **Intergalactic Development Index (IDI) and IDI Rank**
  - The IDI itself has a positive correlation of 0.661725 with well-being, indicating that higher development levels are associated with greater well-being. In contrast, the IDI rank has a negative correlation of -0.705557, suggesting that lower-ranked galaxies, which are less developed, tend to have higher levels of well-being. This could be attributed to factors such as close-knit communities and simpler lifestyles fostering greater satisfaction and contentment.

- **Young Age Dependency Ratio**
  - The negative correlation score of -0.638891 suggests that as the proportion of young individuals relative to the working-age population increases, there is a negative impact on well-being. Higher youth dependency ratios may strain social services and resources, leading to lower well-being outcomes due to factors like inadequate education and healthcare provision for children.

- **Income Index**
  - With a positive correlation of 0.606666, the income index indicates that higher income levels are associated with greater well-being. Increased income provides individuals and families with greater access to resources and opportunities, leading to improved living standards and overall well-being.

- **Existence Expectancy at Birth and Existence Expectancy Index**
  - Both variables show positive correlations with well-being, indicating that higher life expectancies are associated with greater well-being. Longer life expectancies typically reflect better healthcare systems, higher standards of living, and overall better quality of life.

- **Life Expectancy at Birth (Male and Female)**
  - Similarly, both male and female life expectancies show positive correlations with well-being. Higher life expectancies for both genders indicate healthier populations and better overall well-being outcomes.

The insights from the correlation analysis guided the selection of features that significantly influence the well-being index prediction. These features were instrumental in training and evaluating the predictive models.

---

These insights provide a deeper understanding of how socio-economic and demographic factors contribute to the well-being index across different regions.


---
## Modeling

### Feature Scaling

- Normalized numerical features to ensure they are on a similar scale, preventing features with larger magnitudes from dominating the learning process.
  
### Model Training

Trained the following models to predict the well-being index:

- Random Forest
- Decision Tree
- Ridge Regression
- Linear Regression
- Lasso Regression

### Model Evaluation

The Root Mean Square Error (RMSE) scores for each model are as follows:

| Model              | RMSE   |
|---------------------|--------|
| Random Forest       | 0.025570 |
| Decision Tree       | 0.034923 |
| Ridge Regression    | 0.035895 |
| Linear Regression   | 0.035970 |
| Lasso Regression    | 0.053474 |

**Conclusion**: Based on RMSE alone, the Random Forest model outperforms all other models in predicting the well-being index.

## Conclusion

This project successfully predicted the well-being index using various socio-economic and demographic features. The Random Forest model demonstrated superior performance with the lowest RMSE.

## Future Work

- **Data Enrichment**: Include more features and data sources to improve model accuracy.
- **Model Improvement**: Explore advanced modeling techniques and hyperparameter tuning.
- **Real-Time Prediction**: Develop a web application for real-time prediction of the well-being index.
- **Ethical Considerations**: Ensure data privacy and ethical use of data in future applications.

---

Feel free to explore the project and contribute by opening issues or submitting pull requests. For any questions or discussions, please reach out via [contact information].

---
## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
# Author

`Rasmo Wanyama`

`Data Analyst/Data Scientist`

Let's connect on LinkedIn:
[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rasmo-/) 

---

**Disclaimer**: This project is for educational purposes only. The predictions and results are based on the given dataset and may not reflect real-world scenarios accurately.
