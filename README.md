---
---
---

# Moffitt Intern-project 2023

## DepMap Statistical Analysis and Machine Learning

-   **Goal 1:** Proficiency of pandas for handling and manipulating structured data.![](https://github.com/chingyaousf/Intern-project/blob/main/plots/22Q2_CRISPR_gene_dependency.csv.png?raw=true)![](https://github.com/chingyaousf/Intern-project/blob/main/plots/22Q2_CCLE_expression.csv.png?raw=true)![](https://github.com/chingyaousf/Intern-project/blob/main/plots/Dep_Exp_merged_data.png?raw=true)

-   **Goal 2:** Generate scatter plots correlating the CRISPR KO effect (CRISPR_gene_effct, CRISPR_gene_depency) vs Gene expression (CCLE_expression).

![](https://github.com/chingyaousf/Intern-project/blob/main/plots/A1BG(1)Eff_Exp.png?raw=true){width="300"}![](https://github.com/chingyaousf/Intern-project/blob/main/plots/A1BG(1)Dep_Exp.png?raw=true){width="300"}![](https://github.com/chingyaousf/Intern-project/blob/main/plots/A1CF(29974)Eff_Exp.png?raw=true){width="300"}![](https://github.com/chingyaousf/Intern-project/blob/main/plots/A1CF(29974)Dep_Exp.png?raw=true){width="300"}

-   **Goal 3:** Systematically screen for the relationship between CRISPR_gene_depency(Dep) vs Gene_expression(Exp) in CCLE.![](https://github.com/chingyaousf/Intern-project/blob/main/plots/intern_SpearmanCorrelation_pipeline.png?raw=true)

1.  *(Generate Spearman* *correlation matrix between CRISPR_gene_dependency(Dep) and Gene_expression(Exp)).*![](https://github.com/chingyaousf/Intern-project/blob/main/plots/Dep_Exp_correlation_table.png?raw=true)

2.  *(Compare diagonal values with non-diagonal values of correlation matrix (such as value of A1BG (1) Dep vs. A1BG (1) Exp with the rest of values of matrix)).*![](https://github.com/chingyaousf/Intern-project/blob/main/plots/violin_boxplot_histogram.png?raw=true)

3.  *(Perform the Wilcoxon test between diagonal and non-diagonal values).*

    Wilcoxon_test_diaonal_nondiagonal_02.txt;

    `Average Wilcoxon test statistic: 66641376.968`

    `Average Wilcoxon test p-value: 2.1638665163031885e-20`

-   **Goal 4:** Develop several machine learning models to identify gene expression predictive of the CRISPR_gene_depency.**![](https://github.com/chingyaousf/Intern-project/blob/main/plots/intern_ML_pipeline.png?raw=true)RF Model:**

    ![](https://github.com/chingyaousf/Intern-project-2023/blob/main/plots/RF_scatterplots_correlation_positive_negative_01.jpg?raw=true)

**Blog:**

<https://ssidmarine.wordpress.com/>

**Access data:**

DepMap Public 22Q2 Primary Files

<https://depmap.org/portal/download/all/>

22Q2 CRISPR_gene_effect

CRISPR_gene_dependency.csv

CCLE_expression.csv

**testing data available in the data folder**
