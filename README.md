# Cap_stone
├── data/
├── logs/
├── src/
│   ├── parsing/
│   ├── models/
│   ├── rca/
│   └── ui/
├── notebooks/
├── config/
├── tests/
└── README.md

logs/ — Raw or Source Logs
This folder contains:
Unprocessed or original log files from systems, applications, servers, etc.
These logs are the primary input to your pipeline (for parsing, anomaly detection, etc.).
Format examples:
.log, .txt, .json
Logs from LogHub datasets like OpenStack, BGL, HDFS, etc.
logs/
├── openstack_log.log
├── hdfs_2023.log
└── custom_app_logs/
    ├── app_log_1.txt
    └── app_log_2.txt

logs/
├── anomaly_detection/
│   ├── OpenStack/
│   │   ├── log_file.txt
│   │   └── anomaly_label.csv
│
├── rca/
│   ├── OpenStack/
│   └── AIOpsChallenge/
│       ├── logs/
│       └── rca_reports/


data/ — Processed, Structured, or Intermediate Data
This folder stores:
Parsed logs in structured formats (e.g., JSON, CSV, Parquet)
Event templates, event IDs, anomaly labels
Datasets ready for model training, evaluation, or RAG indexing
Features extracted from logs

data/
├── parsed/
│   └── openstack_structured.csv
├── sequences/
│   └── log_event_sequences.npy
├── labels/
│   └── openstack_labels.json
└── embeddings/
    └── logbert_embeddings.pt
