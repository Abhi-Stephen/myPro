# Project Pipeline with Methodology

```mermaid
graph TD;
    A[Data Collection] --> B[Data Augmentation]
    B --> C[Add Gaussian and Salt-and-Pepper Noise to Frames]
    C --> D[Data Preparation]
    D --> E[Normalize and Process Event Frames]
    E --> F[Model Training]
    F --> G[Train on Clean Data, Fine-tune with Noisy Data]
    G --> H[Evaluation]
    H --> I[Measure Feature Age, Expected Feature Age]
    I --> J[Post-Processing]
    J --> K[Visualize Results and Save Checkpoints]
    K --> L[Final Deliverables]
    L --> M[Augmented Dataset, Trained Model, Evaluation Report]

    %% Methodology Section
    A1[Methodology] --> B1[Add Noise to Frames]
    B1 --> C1[Apply Affine Transformations]
    C1 --> D1[Train with Noisy Data]
    D1 --> E1[Use Truncated Loss Function]
    E1 --> F1[Evaluate Model's Robustness]
    F1 --> G1[Compare with Baseline Model]
    
    %% Connecting Methodology to Pipeline
    A --> A1
    B --> B1
    F --> D1
    H --> F1
    L --> G1
