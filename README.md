 SCRNA-assignment-
Pre-processing of 10X data, scRNA-seq tutorial, and AnnData analysis 10X Preprocessing

Steps Performed:

* Loaded 10X dataset
* Quality control performed
* Filtered low-quality cells
* Normalized data

Output:
Screenshots of preprocesing steps are attached.


 1. Load Data

Explanation:
This step loads the 10x Genomics single-cell RNA sequencing dataset into Scanpy as an AnnData object, which stores gene expression data along with cell and gene annotations.



2. Quality Control (QC)

Explanation:
This step filters low-quality cells and genes to remove noise from the dataset, ensuring only reliable cells are used for downstream analysis.



 3. Normalize Data

Explanation:
Gene expression values are normalized to make cells comparable by removing differences caused by sequencing depth.



4. Find Highly Variable Genes

Explanation:
This step selects the most informative genes that show strong variation across cells, which helps improve clustering and visualization.



 5. PCA (Dimensionality Reduction)

Explanation:
Principal Component Analysis reduces the dataset dimensions while keeping the most important variation in the data.


6. Compute Neighbors

Explanation:
A nearest-neighbor graph is built to group similar cells based on their gene expression profiles.



 7. UMAP

Explanation:
UMAP is used to visualize high-dimensional single-cell data in 2D space while preserving cell relationships.


 8. Leiden Clustering

**Explanation:**
Cells are grouped into clusters based on similarity in gene expression to identify potential cell types.


 9. UMAP Plot

Explanation:
The final visualization shows how cells are grouped into clusters in 2D space for interpretation.

