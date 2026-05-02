# KDDCUP2015 MOOC Dataset

This folder contains the KDDCUP2015 MOOC dataset used in this study for MOOC dropout prediction and learning behavior analysis.

The dataset is organized into training and testing subsets. Each subset contains the original CSV files required for constructing learner behavioral features and dropout labels.

## Folder Structure

```text
KDDCUP2015data/
├── train/
│   ├── enrollment_train.csv
│   ├── log_train.csv
│   ├── truth_train.csv
│   ├── object.csv
│   └── date.csv
│
└── test/
    ├── enrollment_test.csv
    ├── log_test.csv
    ├── truth_test.csv
    ├── object.csv
    └── date.csv
