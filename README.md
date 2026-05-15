This is a professional README.md drafted in English, optimized for an academic audience and structured to serve as a formal reference for your submission to BMC Medical Informatics and Decision Making.
Multidimensional Symptom Profiles and Clinical Trajectories in Fibromyalgia

This repository contains the computational pipeline and research data management workflow for the study: "Symptom Trajectories and Tolerability of Low-Intensity Repetitive Transcranial Magnetic Stimulation (Li-rTMS) in Fibromyalgia".

The project identifies distinct patient phenotypes and tracks clinical evolution through machine learning (K-means++) and longitudinal transition analysis.
📂 Repository Structure
Plaintext

.
├── notebooks/
│   ├── 01_Data_Curation_Fin.ipynb      # Raw data cleaning and preprocessing
│   └── 02_Processing_Github.ipynb     # Clustering, validation, and trajectories
├── results/
│   ├── figures/                       # PNG exports (Heatmaps, Sankey, Stability)
│   └── tables/                        # CSV summaries (Clinical profiles, Metrics)
└── README.md

🚀 Computational Pipeline
1. Data Curation & Preprocessing

The first stage, handled by 01_Data_Curation_Fin.ipynb, transforms raw clinical data into an analysis-ready format.

    Input: Dataset_Bioinformatics_Completo.csv

    Operations: Outlier detection (Z-score), missing value imputation, categorical encoding, and feature standardization.

    Output: Dataset_Bioinformatic_Depured.csv

2. Phenotyping & Validation

The core analysis is performed in 02_Processing_Github.ipynb.

    Clustering Analysis: Implementation of K-means++ to identify three clinical profiles: CP1 (Mild), CP2 (Moderate), and CP3 (Severe).

    Robustness Testing: Cluster stability is validated using a Bootstrap Jaccard Index (n=100) and Silhouette Scores.

    Trajectory Mapping: Longitudinal flow analysis between treatment stages (Pre-treatment, Intermediate, and Post-treatment).

📊 Key Visualizations

The pipeline generates the following clinical insights:

    Phenotype Heatmap: A multidimensional characterization of clusters based on FIQ (Fibromyalgia Impact Questionnaire), WPI (Widespread Pain Index), and SSS (Symptom Severity Scale).

    Sankey Diagram: A visual representation of patient "jumps" between severity profiles, illustrating the therapeutic effect of Li-rTMS.

    Stability Plot: Statistical proof of cluster reproducibility.

🛠️ Requirements

The analysis is optimized for Google Colab. Required dependencies:

    scikit-learn (Clustering & Metrics)

    pandas/numpy (Data Processing)

    seaborn/matplotlib (Statistical Visualization)

    plotly/kaleido==0.2.1 (Longitudinal Trajectories)

📜 Citation & Reproducibility

This repository is part of a peer-reviewed submission. For reproducibility, please ensure you execute the notebooks in sequential order.

Reference:

    González, N. F., et al. (2026). Symptom Trajectories and Tolerability of Low-Intensity Repetitive Transcranial Magnetic Stimulation (Li-rTMS) in Fibromyalgia. BMC Medical Informatics and Decision Making.

Corresponding Author: Nazario Félix González – Center for Biomedical Technology (CTB-UPM), Universidad Politécnica de Madrid. 
nazario.felix@ctb.upm.es

## ⚖️ License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
