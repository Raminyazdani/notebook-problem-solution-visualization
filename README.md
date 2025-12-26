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

## Notebook Contents

The notebook is organized into the following sections:

1. **Imports and Setup** - Load libraries and define plotting utilities
2. **Logistic Regression** - Binary classification with synthetic data
3. **Exercises**:
   - Exercise 1: Analyze prediction probability distributions
   - Exercise 2: Compute Type-1 and Type-2 errors
   - Exercise 3: Visualize correct vs incorrect predictions
4. **Gaussian Data Exploration** - Different covariance structures
5. **LDA and QDA Theory** - Mathematical background
6. **Comparative Analysis** - Visual performance comparison

## Reproducibility

### Fixed Random Seeds
The notebook uses fixed random seeds (`random_state` parameters) to ensure consistent results across runs:
- Dataset generation: `random_state=1`, `random_state=42`, `seed=0`

### Environment
Tested with:
- Python 3.8+
- NumPy 1.21+
- scikit-learn 0.24+
- Matplotlib 3.3+

### Expected Behavior
Each run should produce identical:
- Dataset distributions
- Model parameters
- Visualizations
- Accuracy metrics

## Troubleshooting

### Import Errors
```
ModuleNotFoundError: No module named 'sklearn'
```
**Solution:** Install scikit-learn: `pip install scikit-learn`

### Kernel Issues
If the kernel fails to start:
1. Verify Python environment: `python --version`
2. Reinstall jupyter: `pip install --upgrade jupyter`
3. Try: `jupyter notebook --debug`

### Visualization Not Showing
If plots don't appear inline:
- Ensure `%matplotlib inline` is executed (included in notebook)
- Try restarting the kernel: Kernel → Restart & Run All

### Version Conflicts
If you encounter dependency conflicts:
```bash
pip install --upgrade numpy matplotlib scikit-learn
```

Or use a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

## Key Concepts Demonstrated

- **Logistic Regression**: Probabilistic linear classifier
- **LDA (Linear Discriminant Analysis)**: Assumes classes share covariance structure
- **QDA (Quadratic Discriminant Analysis)**: Allows different covariance per class
- **Decision Boundaries**: Geometric interpretation of classifiers
- **Covariance Structures**: Isotropic, shared, and class-specific covariances
- **Performance Metrics**: Accuracy, confusion matrices, error types

## Learning Outcomes

After exploring this notebook, you will understand:

1. How logistic regression forms linear decision boundaries
2. The geometric difference between LDA (linear) and QDA (quadratic) boundaries
3. When to choose LDA vs QDA based on data covariance structure
4. How to interpret confusion matrices and classification errors
5. The importance of data distribution assumptions in classifier selection

## License

This project is available for educational and portfolio purposes.

## Author

Ramin Yazdani

## Contributing

This is a portfolio/educational project. Feel free to fork and adapt for your own learning purposes.

---

**Tags:** machine-learning, classification, logistic-regression, lda, qda, discriminant-analysis, data-visualization, scikit-learn, jupyter-notebook, decision-boundaries, supervised-learning
