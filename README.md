# Analyzing Cain’s Jawbone With Artificial Intelligence

## Description

This project aims to study the usefulness of analyzing Cain’s Jawbone with Artificial Intelligence. Note that this is a work in progress. 

*Cain’s Jawbone, a Torquemada Mystery Novel*, is a mystery puzzle by Edward Powys Mathers (1892 – 1939). It was initially published in 1934 (Victor Gollancz, Ltd) and was reprinted in 2019 (Unbound).

This puzzle consists of 100 shuffled pages. This puzzle is solved by correctly ordering them using clues from the text. Only one solution exists and has yet to be officially made public.

We suggest a solution [here](https://glthr.com/cj/). This unofficial solution has been done almost entirely manually (we just developed a tool to detect hidden quotes to assist with this process).

## Data

- `jawbone.json` corpus from original edition (in the public domain)
- `unofficial_solution.json` contains the solution suggested [here](https://glthr.com/cj/)

## Install

Install the dependencies:

```
python3 -m venv venv
source venv/bin/activate 
pip3 install -r requirements.txt
jupyter notebook
```

## Run

* K-means preliminary analysis: `1_k-means.ipynb`
* Binary Classification (Bill Hardy) using BERT: `2_BERT_binary_classification_bill.ipynb`
* Multiclass Classification using BERT: `3_BERT_multiclass_classification.ipynb`
* Binary Classification (all narrators) using BERT: `4_BERT_binary_classification_all.ipynb`
* Assessing the Impact of Grammatical Tenses on Pages Classification: `5_Grammatical_tenses_assessment.ipynb`
