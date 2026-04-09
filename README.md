# hello-world-mlops update
project/
│
├── data/
│   ├── raw/                # untouched source data
│   ├── processed/          # cleaned, feature‑engineered data
│   └── external/           # third‑party datasets
│
├── notebooks/
│   ├── exploration/        # EDA, experiments
│   └── prototypes/         # early model attempts
│
├── src/
│   ├── data/               # data loading, preprocessing
│   │   ├── loaders.py
│   │   └── preprocess.py
│   │
│   ├── features/           # feature engineering
│   │   └── build_features.py
│   │
│   ├── models/             # model definitions & training
│   │   ├── train.py
│   │   ├── predict.py
│   │   └── model.py
│   │
│   ├── evaluation/         # metrics, validation, drift checks
│   │   └── evaluate.py
│   │
│   ├── serving/            # FastAPI or other inference server
│   │   ├── app.py
│   │   └── health.py
│   │
│   └── utils/              # shared helpers
│       ├── logging.py
│       └── config.py
│
├── models/
│   ├── checkpoints/        # training checkpoints
│   ├── final/              # production-ready models
│   └── metadata.json       # version, training params, metrics
│
├── configs/
│   ├── training.yaml
│   ├── model.yaml
│   └── serving.yaml
│
├── tests/
│   ├── unit/
│   └── integration/
│
├── scripts/
│   ├── train.sh
│   ├── evaluate.sh
│   └── deploy.sh
│
├── infra/
│   ├── docker/
│   │   └── Dockerfile
│   ├── k8s/
│   │   ├── deployment.yaml
│   │   ├── service.yaml
│   │   └── scaledobject.yaml
│   └── terraform/          # optional
│
├── requirements.txt
├── pyproject.toml          # optional
├── README.md
└── .gitignore
