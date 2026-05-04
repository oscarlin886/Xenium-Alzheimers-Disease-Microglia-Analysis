# Xenium Alzheimer's Disease Microglia Analysis

This repository contains the analysis notebooks for the Xenium microglia project.

The notebooks are kept in roughly the order they were run. Some notebooks include plotting variants that were generated while preparing manuscript and supplemental figures.

---

# Clustering / Annotation Run Order

1. `Miranda_Clustering`

   Main clustering notebook.

2. `ImportAnnotation_Miranda`

   Imports Miranda's updated annotations into the clustered object.

3. `MirandaQ`

   Adds/consolidates ROI information.

4. `Miranda_regatemg_02272026`

   Microglia re-gating notebook. This is where the log1p layer was reattached and the double-gated microglia object was generated.

5. `Miranda_post_regatemg_subcluster_02272026`

   Re-clustering notebook for the double-gated microglia subset.

6. `ImportAnnotation_Miranda_mgSubclusterCLEANED`

   Imports the cleaned microglia subcluster annotations and creates the DAM/Homeostatic/IFN-responsive labeling versions.

7. `CombineFullwFC`

   Combines the updated annotations and reattaches the raw counts layer for downstream plotting and differential expression.

8. `Miranda_DAM_IFNR_combined_volcano`

   Main volcano plotting / differential expression notebook for the combined DAM and IFN-responsive annotation workflow.

9. `Miranda_DAM_IFNR_combined_boxplot`

   Boxplot notebook for the combined DAM and IFN-responsive annotation workflow.

10. `Miranda_DAM_IFNR_combined_volcano`

   Returned to this notebook for the final updated volcano/plotting object, including updated colors and legend ordering.

---

# Notes

- Large data objects are not stored in this repository.
- Raw Xenium output files are not stored in this repository.
- Several plotting notebooks contain more than one plotting version because figures and supplemental plots were revised during manuscript preparation.
