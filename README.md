## Project Objectives

- Extract the **top 3 dominant colors** from each image using K-Means clustering.
- Represent each image as a **9-dimensional RGB vector**.
- Cluster all images into **10 color scheme groups** based on their dominant palettes.
- Use **Principal Component Analysis (PCA)** to visualize the clustering structure.
- Compare **engagement levels** (likes, repins, comments) across different color themes.
- Manually interpret cluster aesthetics (e.g., “Cool Slate,” “Muted Reds”) and correlate them with performance.

---

## Methodology

1. **Image Preprocessing**: Images resized to 100×100 pixels and converted to RGB arrays.
2. **Color Feature Extraction**: Applied K-Means to extract top 3 dominant colors (RGB).
3. **Color Clustering**: Used K-Means (n_clusters=10) to group all images into color profile clusters.
4. **Dimensionality Reduction**: Applied PCA to project color vectors into 2D space for visualization.
5. **Engagement Analysis**: Compared average likes, repins, and comments across clusters.
6. **Manual Labeling**: Assigned descriptive names to each cluster based on dominant tones.

---

## Key Findings

- Cool-toned and neutral palettes (e.g., soft greens, grays) attracted higher engagement.
- Warm and muted red-heavy clusters underperformed.
- PCA visualization revealed clear grouping patterns aligned with color aesthetics.
- Cluster sizes varied, which introduced slight skew in engagement averages.

---

## Technologies Used

- Python 3
- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `scikit-learn`
- Jupyter Notebook

---

## Getting Started

### Requirements

- Python 3.8+
- Jupyter Notebook or VSCode with Jupyter extension
- Required packages:
  ```bash
  pip install pandas numpy matplotlib seaborn scikit-learn
