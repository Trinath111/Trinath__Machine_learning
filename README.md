

## Depth and Width in Multilayer Perceptrons: A Study of Representational Power

This repository accompanies a machine learning tutorial investigating how architectural depth and width affect the representational power of Multilayer Perceptrons (MLPs). The project combines mathematical grounding, controlled experiments, and visual analysis to demonstrate why deeper neural networks are often more effective than shallow ones, even under comparable conditions.

The tutorial focuses on representation learning, contrasting shallow and deep MLPs with linear and feature-engineered baselines using synthetic two-dimensional classification data.

Repository Structure
.
├── notebooks/
│   └── Machine_Learning_Code.ipynb
├── figures/
│   ├── decision_boundaries.png
│   ├── learned_representations.png
│   └── confusion_matrices.png
├── tutorial/
│   └── mlp_depth_width_tutorial.pdf
├── README.md
├── LICENSE
└── requirements.txt


notebooks/: Contains the Jupyter notebook with all code used for data generation, model training, evaluation, and visualisation.

figures/: Stores figures generated programmatically by the notebook.

tutorial/: Contains the final tutorial document submitted for assessment.

requirements.txt: Lists required Python packages.

LICENSE: Specifies usage permissions for the repository.

## Tutorial Overview

The tutorial addresses the following question:

How do depth and width influence the representational power of Multilayer Perceptrons?

To answer this, the following models are compared:

Logistic Regression on raw input features

Logistic Regression with polynomial feature expansion

A shallow MLP with a single hidden layer

A deep MLP with multiple hidden layers

Performance is evaluated using classification accuracy, decision boundary visualisations, learned hidden-layer representations, and confusion matrices. All experiments are conducted under controlled conditions using a shared training–test split.

## Dataset

A synthetic two-dimensional two-moons dataset is used for all experiments. The dataset contains 1,000 samples evenly divided between two classes and is deliberately nonlinearly separable. Its low dimensionality enables direct visualisation of decision boundaries and internal representations without loss of interpretability.

The dataset is generated programmatically using scikit-learn; no external data files are required.

## How to Run the Code

Clone the repository:

git clone https://github.com/your-username/mlp-depth-width.git
cd mlp-depth-width


Install dependencies:

pip install -r requirements.txt


Launch the Jupyter notebook:

jupyter notebook notebooks/Machine_Learning_code.ipynb


Running the notebook from top to bottom will reproduce all figures and results used in the tutorial.

## Reproducibility

All experiments use a fixed random seed.

A single train–test split is shared across models.

Figures in the figures/ directory are generated directly from the notebook.

No manual parameter tuning is required to reproduce results.

## Accessibility Considerations

All plots use high-contrast, colour-blind-safe palettes.

Tables do not rely on colour to convey information.

Figures include descriptive captions and alt text in the tutorial document.

Code is organised and commented for clarity and readability.
