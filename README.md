# Orthogeriatric Fracture Syndrome: A Large-Scale Bibliometric Analysis of a Proposed Concept for Cross-Disciplinary Awareness and Coordinated Care

Keyword co-occurrence analysis of OFS-related terms in the PubMed literature (2026 snapshot).

## Analysis overview
 
The notebook proceeds in four steps:
 
1. **Keyword filtering** — binary presence flags for OFS, age-related, metabolic syndrome, and negative control terms across ~23M abstracts
2. **Prevalence statistics** — keyword occurrence counts and butterfly plot comparing fragility vs. non-fragility fracture papers
3. **Pairwise φ-coefficient analysis** — correlation heatmap with χ²/Fisher exact tests and Holm FDR correction
4. **t-SNE visualisation** — embedding projection coloured by keyword group
   
## Data
 
Expects preprocessed PubMed 2026 data (https://pubmed.ncbi.nlm.nih.gov/download/). Precomputed t-SNE coordinates are loaded from (https://github.com/berenslab/pubmed-landscape). 

## Dependencies

Python 3.10.16. Key libraries: numpy 1.26.4, pandas 2.2.3, scipy 1.11.4, statsmodels 0.14.4, matplotlib 3.10.1, openTSNE 1.0.2.

Custom package: `pubmed_landscape_src` (see https://github.com/alceubissoto/OFS_pubmed).
