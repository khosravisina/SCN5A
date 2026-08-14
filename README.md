# SCN5A
 ## 🧪 Folder 1: `dataset - feature calculation`

This folder handles everything from **raw data to processed features**.

- **`data/raw/`**: Contains the original CSV files downloaded from ChEMBL and the herbal dataset. 
- **`data/processed/`**: Includes data after preprocessing:
  - Removal of rows with invalid (`NaN`) IC50 values.
  - Separation of unique vs. duplicated entries for further inspection.
  - Final feature-ready dataset (`df_for_calculate_feature.csv`).
- **`notebooks/`**: Step-by-step Python notebooks for:
  1. Downloading data (`download data.ipynb`).
  2. Exploring the herbal dataset (`herbal-dataset.ipynb`).
  3. Calculating molecular descriptors and features for both ChEMBL and herbal datasets (`calculation-feature for chembl data.ipynb` & `calculation-feature-for herbal dataset.ipynb`).

---

## 🤖 Folder 2: `Models`

This folder is dedicated to **training predictive models** using the engineered features.

- **`xgboost-model.ipynb`**: Implements an XGBoost classifier with hyperparameter tuning.
- **`lightboost model.ipynb`**: Implements a LightGBM model.
