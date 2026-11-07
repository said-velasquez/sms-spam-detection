# SMS Spam Detection

A spam filter for SMS messages built with scikit-learn. It turns 5,572 messages into Bag-of-Words features, compares Multinomial Naive Bayes with Logistic Regression, and studies the errors of the best model with a confusion matrix.

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikitlearn&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?logo=pandas&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?logo=jupyter&logoColor=white)

## Results

Multinomial Naive Bayes was the best model, with **98% accuracy** on 1,115 test messages.

| Class | Precision | Recall | F1-score |
|---|---|---|---|
| Ham | 0.99 | 0.99 | 0.99 |
| Spam | 0.96 | 0.92 | 0.94 |

Out of 1,115 test messages, only 6 legitimate messages were flagged as spam and 12 spam messages got through.

## Project structure

```
sms-spam-detection/
├── notebooks/
│   └── sms_spam_detection.ipynb
├── data/
│   └── README.md        # how to get the dataset
├── requirements.txt
└── LICENSE
```

## Run it

```bash
git clone https://github.com/said-velasquez/sms-spam-detection.git
cd sms-spam-detection
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook
```

Download the dataset first and put `spam.csv` in `data/` (see [`data/README.md`](data/README.md)).

## Tech stack

Python, pandas, scikit-learn, Matplotlib, Seaborn, Jupyter.

## Author

**Said Velásquez**, Computer Engineering student based in Madrid.
[LinkedIn](https://www.linkedin.com/in/said-vel%C3%A1squez-650905333) · [GitHub](https://github.com/said-velasquez)
