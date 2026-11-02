# APTOS_2019-
# 🧠 Uncertainty-Flagged Visual-Textual Explanations for Diabetic Retinopathy Grading on APTOS 2019

## 📌 Project Overview

This project explores the classification of Diabetic Retinopathy (DR) using Deep Learning and Explainable Artificial Intelligence (XAI).

It uses retinal fundus images from the APTOS 2019 Blindness Detection dataset to classify Diabetic Retinopathy into five severity levels (0–4).

The project focuses on making AI predictions more reliable and understandable through uncertainty estimation, visual explanations, and textual explanations.

## 🎯 Project Objectives

- Classify Diabetic Retinopathy into five severity grades.
- Estimate prediction uncertainty using Monte Carlo Dropout.
- Generate visual explanations using Grad-CAM.
- Generate short textual explanations using templates.
- Evaluate the reliability of uncertainty-based referral decisions.
- Study the faithfulness and stability of AI explanations.

## 🛠️ Technologies Used

- Python
- Google Colab
- PyTorch
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- EfficientNet-B0
- Grad-CAM
- Monte Carlo Dropout

## 📊 Dataset

**APTOS 2019 Blindness Detection Dataset**

The dataset contains retinal fundus images categorized into five classes:

| Grade | Description |
|---|---|
| 0 | No DR |
| 1 | Mild |
| 2 | Moderate |
| 3 | Severe |
| 4 | Proliferative DR |

- Total graded images: 3,662
- Image size used: 224 × 224 pixels
- Default dataset source: Hugging Face (`bumbledeep/aptos`)
- Alternative source: Kaggle APTOS 2019 dataset

## 🧠 Model Architecture

**EfficientNet-B0** is used as the primary deep learning model with ImageNet pretrained weights and a dropout classification head.

The project incorporates:

1. **Monte Carlo Dropout:** Estimates uncertainty by performing multiple stochastic predictions.
2. **Grad-CAM:** Generates heatmaps to highlight important image regions.
3. **Textual Explanations:** Provides short explanations based on the regions identified by the visual explanation method.

## 🔬 Research Questions

- **RQ1:** Can uncertainty estimation identify potentially incorrect predictions and improve referral decisions?
- **RQ2:** Are visual explanations faithful and stable?
- **RQ3:** Are textual explanations faithful to the model's predictions?

## ⚙️ How to Run the Project

1. Open the notebook in Google Colab.
2. Select Runtime → Change runtime type.
3. Select T4 GPU.
4. Run the installation and setup cells.
5. Keep `PILOT = True` for the initial test.
6. Execute Runtime → Run all.
7. After successful pilot execution, change `PILOT = False` for the full study.
8. Run all cells again to generate the analysis tables and figures.

**Note:** Google Drive is used to store datasets, model checkpoints, and experiment outputs.

## 📈 Expected Outputs

- Diabetic Retinopathy classification results.
- Prediction uncertainty scores.
- Grad-CAM visualization heatmaps.
- Visual and textual explanation analysis.
- Performance and calibration tables.
- Research figures and evaluation metrics.

## ⚠️ Disclaimer

This project is developed for academic and research purposes only. It is not intended to replace professional medical diagnosis or clinical decision-making.

## 👨‍💻 Author

**Pratham Raj**

GitHub: https://github.com/prathamraj-dev

---

⭐ If you find this project interesting, feel free to explore the notebook and its implementation.
