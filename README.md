# 🦖 DINOv3 Visualization Applications

[![Medium](https://img.shields.io/badge/-Medium-12100E?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@elsayed_mohamed/paper-review-dinov3-the-new-state-of-the-art-in-self-supervised-vision-models-d337ee4bf9dc)
[![Hugging Face](https://img.shields.io/badge/-🤗%20Hugging%20Face-yellow?style=for-the-badge&logoColor=white)](https://huggingface.co/spaces/sayedM/DINOv3-features)


This repository contains two interactive Gradio applications for visualizing the capabilities of the DINOv3 self-supervised vision transformer. These tools allow you to explore how the model "sees" an image by analyzing its learned features.

## 🚀 Applications

### 1. Single-Image Patch Similarity

This application lets you understand how DINOv3's learned features can be used to find similar regions within a single image.

-   **How it Works:** Upload an image and click on any point. The application will compute the cosine similarity between the feature vector of the clicked image patch and every other patch in the image. It then generates a heatmap and highlights the most semantically similar regions.
-   **Features:**
    -   Visualize similarity as a heatmap overlaid on the original image.
    -   Display the top-K most similar patches as highlighted boxes.
    -   Adjust the processing resolution, overlay opacity, and colormap.
    -   Exclude a local neighborhood around the clicked patch to find non-local matches.

### 2. PCA Explorer

This tool visualizes the principal components (PCs) of DINOv3's patch features, revealing the main axes of semantic variation within an image.

-   **How it Works:** Upload an image, and the application will perform a Principal Component Analysis (PCA) on the DINOv3 patch features. The top principal components are then visualized as heatmaps.
-   **Features:**
    -   Generate a heatmap for the first principal component (PC1).
    -   Visualize the top 3 PCs simultaneously as a colorful RGB image.
    -   View the percentage of explained variance for each of the top PCs.
    -   Control the processing resolution and heatmap style.

## 🖼️ Visualizations

Here is a demo of the Single-Image Patch Similarity application in action.

![Demo animation](assets/ezgif.com-animated-gif-maker.gif)



