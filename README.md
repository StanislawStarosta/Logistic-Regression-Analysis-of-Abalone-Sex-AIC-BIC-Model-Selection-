# Logistic Regression Analysis of Abalone Sex (AIC & BIC Model Selection)

## 📌 Project Description

The goal of this project is to analyze the relationship between physical characteristics of abalone and their sex using logistic regression.

Model selection was performed using:
- AIC (Akaike Information Criterion)  
- BIC (Bayesian Information Criterion)

The analysis was carried out in **R** using **R Markdown**.

---

## 📂 Project Structure

```
├── data/
│   ├── abalone.data
│   └── abalone.names
│
├── images/
│   ├── 3d_plot_1.png
│   ├── 3d_plot_2.png
│   ├── 3d_plot_3.png
│   └── 3d_plot_4.png
│
├── analysis/
│   ├── projekt_GLM.Rmd
│   └── projekt_GLM.pdf
│
└── README.md
```

---

## ⚙️ Methods Used

- logistic regression  
- model selection (AIC, BIC)  
- odds ratio interpretation  
- data visualization  

---

## 📊 Variables Description

The dataset consists of both quantitative and categorical variables.

### Quantitative Variables

The following variables are numerical:

- Length  
- Diameter  
- Height  
- WholeWeight  
- ShuckedWeight  
- VisceraWeight  
- ShellWeight  
- Rings  

Based on summary statistics, these variables differ substantially in their ranges. For instance, weight-related variables such as *WholeWeight* and *ShellWeight* exhibit relatively low minimum values and wide interquartile ranges, indicating high variability in specimen sizes.

This variability may suggest the need for:
- data transformation (e.g., logarithmic scaling), or  
- more careful handling of potential outliers  

prior to model fitting.

---

### Categorical Variable

- **Sex** — a factor variable with three levels:
  - "M" — Male  
  - "F" — Female  
  - "I" — Infant  

This variable serves as the response variable in the classification task.

---

## ▶️ How to Run the Project

1. Clone the repository:
```
git clone https://github.com/your-username/your-repo.git
```

2. Open the `.Rmd` file in RStudio  

3. Knit the report:  
```
Knit → PDF
```

---

## 📎 Repository Contents

- `.Rmd` file – full analysis code  
- `.pdf` file – final report  
- dataset files  
- images used in the analysis  

---

## 📈 Key Findings

The most influential variables affecting the probability of being male are:
- Diameter  
- ShuckedWeight  
- VisceraWeight  

These variables significantly impact the odds ratios in the logistic regression model.

---

## 🧠 Author

Project created as part of a study.
