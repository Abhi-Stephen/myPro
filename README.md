# Optimized Horizontal Event Camera Feature Tracking Pipeline

```mermaid
graph LR;
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
