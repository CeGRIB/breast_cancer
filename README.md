# Breast Cancer pIC50 Prediction Web App

![App Logo](logo/logo.png)


```markdown
## Overview

A Streamlit web application that predicts pIC50 values for compounds targeting breast cancer proteins using machine learning models trained on ChEMBL bioactivity data.

## Features

- 🎯 Target-specific predictions for 20+ breast cancer proteins
- 🧪 Models trained on experimental data from ChEMBL database
- 🖥️ Simple CSV input with SMILES strings
- 📊 Instant predictions with downloadable results
- 🚀 Powered by CatBoost and RDKit

## Live Demo

[![Streamlit App](https://breast-cancer-pic50.streamlit.app/)]

## Installation

```bash
git clone https://github.com/yourusername/breast-cancer-pic50-predictor.git
cd breast-cancer-pic50-predictor
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements.txt
```

## Usage

1. Run the app:
```bash
streamlit run app.py
```

2. In the app:
- Select target protein
- Upload CSV with SMILES strings
- View/download predictions

### Input Format
```csv
name,SMILES
Compound1,CN1C=NC2=C1C(=O)N(C(=O)N2C)C
Compound2,CC(=O)OC1=CC=CC=C1C(=O)O
```

[Sample Input File](https://example.com/sample.csv)

## Model Performance

| Target  | R²    | RMSE |
|---------|-------|------|
| ER      | 0.87  | 0.45 |
| HER2    | 0.85  | 0.48 |
| AKT     | 0.82  | 0.51 |

## File Structure

```
├── app.py                # Main application
├── requirements.txt      # Dependencies
├── models/               # Pretrained models
├── notebooks/            # Training notebooks
└── images/               # App visuals
```

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Open a pull request

## License

MIT License

## Contact

Afolabi Owoloye - [@afolabiowoloye](https://github.com/afolabiowoloye)
