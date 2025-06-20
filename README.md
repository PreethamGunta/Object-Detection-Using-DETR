
# Object Detection Using DETR

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg) ![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=flat&logo=pytorch&logoColor=white) ![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97%20hugging%20face-transformers-blue)

This repository contains the code and the final results for fine-tuning and evaluating a DETR (DEtection TRansformer) model on a custom traffic scene dataset. The project is implemented using Jupyter Notebooks.

---

## Repository Structure

```
├── notebooks/
│ ├── DETR_Training.ipynb # Trains the model.
│ └── DETR_Evaluation.ipynb # Evaluates the model.
├── model weights/
│ └── model_weights_link.txt # A link to download the final model weights.
├── report/
│ ├── Object Detection Using DETR.pdf # Detailed project report.
│ ├── Object Detection Using DETR.tex # LaTeX source file for the report.
│ ├── refs.bib # Bibliography file for the report.
│ └── images/ # Images used in the report.
└── README.md # This file.
```

---

## Quick Start Guide

### 1. Setup

**A. Clone the repository:**
```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

**B. Install dependencies:**
It is recommended to use a virtual environment.
```bash
# Create and activate a virtual environment
python -m venv venv
source venv/bin/activate

# Install required packages
pip install torch torchvision transformers pycocotools tqdm numpy Pillow jupyterlab matplotlib seaborn
```

**C. Prepare data:**
Place your dataset following this structure of images and coco format annotations:
```
data/
├── images/
│   ├── 00001.jpg
│   └── ...
└── output_coco.json
```

### 2. Usage

**A. Train the Model:**
- Open the `notebooks/DETR_Training.ipynb` notebook.
- **Important:** Check and update the file paths in the notebook.
- Set the number of epochs and run the `DETR_Training.ipynb` notebook to train the model.


**B. Evaluate the Model:**
- Open the `notebooks/DETR_Evaluation.ipynb` notebook.
- **Important:** Ensure that image data, trained model weights and other paths in the notebooks are correct.
- Run the notebook.
- This will generate all the evaluation metrics and visualizations discussed in the report.

---

## Full Report

For a detailed analysis of the methodology, results, and conclusions, please see the full PDF report.

**➡️ [Read the Full Report (PDF)](report/Object%20Detection%20Using%20DETR.pdf)**

---

## Authors
- **Gunta Preetham** (23125013)
- **Kodavali Purnendra Sri Krishnaditya** (23125017)
