[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/12v1M7eNUXDem2RFR0TIsBe-NBgKjlny4?usp=sharing)

# Volcano Plot for Gene Expression Analysis
##### by [Mo Shakiba](https://github.com/moneuron)

This repository contains a Jupyeter Notebook that generates a **Volcano Plot** for visualizing differential gene expression data, typically from RNA-Seq or microarray experiments.

## Features

- **User Inputs**: Upload your GEO `.tsv` file and provide gene names of interest, p-value threshold, log fold change (logFC) threshold, plot size, and custom colors.
- **Aggregation**: The code aggregates data for genes of interest by computing mean logFC and the minimum p-value across replicates.
- **Gene Annotation**: Automatically annotates genes of interest in the plot.
- **Customization**: Customize plot size and color scheme for better presentation and clarity.

## Usage

1. **Upload your GEO `.tsv` file**: Provide your data file to the notebook. The file should contain gene names, logFC, and p-values for each gene.
   
2. **Adjust parameters**: Customize the p-value threshold, log fold change threshold, plot dimensions, and colors using the interactive input form in the notebook.
   
3. **Generate Volcano Plot**: The notebook will plot the volcano plot and automatically label genes of interest with non-overlapping text.

### Example

```python
pval_threshold = 0.05
logfc_threshold = 0
genes_of_interest_input = "MMP2, MMP7, MMP15"
plot_width = 12
plot_height = 10
upregulated_color = "crimson"
downregulated_color = "navy"
non_significant_color = "gray"
```

4. **View Results**: The notebook will print a list of upregulated, downregulated, and non-significant genes of interest and display the volcano plot.
