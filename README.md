# Processing pipeline (Python notebooks) for "Multimodal MRI Marker of Cognition Explains the Association Between Cognition and Mental Health in UK Biobank"
**1_Cognitive_preprocessing**
- 01_GetCogData: Uploading and primary preparation of cognitive performance data (selection of appropriate metrics, score transformation, etc.), including split into 5 folds.
- 02_CogData_Descriptive_5Folds: Descriptive statistics for cognitive performance scores in each of the 5 folds.
- 03_GetGFactor_5Folds: Derivation of the *g*-factor using ESEM/CFA.
- 04_GetGFactor_SingleSplit: Derivation of the *g*-factor using ESEM/CFA for a single train/test split to visualize model parameters.

**2_Mental_Health**
- 01_GetMHData:
- 02_MHData_Descriptives:

**3_MRI_preprocessing**
- 01_GetMRIData_dwMRI_IDP:
- 02_GetMRIData_dwMRI_Parcellations:
- 03_GetMRIData_sMRI:
- 04_GetMRIData_rsMRI_IDP_FullPartCorr_Confounds:
- 05_GetMRIData_rsMRI_Parcellations:
- 06_GetMRI_rsMRI_Parcellations_Get2DMatrix:

**4_PLS**
- 01_PLS_MH_5Folds:
- 02_1_PLS_MH_SingleSplit:
- 02_2_PLS_MH_SingleSplit:
- 03_PLS_dwMRI_IDP:
- 04_PLS_dwMRI_Parcellations:
- 05_PLS_rsMRI_Select_RSFC_Estimate:
- 06_PLS_rsMRI_IDP_Tangent:
- 07_PLS_rsMRI_Parcellations_FullCorr:
- 08_PLS_sMRI_IDP_T1w:
- 09_PLS_sMRI_IDP_WholeBrainT1w_T2w_:
- 10_PLS_ResultPlotFolds:

**5_Bootstrap_and_Stack**
- 01_Stacking_CombinePhenotypes:
- 02_Stacking:
- 03_Bootstrapping:

**6_Commonality_Analysis**
- 01_Commonality_Analysis:
