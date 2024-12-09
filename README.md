# Optimized Event Camera Feature Tracking Pipeline

This is a condensed version of the pipeline for noise robustness testing.

```mermaid
graph TD;
    A[Dataset] --> B[Data Augmentation]
    B --> C[Gaussian and Salt-and-Pepper Noise]
    C --> D[Affine Transformations]
    D --> E[Data Preparation]
    E --> F[Model Training]
    F --> G[Baseline and Noise-Robust Models]
    G --> H[Evaluation]
    H --> I[Feature Age & Error Metrics]
    I --> J[Post-Processing]
    J --> K[Final Deliverables]
