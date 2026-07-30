# Budget-Aware Machine Learning Preprocessing

This repository contains an industry-facing white paper based on my doctoral research at the University of Maryland's Robert H. Smith School of Business.

The research studies how data preprocessing choices affect machine learning pipeline performance and how preprocessing effort can be made visible, measurable, and comparable.

## Core Idea

Data preprocessing is often treated as background setup work. In practice, choices such as imputation, encoding, scaling, feature selection, and dimensionality reduction can materially affect model performance.

This work proposes a budget-aware framework that treats preprocessing choices as searchable machine learning pipeline parameters, similar to hyperparameters.

## Research Design

The study compares three search regimes:

1. Data preprocessing only
2. Hyperparameter optimization only
3. Joint data preprocessing and hyperparameter optimization

The empirical study uses:

- 3 real-world datasets: Airbnb, Kickstarter, and Yelp
- 30 supervised prediction tasks
- Classification and regression settings
- Approximately 3.6 million trained candidate machine learning pipelines
- Budget-based evaluation using efficiency curves and validation-selected incumbents

## Main Findings

- Joint preprocessing and hyperparameter search generally provides stronger performance across the search budget.
- Preprocessing and hyperparameter choices are interdependent.
- Isolated conclusions about which preprocessing or tuning choices matter often change under joint search.
- Broad preprocessing patterns transfer more reliably than exact pipeline recipes.
- Preprocessing knowledge transfers more reliably within related datasets than across unrelated datasets.

## Industry Implications

Organizations building predictive machine learning systems should:

- Track preprocessing effort alongside model-tuning effort.
- Compare pipeline performance across compute budgets, not only final best scores.
- Treat preprocessing defaults as hypotheses rather than universal best practices.
- Optimize preprocessing and model choices jointly when resources permit.
- Revalidate preprocessing decisions when datasets, targets, or deployment settings change.

## White Paper

[Download the white paper](whitepaper/Aseem_Baji_Budget_Aware_ML_Preprocessing_White_Paper.pdf)

## Status

This repository summarizes ongoing doctoral research. The full academic manuscript and experimental code are not currently public because the work is being prepared for journal submission.

## Author

Aseem Baji  
PhD Candidate, Information Systems  
Robert H. Smith School of Business  
University of Maryland  
LinkedIn: https://www.linkedin.com/in/aseem-baji-07237211b/
