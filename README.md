# CIELAB Color Analysis Code

This folder contains the code used to perform the CIELAB color analysis reported in the accompanying research paper.

## Overview

The analysis converts sampled visual data from the source material into the CIELAB color space. CIELAB represents color using three dimensions:

- **L\***: perceptual lightness, ranging from black to white
- **a\***: the green–red color axis
- **b\***: the blue–yellow color axis

The scripts were used to extract color information, calculate summary measures, and generate the tables and visualizations used in the analysis.

## Folder contents

| File or folder | Description |
|---|---|
| `[01_extract_frames.py]` | Extracts frames or images from the source video. |
| `[02_convert_to_cielab.py]` | Converts image pixels from RGB to CIELAB. |
| `[03_calculate_statistics.py]` | Calculates descriptive statistics for L\*, a\*, and b\*. |
| `[04_generate_visualizations.py]` | Produces figures and plots from the calculated values. |
| `[utils.py]` | Contains shared helper functions. |
| `[config.yaml]` | Stores analysis parameters and file paths. |
| `[requirements.txt]` | Lists the required Python packages. |

Rename or remove rows so that this table matches the files included in the folder.

## Analysis workflow

The analysis follows these steps:

1. Extract frames or load the selected images.
2. standardize the images where required.
3. Convert pixel values from RGB to CIELAB.
4. Calculate image-level or frame-level CIELAB statistics.
5. Export the calculated measurements in a tabular format.
6. Generate the figures and summaries used in the paper.

## Software requirements

The analysis was conducted using:

- Python `[version]`
- NumPy `[version]`
- pandas `[version]`
- OpenCV `[version]`
- scikit-image `[version]`
- Matplotlib `[version]`
- seaborn `[version]`

Install the required packages with:

```bash
pip install -r requirements.txt
