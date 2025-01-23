# 🧠Sentiment Analysis of Product Reviews🌟(NLP)

## 🌐 Background

In the age of the Internet, the e-commerce market has seen exponential growth. A pivotal part of online shopping is the reviews that users drop on products they've purchased. These reviews, a treasure trove of data, when analyzed right, can deliver deep insights into customer satisfaction and market preferences.

A leading e-commerce company wishes to harness this data goldmine. They've amassed a plethora of product reviews and are gearing up to analyze them to enhance the service quality they deliver. This is where YOUR challenge begins.

## 🗂️ Dataset

The dataset you'll be harnessing is a modified version of an Amazon product reviews set, consisting of:

Summary: A succinct review summary penned by the user.

Text: The full-blown review content.

The Score column, representing the product rating given by the user (on a 1 to 5 scale), has been axed for this challenge. This will be the target variable your model must predict.

## 📂 Repository Structure

The repository structure is provided and must be adhered to strictly:

```markdown
nuwe-data-nlp1/
├── predictions
│   └── example_predictions.json
├── README.md
├── test
│   └── test.csv
└── train
    └── train.csv
```

## 🎯 Tasks

 Your mission, should you choose to accept it, is to craft a classification model that can predict the "rating" of a review, relying solely on its textual content. The company has made some tweaks and omissions to safeguard user privacy. Thus, they'll supply you with just two features to work on: 'Summary' and 'Text'.

## 📤 Submission Requirements

To carry out this challenge, we expect to obtain a file in json format whose name is predictions.json, where we will have as key the Test_id, from the file test/test.csv and as value the prediction of the Score column that has values ranging from 1 to 5. predictions.json:

```markdown
{
    "target": {
        "297": 1,
        "11": 5,
        "67": 1,
        "54": 3,
        "156": 2,
        "290": 2,
        "193": 4,
        ...

  }
}
```

## 📊 Evaluation

As part of our commitment to providing a clear and consistent assessment of performance, this practice will be evaluated automatically using the F1 Score metric. The evaluation process will utilize the predictions.json file, which contains your model's predictions.

The F1 Score is a widely recognized statistical measure used in classification tests, which balances precision and recall. It is especially useful in scenarios where the distribution of class labels is uneven, providing a more nuanced insight into the model's predictive power.

Your predictions will be compared against the true values to calculate the precision and recall, from which the F1 Score will be derived. The closer your F1 Score is to 1, the better your model's performance is considered in terms of both accuracy and robustness.

## CHALLENGE BY

![NUWE](/nuwe-logo.jpg)

## Solution

### Environment Setup

```bash
python -V
# Output: Python 3.12.1
```

```bash
# create a environment named -> samba-ai
python -m venv sentiment-ai
```

```bash
# activate the environment
source sentiment-ai/bin/activate
```

```bash
# deactivate the virtual environment
deactivate
```

```bash
# create a Jupyter Notebook kernel
pip install jupyter ipykernel
```

```bash
# add the virtual environment as a kernel for the jupyter notebook
python -m ipykernel install --user --name=sentiment-ai --display-name="Py3.12-sentiment-ai"
```

```bash
# verify kernel installation
jupyter kernelspec list
```

```bash
# If needed
jupyter kernelspec uninstall sentiment-ai
```

## Submitted by : Ashish Soni
