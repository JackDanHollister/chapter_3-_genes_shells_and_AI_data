# Limpet Morphometric Analysis

This repository contains the code used for data generation in the paper **"[XXXXX]"**, published in *Scientific Reports* and available at DOI: [xxxx].

## Contents

### Image Classification Pipelines

Two Jupyter notebooks implement the image classification workflows:

**1. `limpet_master_IM.ipynb` - Standard Classification Pipeline**
- Standard image classification approach
- Once the species directory and orientation are defined (e.g., `FV_dorsal`), the pipeline runs automatically

**2. Mixed Class Version**
- Ensures balanced class mixing across runs
- Maintains 50% representation from each original class in the resulting classifications

### YOLO Segmentation Pipeline

**`yolo_and_segmentation_scripts.ipynb`**

This notebook demonstrates:
- Training a YOLO model for feature detection
- Using the trained model to segment specific features (e.g., the keyhole)
- Extracting, standardizing, and deriving metrics from segmented regions
- **Note:** YOLO model training requires labeled data

### Data and Visualization

**`data_and_graph_makers/`**

This directory contains:
- F1-scores from 'Test-even' and 'Full-test' evaluations for all species across 100 iterations
- Shape metrics derived from *Fissurella volcano* (FV) keyhole measurements
- Shell metric assessments for *Lottia conus* (LC), *Lottia gigantea* (LG), and *Lottia strigatella* (LS)
- `graph_maker.ipynb` - notebook for generating all figures used in the paper

## Data Access

- **Images**: [Download link](xxxx)
- **Labels**: [Download link](xxxx)

## Citation

If you use this code, please cite:
```
[Citation details to be added]
```
