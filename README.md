```mermaid
graph LR;
    A[Data Collection] --> B[Data Augmentation (Gaussian, Salt-and-Pepper Noise, Affine Transforms)]
    B --> C[Data Preparation (Normalization, Event Frame Processing)]
    C --> D[Model Training (Baseline & Noise-Robust Model)]
    D --> E[Evaluation (Feature Age, Expected Feature Age, Error Metrics)]
    E --> F[Post-Processing (Visualization, Checkpoints)]
    F --> G[Final Deliverables (Augmented Dataset, Trained Model, Evaluation Report)]
