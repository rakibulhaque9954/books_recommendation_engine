# books_recommendation_engine

flowchart TD
    A[Start]
    B[Data Collection<br>(Book-Crossing, Goodreads, Amazon Reviews)]
    C[Data Preprocessing & Cleaning]
    D[Data Splitting (Train/Test)]
    E[Offline Model Training<br>(Collaborative Filtering, Matrix Factorization)]
    F[Model Evaluation<br>(RMSE, Precision, Recall)]
    G[Deploy Model via API<br>(Flask/FastAPI)]
    H[User Receives Recommendations]

    I[Real-Time Pipeline Setup]
    J[Streaming Ingestion<br>(Kafka)]
    K[Real-Time Consumer Processing]
    L[Incremental Model Updates<br>(Online Learning)]
    M[Hybrid Recommendation Update]

    A --> B
    B --> C
    C --> D
    D --> E
    E --> F
    F --> G
    G --> H

    F --> I
    I --> J
    J --> K
    K --> L
    L --> M
    M --> G
