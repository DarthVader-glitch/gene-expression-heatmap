# gene-expression-heatmap
Python-based bioinformatics project for visualizing gene expression patterns using clustered heatmaps generated from tumor and normal sample datasets.

## Overview
The project demonstrates how computational biology techniques can be used to analyze and visualize differences between normal and tumor samples using gene expression profiles.

# What is Gene Expression Data?

Gene expression data represents the activity level of genes inside biological samples.

In this project:

- Rows represent genes
- Columns represent biological samples
- Numerical values represent expression levels

Higher values indicate higher gene activity.

The dataset contains:
- Normal tissue samples
- Tumor tissue samples

This type of analysis is commonly used in:
- Cancer research
- Transcriptomics
- Genomics
- Precision medicine

# Understanding the CSV Dataset

The file:

```text
fake_gene_expression_data.csv
```

contains simulated gene expression values.

## Dataset Structure

| Column | Description |
|--------|-------------|
| First Column | Gene names |
| Remaining Columns | Expression values for each sample |

Example:

| Gene | Sample1 | Sample2 |
|------|----------|----------|
| Gene1 | 12 | 45 |
| Gene2 | 8 | 31 |

# What is a Heatmap?

A heatmap is a graphical representation of numerical data where colors represent value intensity.

In this project:
- Dark colors represent lower expression
- Bright colors represent higher expression

The heatmap helps identify:
- Similar gene behavior
- Clustering patterns
- Tumor vs normal sample differences

# Hierarchical Clustering

The project uses hierarchical clustering through Seaborn's `clustermap()` function.

This automatically groups:
- Similar genes together
- Similar samples together

The dendrograms visible in the heatmap represent these clustering relationships.

# Output

The program generates:

```text
GeneHeatmap.pdf
```

containing the clustered heatmap visualization.

# Applications

This project demonstrates concepts used in:
- Bioinformatics
- Computational Biology
- Gene Expression Analysis
- Cancer Informatics
- Data Visualization

# Future Improvements

Possible future enhancements:
- Use real RNA-seq datasets
- Add data normalization
- Interactive heatmaps
- Differential expression analysis
- PCA visualization
- Jupyter Notebook support
