# Processing pipeline (Python notebooks) for "Multimodal MRI Marker of Cognition Explains the Association Between Cognition and Mental Health in UK Biobank"
**1_Cognitive_preprocessing**
- 01_GetCogData: Uploading and primary preparation of cognitive performance data (selection of appropriate metrics, score transformation, etc.), including split into 5 folds.
- 02_CogData_Descriptive_5Folds: Descriptive statistics for cognitive performance scores in each of the 5 folds (html view: https://HAM-lab-Otago-University.github.io/UKBiobank/1_Cognitive_preprocessing/03_GetGFactor_5Folds.html).
- 03_GetGFactor_5Folds: Derivation of the *g*-factor using ESEM/CFA.
- 04_GetGFactor_SingleSplit: Derivation of the *g*-factor using ESEM/CFA for a single train/test split to visualize model parameters (html view: https://HAM-lab-Otago-University.github.io/UKBiobank/1_Cognitive_preprocessing/04_GetGFactor_SingleSplit.html).

**2_Mental_Health**
- 01_GetMHData: Uploading and primary preparation of cognitive performance data.
- 02_MHData_Descriptives: Descriptive statistics for mental health indices.

**3_MRI_preprocessing**
- 01_GetMRIData_dwMRI_IDP: Uploading and primary preparation of dwMRI data
- 02_GetMRIData_dwMRI_Parcellations: Uploading and primary preparation of dwMRI structural connectome data
- 03_GetMRIData_sMRI:  Uploading and primary preparation of sMRI data
- 04_GetMRIData_rsMRI_IDP_FullPartCorr_Confounds: Uploading and primary preparation of rsMRI data
- 05_GetMRIData_rsMRI_Parcellations: Uploading and primary preparation of rsMRI BOLD time series data
- 06_GetMRI_rsMRI_Parcellations_Get2DMatrix:A code to convert a 1D array back to matrix

**4_PLS**
- 01_PLS_MH_5Folds: PLSR on mental health in 5 folds
- 02_1_PLS_MH_SingleSplit: PLSR on mental health in the whole sample (pt.1)
- 02_2_PLS_MH_SingleSplit: PLSR on mental health in the whole sample (pt.2)
- 03_PLS_dwMRI_IDP: PLSR on dwMRI IDPs in 5 folds
- 04_PLS_dwMRI_Parcellations: PLSR on dwMRI structural connectomes in 5 folds
- 05_PLS_rsMRI_Select_RSFC_Estimate: Select the best RSFC estimate in a training set
- 06_PLS_rsMRI_IDP_Tangent: PLSR on rsMRI IDPs (tangent matrices) in 5 folds
- 07_PLS_rsMRI_Parcellations_FullCorr: PLSR on rsMRI functional connectomes (full correlations) in 5 folds
- 08_PLS_sMRI_IDP_T1w: PLSR on sMRI IDPs (T1w segmentations) in 5 folds
- 9_PLS_sMRI_IDP_WholeBrainT1w_T2w: PLSR on sMRI IDPs (whole-brain T1w and T2w) in 5 folds
- 10_PLS_ResultPlotFolds: A code to plot results

**5_Bootstrap_and_Stack**
- 01_Stacking_CombinePhenotypes: A code to combine predicted g-factor to build a second-level stacked model
- 02_Stacking: Second-level stacked model
- 03_Bootstrapping: A code to obtain a bootstrap distribution of Pearson r and R2

**6_Commonality_Analysis**
- 01_Commonality_Analysis: Commonality analyses + plots
