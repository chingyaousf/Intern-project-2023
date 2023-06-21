# Moffitt Intern-project 2023

## DepMap Statistical Analysis and Machine Learning

-   **Goal 1:** Proficiency of pandas for handling and manipulating structured data.![](22Q2%20CRISPR_gene_dependency.csv.png)![](22Q2%20CCLE_expression.csv.png)![](Dep_Exp%20merged_data.png)

-   **Goal 2:** Generate scatter plots correlating the CRISPR KO effect (CRISPR_gene_effct, CRISPR_gene_depency) vs Gene expression (CCLE_expression).![](A1BG%20(1)%20Eff_Exp.png)![](A1CF%20(29974)%20Eff_Exp.png)![](A1BG%20(1)%20Dep_Exp.png)![](A1CF%20(29974)%20Dep_Exp.png)

-   **Goal 3:** Systematically screen for the relationship between CRISPR_gene_depency(Dep) vs Gene_expression(Exp) in CCLE.

1.  *(Generate correlation matrix between CRISPR_gene_dependency(Dep) and Gene_expression(Exp)).*![](Dep_Exp%20correlation_table.png)

2.  *(Compare diagonal values with non-diagonal values of correlation matrix (such as value of A1BG (1) Dep vs. A1BG (1) Exp with the rest of values of matrix)).*![](data_analysis%20batch%20scripts/intern_plots/boxplot_02.png)

    ![](data_analysis%20batch%20scripts/intern_plots/violin_plot_02.png)

-   **Goal 4:** Develop several machine learning model to identify gene expression predictive of the CRISPR_gene_depency.[![](https://github.com/chingyaousf/Intern-project/blob/main/plots/intern%2520ML%2520pipeline.png)](https://github.com/chingyaousf/Intern-project/blob/main/plots/intern%20ML%20pipeline.png)

**Blog:**

<https://ssidmarine.wordpress.com/>

**Access data:**

DepMap Public 22Q2 Primary Files

<https://depmap.org/portal/download/all/>

22Q2 CRISPR_gene_effect

CRISPR_gene_dependency.csv

CCLE_expression.csv

**testing data available in the data folder**
