# TA_ML — Machine Learning Lab Materials

Practical notebooks and competition resources for the Machine Learning course.

---

## Labs

| Notebook | Topic | Key concepts |
|---|---|---|
| [`labs/lab1_MLE_MAP.ipynb`](labs/lab1_MLE_MAP.ipynb) | MLE & MAP | MLE = Least Squares, MAP = Ridge Regression, overfitting, basis functions |
| [`labs/lab2_Perceptron_SVM.ipynb`](labs/lab2_Perceptron_SVM.ipynb) | Perceptron & Linear SVM | Hyperplane, loss functions, Perceptron update rule, hard/soft-margin SVM, effect of C |

Each notebook contains:
- Theory recap with formulas
- Guided coding exercises (`# --- WRITE YOUR CODE HERE ---`)
- Visualizations and concept review questions

---

## Kaggle Competition

**[SVM Margin Challenge: Detect Faulty Sensors](https://www.kaggle.com/competitions/svm-margin-challenge-detect-faulty-sensors)**

Build a **linear SVM classifier** to detect whether an industrial sensor is faulty, based on 30 numerical measurements.

| | |
|---|---|
| **Task** | Binary classification — predict `faulty` (0 = normal, 1 = faulty) |
| **Metric** | Macro F1-score (balances precision and recall on both classes) |
| **Data** | 2 000 train / 2 000 test rows, 30 sensor features |
| **Allowed models** | Linear SVM only — `SVC(kernel='linear')`, `LinearSVC`, or `SGDClassifier(loss='hinge')` |
| **Submissions** | Up to 15 per day, select 2 final submissions |
| **Team size** | Individual only (1 member) |

**Tips:** Feature scaling matters (try `StandardScaler` or `RobustScaler`). Tune `C` carefully. The dataset has class imbalance, so macro F1 penalises ignoring the minority class.

> Full rules and data: see the competition page on Kaggle.
