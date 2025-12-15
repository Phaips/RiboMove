# RiboMovement

Analysis of ribosome-membrane orientats from cryo-EM 3D classes.

## Method

- **Membrane detection**: High-intensity pixels identified in an annular region using percentile thresholding
- **Normal extraction**: In-plane orientation determined via PCA, through-plane tilt via linear regression across Z-slices
- **Visualization**: Angular deviations projected onto 2D tangent plane and displayed as kernel density map

## Output

The script generates:
1. **Membrane plane intersections** - Red lines show the fitted membrane plane across Z-slices for each class
2. **Movement density map** - Kernel density visualization of angular deviations from mean membrane orientation

![Membrane plane intersections](membrane_plane_intersections.png)
![Movement density map](movement_density_map.png)

## Usage
```python
python ribocone.ipynb  # or run in Jupyter
```

Requires: `numpy`, `mrcfile`, `matplotlib`
