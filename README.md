# TrackMate_CellPose_Bacterial_Generation_Determination
End-to-end pipeline for bacterial single-cell lineage, growth, and morphology analysis from TrackMate exports with publication-ready plots (Colab-friendly).

# Bacterial Cell Growth & Shape Analysis Pipeline

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/JoeVPhD/TrackMate_CellPose_Bacterial_Generation_Determination/blob/main/TrackMate_CellPose_Bacterial_Generation_Determination.ipynb)


## Overview
Automated analysis pipeline for bacterial cell lineage tracking, morphology quantification, and multi-condition population comparisons. Analyzes shape mutants, growth rates, division timing, and cell geometry across generations.

## Key Features
- **Lineage Memory Analysis**: Mother-daughter growth correlations
- **Sister Cell Symmetry**: Division timing asymmetry quantification  
- **Size Control Models**: Adder/Timer/Sizer classification
- **Geometric Profiling**: Length, width, aspect ratio, circularity across 12 metrics
- **Statistical Rigor**: Mann-Whitney U tests + Cliff's Delta effect sizes with FDR correction

## Quick Start (No Coding Required!)

### Option 1: Google Colab (Recommended)
1. Upload your files to Google Drive
2. Click the "Open in Colab" badge above
3. Mount Google Drive
4. Set Parameters to your liking
5. Click Runtime → Run All
6. Select folder containing your paired spots.csv and edges.csv using interactive folder selector
7. Wait for files to process
8. Visualize by selecting an output folder using the interactive folder selector at the end of the code
9. Download results from the output folder

### Option 2: Local Installation
See [Installation Guide](docs/installation.md)

## Input Data Format
CSV files from TrackMate required: _spots.csv and _edges.csv 
**Files should be saved in Date_Mutatation_Gene_Location format** (example: 20260101_L206K_mreB_s1_spots.csv / 20260101_L206K_mreB_s1_edges.csv

[Download sample dataset](data/sample/example_data.csv)

## Output Files
- **Plots**: 15+ publication-ready figures (PNG, 150 DPI)
- **Stats Table**: `Boss_Summary_Table.csv` with medians & sample sizes
- **Raw Data**: `Total_Population_Dataset.csv` for custom analysis

## Citation
If you use this pipeline, please cite: [Your Paper/DOI]

## License
MIT License - See LICENSE file

## Contact
Questions? JoeVPhD@gmail.com
