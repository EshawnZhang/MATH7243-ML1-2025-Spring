# Multi-window CNN for Cerebral Hemorrhage Staging (MATH 7243 Project)

This repo contains Jupyter notebooks for a **multi-window CT** pipeline and a custom **CNN** to perform **6-class** cerebral hemorrhage staging (course: Machine Learning I, MATH 7243).

## Authors
- Yixiao Zhang(zhang.yixiao1@northeastern.edu)
- Yunlong Jiao(jiao.yunl@northeastern.edu)

## Contents
- `Prepare test.ipynb` – data loading & preprocessing (multi-window CT assembled as 4-channel inputs).
- `Improve test.ipynb` – training experiments and regularization (e.g., dropout tuning).
- `Formal test.ipynb` – final configuration and evaluation.

> Note: This repository does **not** include any data. The dataset used in this project was provided by **Zeta Surgical** to **Northeastern University** solely for educational use under a course/educational arrangement. Redistribution or public release of the dataset (in whole or in part), including derived raw files, original DICOM/PNG/JPG/NPY/CSV, model checkpoints trained on the dataset, and any metadata that could reveal protected health information (PHI), is **strictly prohibited** by the applicable Data Use Agreement (DUA) and institutional policies.

## Environment
```bash
# Python 3.9+ recommended
pip install -r requirements.txt
```

## Quick Start
1. Launch Jupyter:
   ```bash
   jupyter lab
   ```
2. Open notebooks in this order:
   - `Prepare test.ipynb`
   - `Improve test.ipynb`
   - `Formal test.ipynb`
3. Edit dataset paths where necessary and run cells top-to-bottom.

## Results
- 6-class classification with test accuracy ~**0.50** in our course experiments (vs. random baseline 0.167).
- Stable train/validation learning curves after increasing sample from 10%→20% and tuning dropout to **p=0.25**.

## Citation
If you use or reference this project, please cite as:
```
Zhang, Y. (2025). Multi-window CNN study for automatic cerebral hemorrhage staging (Course Project, MATH 7243).
```

## License
MIT
