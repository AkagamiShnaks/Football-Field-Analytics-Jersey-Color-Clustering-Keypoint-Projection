<h1 align="center">Football Field Analytics 🧠⚽</h1>

<p align="center">
  <b>Jersey Color Clustering & Keypoint Projection using Computer Vision</b><br>
</p>

<p align="center">
  <img src="https://img.shields.io/github/repo-size/AkagamiShnaks/Football-Field-Analytics-Jersey-Color-Clustering-Keypoint-Projection?color=green&style=for-the-badge" />
  <img src="https://img.shields.io/github/languages/top/AkagamiShnaks/Football-Field-Analytics-Jersey-Color-Clustering-Keypoint-Projection?style=for-the-badge" />
  <img src="https://img.shields.io/github/last-commit/AkagamiShnaks/Football-Field-Analytics-Jersey-Color-Clustering-Keypoint-Projection?color=blue&style=for-the-badge" />
</p>

---

## 📝 Summary

Two Jupyter notebooks that form a computer vision pipeline for football video analytics:

- **Color clustering** to extract dominant jersey colors of players and goalkeepers.
- **Keypoint analytics** to project top-down field information onto match footage using homography and YOLO-labeled data.

This work builds a foundation for real-time player identification, tactical mapping, and visual augmentation of football broadcasts.

---

## 📘 Notebooks Overview

### 📌 `color_clustering.ipynb`

**Goal:** Extract top jersey colors from player/goalkeeper images.

- Uses OpenCV to mask backgrounds.
- Applies KMeans clustering on foreground to find dominant colors.
- Visualizes results as labeled image grids.

**Visuals:**

![Masked Player](assets/masked_.png)
*Masked “player” frame*

![Clustering Result](assets/Clusterd_!.png)
*Dominant color clusters*

---

### 📌 `keypoints_detection.ipynb`

**Goal:** Process football keypoints and project field map onto camera views.

- Parses YOLOv8 keypoint dataset from Roboflow.
- Computes how often each field keypoint appears across frames.
- Builds a radial heatmap for spatial frequency.
- Uses homography to warp the heatmap onto match images.

**Visuals:**

![Visibility Heatmap](assets/keypoint.png)
*Keypoint visibility frequency map*

![Overlay Example](assets/heatmap.png)
*Heatmap projected onto camera image*

---

## 📁 Assets

All images used in this README are stored in the [`assets/`](https://github.com/AkagamiShnaks/Football-Field-Analytics-Jersey-Color-Clustering-Keypoint-Projection/tree/main/assets) directory.

---

## 👨‍💻 Author

**Ayon Sen**  
*Machine Learning Engineer & CV/NLP Enthusiast*  
📫 [ayon7930@gmail.com](mailto:ayon7930@gmail.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/ayon-sen-a37b50349)

---

## ⭐ Star this Repo

If you find this useful for sports analytics or computer vision research, give it a ⭐ to support!


