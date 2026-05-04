# Xenium Alzheimer's Disease Microglia Analysis

This repository contains analysis notebooks and supporting code for Xenium spatial transcriptomics analysis of microglial states in an Alzheimer's disease mouse model.

---

# New Slides Clustering Pipeline

The notebooks below summarize the main execution order for the new-slide microglia clustering and downstream DAM/homeostatic/IFN-responsive analyses.

## Execution Order

1. `Miranda_Clustering`

   Initial clustering workflow for the new-slide Xenium object.

2. `ImportAnnotation_Miranda`

   Imports Miranda-updated annotations into the clustered object.

3. `MirandaQ`

   Adds and consolidates ROI information.

4. `Miranda_regatemg_02272026`

   Reattaches the `log1p` layer and performs double gating of the microglia subset.

5. `Miranda_post_regatemg_subcluster_02272026`

   Reclusters the double-gated microglia subset.

6. `ImportAnnotation_Miranda_mgSubclusterCLEANED`

   Imports cleaned microglia subcluster annotations and generates DAM/homeostatic/IFN-responsive labeling variants.

7. `CombineFullwFC`

   Combines full annotations and reattaches the raw counts layer for downstream analysis.

8. `Miranda_DAM_IFNR_combined_volcano`

   Generates combined DAM/IFN-responsive volcano plot inputs and cleaned annotation names.

9. `Miranda_DAM_IFNR_combined_boxplot`

   Generates boxplot visualizations for combined DAM/IFN-responsive analyses.

10. `Miranda_DAM_IFNR_combined_volcano`

    Final updated volcano plotting workflow, including updated color palette and plot legend ordering.

---

# Notes

- The final analysis object used for later plotting includes updated color palettes and legend ordering.
- Raw count information is restored before downstream differential expression and volcano plotting.
- Multiple volcano and plotting variants were generated during manuscript and supplement preparation. Not all retained plotting variants necessarily correspond to final submitted panels.
- Large data objects and raw Xenium outputs are not stored in this repository.
