# Medical 3D Visualization & Mesh Analysis

A Python-based project for converting medical image
segmentation masks into interactive 3D surface meshes.

## Project Objectives

- Load medical images and segmentation masks.
- Reconstruct 3D surfaces using Marching Cubes.
- Visualize anatomical structures interactively.
- Compute mesh geometry measurements.
- Export 3D models in STL format.

## Technologies

- Python
- NumPy
- NiBabel
- scikit-image
- Trimesh
- Plotly
- Jupyter Notebook

## Dataset

For dataset licensing and attribution details,
see [DATA_LICENSE.md](DATA_LICENSE.md).

## Project Status

Step 1: Project setup.
## Step 2 — Medical Image Loading and Exploration

In this step, CT images and lymph node segmentation masks
from the HCUCH dataset were loaded using NiBabel.

The workflow includes:

- Loading 3D NIfTI medical images.
- Checking image dimensions and voxel spacing.
- Identifying differences in image orientation.
- Aligning segmentation masks with their corresponding CT images.
- Visualizing CT slices and segmentation overlays.

### Image Alignment

The selected CT and segmentation mask had identical dimensions
and voxel spacing but different orientations.

CT orientation: LAS
Mask orientation: LAI

The mask was aligned with the CT image by reversing its
third axis after verifying the voxel-coordinate transformation.

### Dataset

The HCUCH dataset is used for this project.

The original dataset publication and access information
will be included in the dataset documentation.

### Results

CT images and their corresponding segmentation masks
were successfully loaded, geometrically aligned,
and visualized.