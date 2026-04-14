# CervixPredict — Cervical Cancer Survival Prediction Dashboard

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

An interactive clinical decision-support tool for individual cervical cancer survival prediction, developed as a supplementary resource for:

> **Cervical Cancer Survival in Egypt: Statistical Analysis and Machine Learning Models with Cross-Population Validation**  
> Dweep M, Soliman MM, Elhusseiny K, et al. *Cancer Medicine*, 2025 (under review).

---

## 🔗 Live Tool

[Open CervixPredict Tool](https://malaksoliman.github.io/cervixpredict)

## Model Details

| Property | Value |
|---|---|
| Algorithm | Logistic Regression |
| Training dataset | SEER (n = 74,871; 30,067 deaths) |
| External validation 1 | Egyptian cohort, n = 161, C-index = 0.81 |
| External validation 2 | TCGA, n = 275, C-index = 0.61 |
| Input features | Age, FIGO stage, histological type, tumour grade, surgery, radiation, chemotherapy |
| Imputation strategy | Median (fitted on SEER training set only) |

### Logistic Regression Coefficients (SEER-trained)

| Feature | Coefficient |
|---|---|
| Intercept | −4.402 |
| Age | +0.0431 |
| FIGO stage (numeric) | +0.660 |
| Tumour grade | +0.522 |
| Histological type | +0.039 |
| Surgery | −0.766 |
| Radiation | +0.398 |
| Chemotherapy | −0.212 |

---

## Inputs

| Input | Values |
|---|---|
| Age at diagnosis | 15–87 years |
| FIGO stage | IA, IB, IIA, IIB, IIIA, IIIB, IIIC, IVA, IVB |
| Histological type | Squamous cell carcinoma, Adenocarcinoma, Adenosquamous, Other |
| Tumour grade | Grade I, II, III |
| Surgery | Yes / No |
| Radiation therapy | Yes / No |
| Chemotherapy | Yes / No |

---

## Clinical Disclaimer

This tool is for **research and educational purposes only**. It does not constitute medical advice. All clinical decisions must be made by qualified healthcare professionals. clinical judgement should be applied accordingly.

---



## Citation

If you use this tool, please cite:

```
Dweep M, Soliman MM, Elhusseiny K, Gobran NS, Elghamry W, Abdelhafiz AS,
Mysara M, Alorabi M. Cervical Cancer Survival in Egypt: Statistical Analysis
and Machine Learning Models with Cross-Population Validation.
Cancer Medicine. 2025. doi:[DOI]
```

---

## License

MIT License — free to use and adapt with attribution.
