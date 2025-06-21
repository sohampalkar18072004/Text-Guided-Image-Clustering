Multimodal Image Clustering
This project performs unsupervised clustering of images by combining visual features (e.g., ResNet50, SIFT, HOG, LBP, Histograms) and textual features (SBERT embeddings from BLIP-generated captions). The goal is to group visually and semantically similar images without using labels during training.

🔍 Project Overview
Dataset: Images with associated labels (used only for evaluation).

Vision Features:

Deep CNN (ResNet50)

Classical: SIFT, HOG, Color Histogram, Canny Edges, LBP

Text Features:

Captions generated using BLIP

SBERT (all-mpnet-base-v2) used to extract semantic embeddings

Feature Fusion: All features normalized and concatenated into a single vector.

Clustering Algorithms:

K-Means

Agglomerative Clustering

Evaluation:

Adjusted Rand Index (ARI) on train, val, test splits

Visualization:

t-SNE for 2D embedding plots of feature space
