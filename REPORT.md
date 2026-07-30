# Brief Project Report — Vitiligo vs Unknown Classifier

**Dataset & Approach.** We used a real, publicly available dermatology dataset (Kaggle,
shinynose/vitiligo, 3,628 images) split into Vitiligo and Unknown (non-vitiligo) skin
images, with no synthetic data generated. Images were resized to 224x224, augmented
(flip, rotation, zoom, contrast), and split 70/15/15 into train/validation/test sets. A
MobileNetV2 transfer-learning CNN was trained in two phases -- frozen-base feature
extraction, then fine-tuning the top layers -- and evaluated using accuracy, precision,
recall, AUC, and a confusion matrix.

**Usage.** The app is deployed on Streamlit Cloud; users upload a skin image and receive
an instant Vitiligo/Unknown prediction with a confidence score.

**Challenges.** Class imbalance and visual overlap between vitiligo and other
hypopigmentation conditions reduced precision; we mitigated this with augmentation,
class-weighted loss, and AUC-based checkpointing. Future work: expand the dataset, add
Grad-CAM explainability, and support multi-class differential diagnosis.

(Word count target: 100-150 words -- adjust before submission.)
