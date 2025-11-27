# 2D-to-3D-conversion-using-DPT-and-MiDaS-

2D-to-3D-conversion-using-DPT-and-MiDaS is an end-to-end pipeline that transforms single-view 2D images into high-quality 3D models using monocular depth estimation, depth map optimization, point cloud sampling, and hybrid surface reconstruction. This system is designed to streamline 3D model generation for educational, VR/AR, and autonomous applications by integrating cutting-edge techniques into a seamless workflow.

## ✨ Features

- Monocular depth estimation using MiDaS / DPT models.
- Depth map enhancement via Laplacian fusion and bilateral filtering.
- K-means clustering for geometric segmentation.
- Farthest Point Sampling for efficient point cloud reduction.
- Hybrid mesh reconstruction using Poisson surface reconstruction and Ball Pivoting algorithm.
- Export 3D models in `.PLY` and `.OBJ` formats compatible with Blender and other tools.
- Real-time compatible processing with high mesh fidelity.

## 📌 Pipeline Overview

1. Monocular Depth Estimation**: Generate depth maps from RGB images using pretrained models.
2. Depth Map Optimization**: Enhance edges and reduce noise using Laplacian fusion and bilateral filtering.
3. Point Cloud Generation & Sampling**: Convert depth maps to 3D point clouds and apply Farthest Point Sampling.
4. Mesh Generation**: Use Poisson and Ball Pivoting reconstruction to generate watertight meshes.
5. Export for Blender**: Save results as `.PLY` / `.OBJ` for visualization and further editing.

## 📄 Research Paper & Technical Documentation

This project is supported by our research work titled “Edu3D: From Diagrams to Interactive 3D Models”, which presents an optimized pipeline combining monocular depth estimation, Laplacian fusion, bilateral filtering, geometric segmentation, and hybrid Poisson + Ball Pivoting surface reconstruction.

# Our study demonstrates:

22.2% improvement in Mean Edge Strength (MES)
Higher Shannon Entropy, indicating better structural detail
Superior mesh consistency using Laplacian-guided depth optimization
Smooth conversion of single-view 2D diagrams into Blender-ready 3D models
Efficient point cloud processing using Farthest Point Sampling (FPS)

The research validates the complete 2D-to-3D pipeline used in this repository and highlights its suitability for educational content creation, VR/AR assets, robotics, and interactive visualization.


## 🔧 Install Dependencies

```bash
pip install -r requirements.txt




