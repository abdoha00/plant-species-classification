# 🌿 Plant Species Classification using Machine Learning & Computer Vision

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Computer%20Vision-green.svg)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

An end-to-end Computer Vision and Machine Learning solution built to classify plant species automatically from leaf image datasets and visual botanical features.

---

## 📌 Table of Contents
- [Project Overview](#-project-overview)
- [How It Is Useful](#-how-it-is-useful)
- [What the Project Does](#-what-the-project-does)
- [Machine Learning Models & Algorithms Used](#-machine-learning-models--algorithms-used)
- [Technologies Used & Detailed Breakdown](#-technologies-used--detailed-breakdown)
- [Repository Structure](#-repository-structure)
- [Installation & Quick Start](#-installation--quick-start)
- [License](#-license)

---

## 🎯 Project Overview

Accurate plant species identification is crucial for biodiversity monitoring, agricultural management, and botanical conservation. Manual identification can be time-consuming and requires specialized domain expertise.

This project implements an automated visual classification pipeline (`plant species classification.ipynb`) that uses image processing techniques and machine learning algorithms to recognize plant species based on leaf morphology, texture, and visual attributes.

---

## 💡 How It Is Useful

- **Agricultural & Botanical Support:** Aids farmers, researchers, and botanists in quickly identifying plant species and crop types.
- **Automated Feature Extraction:** Converts raw image arrays into meaningful numerical features (such as color histograms, texture, and shape descriptors).
- **Scalable Classification:** Replaces manual visual inspection with reproducible, high-speed machine learning predictions.
- **Educational & Research Benchmark:** Offers a modular foundation for computer vision applications in environmental science and precision agriculture.

---

## 🔍 What the Project Does

1. **Image Preprocessing & Augmentation:** Loads leaf/plant images, resizes image inputs to standard dimensions, normalizes pixel intensity values, and handles noise reduction.
2. **Feature Extraction:** Extracts key visual representations—including color metrics, edge detection features, and morphological shape parameters.
3. **Exploratory Visual Analysis:** Displays sample image batches, plots class label distributions, and visualizes feature mappings across species categories.
4. **Model Training & Benchmarking:** Trains and benchmarks machine learning classifiers on extracted features to achieve optimal classification performance.
5. **Model Evaluation:** Analyzes model performance using confusion matrices, precision, recall, and multi-class accuracy metrics.

---

## 🤖 Machine Learning Models & Algorithms Used

The notebook evaluates multiple machine learning classifiers to accurately distinguish between plant species:

| Model / Algorithm | Category | Role & Purpose |
| :--- | :--- | :--- |
| **Logistic Regression** | Linear Classifier | Serves as a fast baseline model for multi-class classification using linear decision boundaries. |
| **Random Forest Classifier** | Ensemble Method | Utilizes an ensemble of decision trees to capture non-linear feature interactions and rank feature importances. |
| **Support Vector Machine (SVM)** | Kernel-based Classifier | Projects extracted visual features into higher dimensions using kernel functions (e.g., RBF) to find optimal margin separation. |
| **Decision Tree Classifier** | Tree-based Model | Learns hierarchical decision rules based on leaf shape, color metrics, and texture patterns. |
| **K-Nearest Neighbors (KNN)** | Instance-based Model | Classifies plant species based on the majority vote of the nearest feature-space neighbors. |

---

## 🛠️ Technologies Used & Detailed Breakdown

| Technology | Role | Detailed Explanation |
| :--- | :--- | :--- |
| **Python** | Core Language | The primary programming environment for orchestrating data processing, vision libraries, and model execution. |
| **OpenCV / Pillow** | Image Processing | Performs low-level image operations including color space transformations, thresholding, edge detection, and image resizing. |
| **NumPy** | Array Operations | Manages high-dimensional matrix arrays representing image pixel intensities and numerical feature representations. |
| **Pandas** | Tabular Data Handling | Manages metadata, dataset image paths, class labels, and extracted feature matrices in structured dataframes. |
| **Matplotlib & Seaborn** | Data & Image Visualization | Displays visual output plots, sample image grids, training progress curves, and confusion matrix heatmaps. |
| **Scikit-Learn** | Machine Learning Engine | Drives image classification algorithms, feature scaling (e.g., `StandardScaler`), train-test splitting, and evaluation metrics. |
| **Jupyter Notebook** | Development Interface | The primary environment (`plant species classification.ipynb`) documenting step-by-step code execution, visual outputs, and benchmarks. |

---

## 📂 Repository Structure

```text
plant-species-classification/
├── plant species classification.ipynb   # Main Jupyter Notebook containing complete vision pipeline & ML models
└── README.md                            # Full project documentation
```

---

## ⚙️ Installation & Quick Start

### Prerequisites
Ensure **Python 3.8+** is installed on your system.

### 1. Clone the Repository
```bash
git clone https://github.com/abdoha00/plant-species-classification.git
cd plant-species-classification
```

### 2. Set Up a Virtual Environment (Optional)
```bash
# Windows
python -m venv venv
venv\Scripts\activate

# macOS / Linux
python -m venv venv
source venv/bin/activate
```

### 3. Install Required Dependencies
```bash
pip install numpy pandas matplotlib seaborn opencv-python scikit-learn jupyter
```

### 4. Run the Notebook
```bash
jupyter notebook "plant species classification.ipynb"
```

---

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.
