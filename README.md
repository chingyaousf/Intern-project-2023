---
---
---

# Moffitt Intern-project 2023

## DepMap Statistical Analysis and Machine Learning

-   **Goal 1:** Proficiency of pandas for handling and manipulating structured data.![](https://github.com/chingyaousf/Intern-project/blob/main/plots/22Q2_CRISPR_gene_dependency.csv.png?raw=true)![](https://github.com/chingyaousf/Intern-project/blob/main/plots/22Q2_CCLE_expression.csv.png?raw=true)![](https://github.com/chingyaousf/Intern-project/blob/main/plots/Dep_Exp_merged_data.png?raw=true)

-   **Goal 2:** Generate scatter plots correlating the CRISPR KO effect (CRISPR_gene_effct, CRISPR_gene_depency) vs Gene expression (CCLE_expression).

-   ![](https://github.com/chingyaousf/Intern-project/blob/main/plots/A1BG(1)Eff_Exp.png?raw=true){width="100"}![](https://github.com/chingyaousf/Intern-project/blob/main/plots/A1BG(1)Dep_Exp.png?raw=true){width="100"}![](https://github.com/chingyaousf/Intern-project/blob/main/plots/A1CF(29974)Eff_Exp.png?raw=true){width="100"}![](https://github.com/chingyaousf/Intern-project/blob/main/plots/A1CF(29974)Dep_Exp.png?raw=true){width="100"}

-   **Goal 3:** Systematically screen for the relationship between CRISPR_gene_depency(Dep) vs Gene_expression(Exp) in CCLE.

1.  *(Generate correlation matrix between CRISPR_gene_dependency(Dep) and Gene_expression(Exp)).*![](https://github.com/chingyaousf/Intern-project/blob/main/plots/Dep_Exp_correlation_table.png?raw=true)

2.  *(Compare diagonal values with non-diagonal values of correlation matrix (such as value of A1BG (1) Dep vs. A1BG (1) Exp with the rest of values of matrix)).*![](https://github.com/chingyaousf/Intern-project/blob/main/plots/violin_boxplot_histogram.png?raw=true)

-   **Goal 4:** Develop several machine learning model to identify gene expression predictive of the CRISPR_gene_depency.![](https://github.com/chingyaousf/Intern-project/blob/main/plots/intern_ML_pipeline.png?raw=true)

**Blog:**

<https://ssidmarine.wordpress.com/>

**Access data:**

DepMap Public 22Q2 Primary Files

<https://depmap.org/portal/download/all/>

22Q2 CRISPR_gene_effect

CRISPR_gene_dependency.csv

CCLE_expression.csv

**testing data available in the data folder**
