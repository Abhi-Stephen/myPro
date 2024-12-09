# Project Pipeline with Methodology

```mermaid
graph TD;
    A[Data Collection] --> B[Data Augmentation]
    B --> C[Gaussian Noise, Salt-and-Pepper Noise, Affine Transformations]
    C --> D[Data Preparation]
    D --> E[Normalization, Event Frame Processing]
    E --> F[Model Training]
    F --> G[Baseline Model, Noise-Robust Model]
    G --> H[Evaluation]
    H --> I[Feature Age, Expected Feature Age, Error Metrics]
    I --> J[Post-Processing]
    J --> K[Visualization, Checkpoints]
    K --> L[Final Deliverables]
    L --> M[Augmented Dataset, Trained Model, Evaluation Report, Code Documentation]

    %% Methodology Section
    A1[Methodology] --> B1[Data Augmentation: Add Gaussian Noise and Salt-and-Pepper Noise (10%) to Frames]
    B1 --> C1[Apply Affine Transformations: Rotation, Translation, Scaling]
    C1 --> D1[Model Training: Baseline on Clean Data, Fine-tune with Noisy Data]
    D1 --> E1[Use Truncated Loss Function to Mitigate Noise Impact]
    E1 --> F1[Evaluate Model Using Feature Age, Expected Feature Age]
    F1 --> G1[Compare Performance with Baseline Model Without Noise-Augmented Data]

    %% Connecting Methodology to Pipeline
    A --> A1
    B --> B1
    F --> D1
    H --> F1
    L --> G1
