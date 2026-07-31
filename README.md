# Vitiligo vs Unknown — Skin Image Classifier

GET 324 (Cloud Computing and AI Model Deployment for Engineering Applications) —
Laboratory Exercise 10 Mini-Project.

## Overview
A Convolutional Neural Network (MobileNetV2 transfer learning) that performs binary
image classification of dermatology images into **Vitiligo** or **Unknown**
(non-vitiligo skin), deployed as an interactive Streamlit web application.

## Dataset
Real (non-synthetic) dermatology images — Kaggle "Vitiligo" dataset by `shinynose`
(https://www.kaggle.com/datasets/shinynose/vitiligo), 3,628 images across two classes
(Vitiligo, Healthy). "Healthy" is relabeled **Unknown** for this assignment's binary
naming convention. Used strictly for educational purposes.

## Repository contents
| File | Purpose |
|---|---|
| `GET324_Vitiligo_vs_Unknown.ipynb` | Full pipeline: data prep, training, evaluation |
| `app.py` | Streamlit application source code |
| `requirements.txt` | Python dependencies for deployment |
| `vitiligo_classifier.keras` | Trained model weights |
| `class_names.json` | Class index → label mapping |
| `REPORT.md` | Brief project report (100-150 words) |

## Running locally
```bash
pip install -r requirements.txt
streamlit run app.py
```

## Deployment
Deployed on Streamlit Community Cloud: **`<PASTE YOUR DEPLOYED APP URL HERE>`**

To redeploy: push this repo to GitHub, then on https://share.streamlit.io choose
**New app**, select this repository/branch, set the main file to `app.py`, and deploy.

## Team
| Name | Registration Number | GitHub Username |
|---|---|---|
| DANIEL INYANG JOHN | 22/EG/AE/817 | leinadinhoj-max |
| GYUBOK ISAAC ISHAKU | 22/EG/AE/777 | isaac-gyubok-22-777|
| BASSEY SAMUEL BONIFACE | 22/EG/AE/787 | samuel-bassey-22-787 |
| GODFREY VICTOR OKON | 22/EG/AE/797 | godfrey-okon-22-797 |
| AKPAN VICTOR OKON | 23/EG/AE/027 | Victor-Akpan-23-027 |
| ISONG GIDEON EMMANUEL | 23/EG/AE/037 | Gideon-Isong-23-037 |
| AKANAM SHADRACH OSUNG | 22/EG/AE/807 | shadrach-akanam-22-807 |
| WISDOM ANIEDI BASSEY | 23/EG/AE/007 | wisdomsmart123 |
| EZE CHIOMA ORJI  | 23/EG/AE/017 | Eze-Chioma-23-017 |
| BLESSING JOSEPH GEORGE | 22/EG/AE/827 | genialsjoseph204-collab |

## Disclaimer
Built for an academic engineering exercise only. Not a validated medical device and
must not be used for real clinical decisions.
