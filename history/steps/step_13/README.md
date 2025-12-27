# Classification Methods Visualization

**Interactive visualization and comparison of classification algorithms on synthetic datasets**

A Jupyter notebook demonstrating logistic regression, Linear Discriminant Analysis (LDA), and Quadratic Discriminant Analysis (QDA) for binary classification with decision boundary visualization and performance comparison.

## Overview

This project provides a hands-on exploration of three fundamental classification algorithms in machine learning. Through interactive visualizations and synthetic datasets, it illustrates how different classifiers form decision boundaries and perform under various data distributions.

### What It Does

1. **Logistic Regression for Binary Classification**
   - Generates synthetic binary classification datasets
   - Fits logistic regression models
   - Visualizes decision boundaries
   - Analyzes prediction probabilities and classification metrics

2. **Gaussian Data Exploration**
   - Creates datasets with different covariance structures (isotropic, shared, different)
   - Demonstrates how data distribution affects classifier choice

3. **LDA vs QDA Comparison**
   - Applies both Linear Discriminant Analysis and Quadratic Discriminant Analysis
   - Visualizes decision boundaries side-by-side
   - Compares performance across different covariance scenarios

### Problem & Approach

**Problem:** Understanding the geometric interpretation of classification algorithms and their suitability for different data distributions requires visual exploration.

**Approach:** Generate controlled synthetic datasets with known properties, apply classification methods, and visualize decision boundaries to build intuition about when each method excels.

## Tech Stack

- **Python 3.x** - Core programming language
- **Jupyter Notebook** - Interactive computing environment
- **NumPy** - Numerical operations and array handling
- **Matplotlib** - Visualization and plotting
- **scikit-learn** - Machine learning algorithms and datasets

## Repository Structure

```
.
├── classification_visualization.ipynb   # Main notebook with all demonstrations
├── requirements.txt                     # Python dependencies
├── README.md                           # This file
└── .gitignore                          # Python/Jupyter ignore patterns
```

## Setup

### Prerequisites

- Python 3.7 or higher
- pip package manager

### Installation

1. Clone the repository:
```bash
git clone https://github.com/Raminyazdani/notebook-problem-solution-visualization.git
cd notebook-problem-solution-visualization
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

**Dependencies:**
- numpy >= 1.21.0
- matplotlib >= 3.3.0
- scikit-learn >= 0.24.0
- jupyter >= 1.0.0

Alternatively, install individually:
```bash
pip install numpy matplotlib scikit-learn jupyter
```

## How to Run

### Option 1: Jupyter Notebook Interface

1. Start Jupyter:
```bash
jupyter notebook
```

2. Open `classification_visualization.ipynb` in your browser

3. Run cells sequentially (Shift+Enter) from top to bottom

### Option 2: JupyterLab

```bash
jupyter lab
```
Then navigate to and open `classification_visualization.ipynb`.

### Option 3: VS Code

If using VS Code with the Jupyter extension:
1. Open `classification_visualization.ipynb`
2. Select Python kernel
3. Run cells interactively

## Data & Inputs

**No external data files required.** All datasets are generated synthetically using scikit-learn:

- `make_classification()` - Creates binary classification problems
- `make_blobs()` - Generates Gaussian distributed clusters

**Configurable Parameters (within notebook):**
- Number of samples
- Number of features
- Covariance structures
- Random seeds (for reproducibility)

All random seeds are fixed in the notebook to ensure reproducible results.

## Outputs

All outputs are rendered inline within the Jupyter notebook:

### Visualizations
- Scatter plots of synthetic datasets color-coded by class
- Decision boundary plots for each classifier
- Confusion matrices
- Probability distribution histograms
- Side-by-side LDA vs QDA comparisons

### Metrics
- Accuracy scores
- Type I and Type II error rates
- Classification performance summaries

**No external files are created** - all results are embedded in the notebook.
