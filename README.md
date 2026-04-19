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
<img width="1600" height="853" alt="IMG-20260417-WA0004" src="https://github.com/user-attachments/assets/1709353e-b64d-4030-ad64-69da24c60366" />



2. Quality Control (QC)

Explanation:
This step filters low-quality cells and genes to remove noise from the dataset, ensuring only reliable cells are used for downstream analysis.



 3. Normalize Data

Explanation:
Gene expression values are normalized to make cells comparable by removing differences caused by sequencing depth.

<img width="678" height="117" alt="IMG-20260417-WA0011" src="https://github.com/user-attachments/assets/e8c0d234-e09c-440f-ac33-60dd13601dab" />


4. Find Highly Variable Genes

Explanation:
This step selects the most informative genes that show strong variation across cells, which helps improve clustering and visualization.

<img width="1149" height="248" alt="IMG-20260417-WA0012(1)" src="https://github.com/user-attachments/assets/d58b60f1-ac3a-43bf-8b98-d8b199ccaca5" />


 5. PCA (Dimensionality Reduction)

Explanation:
Principal Component Analysis reduces the dataset dimensions while keeping the most important variation in the data.


6. Compute Neighbors

Explanation:
A nearest-neighbor graph is built to group similar cells based on their gene expression profiles.



 7. UMAP

Explanation:
UMAP is used to visualize high-dimensional single-cell data in 2D space while preserving cell relationships.

<img width="1125" height="624" alt="IMG-20260417-WA0013(1)" src="https://github.com/user-attachments/assets/db7f9a86-cf69-45e8-956f-7a6a4429292b" />

 8. Leiden Clustering

**Explanation:**
Cells are grouped into clusters based on similarity in gene expression to identify potential cell types.

<img width="1098" height="620" alt="IMG-20260417-WA0016(1)" src="https://github.com/user-attachments/assets/a596ab44-0484-46b2-b8f6-7211ae1cd2b1" />

 9. UMAP Plot

Explanation:
The final visualization shows how cells are grouped into clusters in 2D space for interpretation.

 Conclusion

In this analysis, a single-cell RNA sequencing dataset from 10x Genomics was processed using Scanpy. The dataset was first loaded and preprocessed, followed by quality control and normalization to ensure reliable expression values. Highly variable genes were selected to capture the most informative biological signals, and dimensionality reduction was performed using PCA. A nearest-neighbor graph was constructed to represent cell similarities, followed by UMAP for visualization in two dimensions. Leiden clustering was applied to group cells based on gene expression similarity, revealing distinct cell populations. Overall, this analysis successfully identified multiple transcriptionally distinct clusters, which likely represent different cell types within the sample.
