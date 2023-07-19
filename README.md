# Moffitt Intern-project 2023

## DepMap Statistical Analysis and Machine Learning

## Project Overview:

The emergence of advanced genetic technologies, notably CRISPR (Clustered Regularly Interspaced Short Palindromic Repeats), has revolutionized genetic research and its applications. This project focuses on investigating the interplay between CRISPR gene dependency and CCLE gene expression, aiming to uncover meaningful relationships between them. CRISPR gene dependency measures the impact of gene knockout, providing insights into gene essentiality within cellular contexts. CCLE gene expression, on the other hand, quantifies gene expression levels across cell lines, offering valuable transcriptional insights. The primary objective is to develop powerful machine learning models capable of predicting CRISPR gene dependency based on gene expression patterns. Through statistical analysis, correlation matrices, and feature engineering techniques, this project aims to enhance our understanding of the underlying mechanisms, potentially leading to more precise genetic interventions and advancements in drug discovery, personalized medicine, and therapeutic development.

### Goal 1: Proficiency of pandas for handling and manipulating structured data.

#### ![](https://github.com/chingyaousf/Intern-project/blob/main/plots/22Q2_CRISPR_gene_dependency.csv.png?raw=true)![](https://github.com/chingyaousf/Intern-project/blob/main/plots/22Q2_CCLE_expression.csv.png?raw=true)![](https://github.com/chingyaousf/Intern-project/blob/main/plots/Dep_Exp_merged_data.png?raw=true)

### **Goal 2:** Generate scatter plots correlating the CRISPR KO effect (CRISPR_gene_effct, CRISPR_gene_depency) vs Gene expression (CCLE_expression).![](https://github.com/chingyaousf/Intern-project-2023/blob/main/plots/EIF2AK3_9451_MYC_4609Dep_Exp.jpg?raw=true)

![](https://github.com/chingyaousf/Intern-project-2023/blob/main/plots/NQO1_1728_SF3B1_23451_SQSTM1_8878Dep_Exp.jpg?raw=true)

### **Goal 3:** Systematically screen for the relationship between CRISPR_gene_depency(Dep) vs Gene_expression(Exp) in CCLE.

#### ![](https://github.com/chingyaousf/Intern-project-2023/blob/main/plots/intern_SpearmanCorrelation_pipeline_02.png?raw=true)

1.  *(Generate Spearman* *correlation matrix between CRISPR_gene_dependency(Dep) and Gene_expression(Exp) by HPC ).*![](https://github.com/chingyaousf/Intern-project/blob/main/plots/Dep_Exp_correlation_table.png?raw=true)

2.  *(Compare diagonal values with non-diagonal values of correlation matrix (such as value of A1BG (1) Dep vs. A1BG (1) Exp with the rest of values of matrix) by HPC ).*![](https://github.com/chingyaousf/Intern-project/blob/main/plots/violin_boxplot_histogram.png?raw=true)

3.  *(Perform the Wilcoxon test between diagonal and non-diagonal values by HPC).*

    Wilcoxon_test_diaonal_nondiagonal_02.txt;

    `Average Wilcoxon test statistic: 66641376.968`

    `Average Wilcoxon test p-value: 2.1638665163031885e-20`

### **Goal 4:** Develop several machine learning models to identify gene expression predictive of the CRISPR_gene_depency.**![](https://github.com/chingyaousf/Intern-project/blob/main/plots/intern_ML_pipeline.png?raw=true)**

### **RF, NNW, and KNN models were compared using five target genes:**

**EIF2AK3 (9451) Dep**![EIF2AK3 (9451) Dep](https://github.com/chingyaousf/Intern-project-2023/blob/main/plots/EIF2AK3_all_models.jpg?raw=true)

**MYC (4609) Dep**![](https://github.com/chingyaousf/Intern-project-2023/blob/main/plots/MYC_all_models.jpg?raw=true)

**NQO1 (1728) Dep**![](https://github.com/chingyaousf/Intern-project-2023/blob/main/plots/NQO1_all_models.jpg?raw=true)

**SF3B1 (23451) Dep**![](https://github.com/chingyaousf/Intern-project-2023/blob/main/plots/SQSTM1_all_models.jpg?raw=true)

**SQSTM1 (8878) Dep**![](https://github.com/chingyaousf/Intern-project-2023/blob/main/plots/SQSTM1_all_models.jpg?raw=true)

### **Prediction error values were compared among RF, NNW, and KNN models using five target genes:**

![](https://github.com/chingyaousf/Intern-project-2023/blob/main/plots/RF_5Genes_by_Features_Filtering.png?raw=true)

![](https://github.com/chingyaousf/Intern-project-2023/blob/main/plots/NNW_5Genes_by_Features_Filtering.png?raw=true)

![](https://github.com/chingyaousf/Intern-project-2023/blob/main/plots/KNN_5Genes_by_Features_Filtering.png?raw=true)

![](https://github.com/chingyaousf/Intern-project-2023/blob/main/plots/MSE_all_Genes.png?raw=true)

![](https://github.com/chingyaousf/Intern-project-2023/blob/main/plots/MAE_all_Genes.png?raw=true)

![](https://github.com/chingyaousf/Intern-project-2023/blob/main/plots/R2_all_Genes.png?raw=true)

### Summary:

The correlation matrix and Wilcoxon test were conducted to examine the relationship between CRISPR gene dependency and gene expression. The RF, NNW, and KNN models were evaluated based on their prediction accuracy for different genes. MYC and SQSTM1 showed higher prediction accuracy in all models, while EIF2AK3, NQO1, and SF3B1 exhibited lower accuracy, indicating a more complex relationship. R2 values indicated moderate prediction accuracy for MYC and SQSTM1. Non-linear regression approaches may be more suitable for certain genes. Further research and advanced modeling techniques like K-means clustering and Non-Negative Matrix Factorization are needed to improve prediction accuracy and understand the complex relationships between gene expression and CRISPR gene dependency. Alternative evaluation metrics, such as RMSE and MAPE, should also be considered for genes with non-linear relationships.

## Blog:

<https://ssidmarine.wordpress.com/2023/06/27/intern-project-introduction/>

## Access data:

DepMap Public 22Q2 Primary Files

<https://depmap.org/portal/download/all/>

22Q2 CRISPR_gene_effect

CRISPR_gene_dependency.csv

CCLE_expression.csv

**testing data available in the data folder**
