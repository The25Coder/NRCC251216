# NRCC251216
NRSC Coding Challenge 2025

# Cloud and Shadow Mask Generator for Resourcesat-2/2A LISS-IV Images

## Description

This Python tool automatically detects clouds, shadows, and water bodies in Resourcesat-2/2A LISS-IV 3-band images (Green, Red, NIR) using threshold-based methods on normalized reflectance bands.

The masks are saved as GeoTIFF files alongside the input image, and a combined mask includes:

- 0: Clear
- 1: Cloud
- 2: Shadow
- 3: Water

The tool features a simple GUI for easy file selection, mask generation, and visualization.

---

## Requirements

- Python 3.x
- numpy
- rasterio
- matplotlib
- tkinter (usually included with Python)

Install dependencies via pip:

```
pip install numpy rasterio matplotlib
```

---

## Usage

1. Run the script:

```
python cloud_shadow_masking.py
```

2. Click **Select File** to choose the input LISS-IV GeoTIFF.

3. Click **Run Masking** to generate cloud, shadow, and water masks.

4. Click **View Results** to visualize masks overlaid on a false-color composite.

5. Masks are saved in the same directory as the input file with suffixes:

   - `_cloud_mask.tif`
   - `_shadow_mask.tif`
   - `_water_mask.tif`
   - `_combined_mask.tif`

---

## Notes

- Threshold values can be tuned within the script for different scenes.
- This is a simple approach; complex scenes might require advanced methods.
- Suitable for quick assessment and baseline masking.

---

## Author

Ashish Kr. Sharma  
Date: 8-June-2025
