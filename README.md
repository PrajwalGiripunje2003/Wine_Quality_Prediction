# Wine Quality Prediction

Exploration and baseline modeling of red wine quality data. The project currently centers on a single Jupyter notebook performing: data loading, cleaning (duplicate removal), exploratory data analysis (EDA) with histograms and correlation heatmap, and simple feature selection. It is prepared with standard project scaffolding for publication on GitHub.

## Project Structure
```
wine-quality-project/
├── Wine Quality Prediction Final-checkpoint.ipynb   # Main analysis notebook
├── requirements.txt                                 # Python dependencies
├── .gitignore                                       # Ignore rules
├── LICENSE                                          # MIT License
└── README.md                                        # Project documentation
```

## Dataset
Expected file: `winequality-red.csv` in the repository root (rename if needed). Download the red wine quality dataset (commonly from UCI Machine Learning Repository) and place it alongside the notebook. Update the notebook path accordingly, e.g.:
```python
import pandas as pd
df = pd.read_csv("winequality-red.csv")
```

## Installation
Use a virtual environment (Windows PowerShell shown):
```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
```

## Usage
Launch Jupyter and open the notebook:
```powershell
jupyter notebook "Wine Quality Prediction Final-checkpoint.ipynb"
```
Recommended first cell (add if missing) to ensure imports are explicit:
```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

## Modeling Steps (Current Notebook)
- Load dataset and preview shape/head.
- Inspect info(), nulls, duplicates; remove duplicate rows.
- Univariate distribution plots (`hist`).
- Correlation heatmap using `sns.heatmap` over numeric columns.
- Simple feature subset creation for exploratory predictors.
- Quality distribution visualization (`countplot`).


## License
Released under the MIT License. See `LICENSE` for details.

## Citation / Acknowledgment
If you use the UCI dataset, cite the source: P. Cortez et al., Modeling wine preferences using physicochemical properties.

## Contributing
Open an issue or submit a pull request. (You can create `CONTRIBUTING.md` later to formalize guidelines.)

---
Feel free to request script creation, CI setup, or additional documentation and they can be added.

