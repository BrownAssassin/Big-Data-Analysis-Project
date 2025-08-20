# Big Data Analysis & Project - Domain Transfer for Martian Traversability Classification

This repository contains the code and experiments for the research project:

> **"Evaluating Domain Transfer for Martian Terrain Traversability Classification Using Terrestrial Imagery"**

Conducted as part of the **Big Data Analysis and Project** course in the Master of Artificial Intelligence and Machine Learning program at the University of Adelaide.

## 🚀 Project Overview

The goal of this project is to evaluate whether co-training convolutional neural networks (CNNs) on terrestrial datasets can improve binary terrain traversability classification on Martian imagery.

We compare three models:
- Logistic Regression (baseline)
- Mini-CNN (lightweight custom architecture)
- MobileNet-V2 (pre-trained and fine-tuned)

All models are evaluated under two configurations:
1. **Mars-only** training (AI4Mars dataset)
2. **Mars+Earth** co-training (AI4Mars + Freiburg Forest datasets)

---

## 🗂 Repository Structure

```
.
├── 10E32C16M/                   # Output plots, saved models, & code snapshot for 15 Epoch Trial (CNN Batch Size: 32; MobileNet Batch Size: 16)
├── 15E64C32M/                   # Output plots, saved models, & code snapshot for 15 Epoch Trial (CNN Batch Size: 64; MobileNet Batch Size: 32)
├── EDA/                         # Output plots and code snapshot from EDA
├── ai4mars-dataset-merged-0.1/  # Dataset containing Martian imagery
├── freiburg_forest_annotated/   # Dataset containing Terrestrial imagery
├── Big Data Analysis.ipynb      # Notebook for exploratory data analysis
├── Modelling.ipynb              # Main notebook for data prep, training, evaluation, and visualization
└── README.md                    # Project README
```

---

## 📦 Installation

1. **Clone this repository:**
```bash
git clone https://github.com/BrownAssassin/Big-Data-Analysis-Project.git
cd Big-Data-Analysis-Project
```
2. Set up a virtual/conda environment (optional)
3. Install dependencies:
```bash
pip install numpy matplotlib pandas opencv-python scikit-learn torch torchvision albumentations
```

---

## 📁 Datasets

This project uses two datasets:

1. AI4Mars (Martian imagery)
    - Source: [NASA Open Data Portal](https://data.nasa.gov/dataset/ai4mars-a-dataset-for-terrain-aware-autonomous-driving-on-mars)

2. Freiburg Forest (Earth imagery)
    - Source: [DeepScene Freiburg](https://deepscene.cs.uni-freiburg.de/)

These datasets are already included in the repository with the required cleaning done.

---

## ▶️ Running the Code

Open the Jupyter Notebook then run each cell in order to:

- Load and preprocess the datasets
- Train the three models on Mars-only and Mars+Earth data
- Generate performance metrics (Precision, Recall, F1-Score, Balanced Accuracy)
- Visualize confusion matrices and learning curves

---

## 📄 Report

A full research report following the IEEE template (with abstract, literature review, methodology, and results) is available in the course submission portal.

---

## 📜 License

This repository is for academic and educational use. For dataset usage, please refer to the licenses of [AI4Mars](https://data.nasa.gov/dataset/ai4mars-a-dataset-for-terrain-aware-autonomous-driving-on-mars) and [Freiburg Forest](https://deepscene.cs.uni-freiburg.de/).

---

## 🙋‍♂️ Author

**Mrinank Sivakumar**

*Master of AI and Machine Learning, University of Adelaide*

[mrinank.sivakumar@student.adelaide.edu.au](mailto:mrinank.sivakumar@student.adelaide.edu.au)
