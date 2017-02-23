# 3D terrain rendering pipeline

A vision for 3D terrain rendering with WebGL

# GOAL: drape maps on top of terrain

- Quick generation of small areas at high resolution
- Larger areas at low resolution
- A way to view online or in an Electron app
- A way to save viewpoint for repeatable generation (say, for print graphics)

# Ingredients

1. Feature (from database or file), probably as GeoJSON
2. Bounding box for analysis
3. Heightfield
  - What image format?
  - Is there a single way to generate this?
4. Image
  - draped over heightfield

# Pipeline

Heightfield and image swatch should be generated procedurally from a bounding box.
But they should also be cacheable for e.g. web use.

Pipeline should be crs-agnostic.

Should heightfield come from standard software or is its preparation more ad-hoc?

# Prior art

[MeshLab](http://www.meshlab.net)
[Qgis2threejs](https://plugins.qgis.org/plugins/Qgis2threejs/)

