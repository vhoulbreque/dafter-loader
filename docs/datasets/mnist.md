---
layout: default
title: MNIST
parent: Datasets
nav_order: 2
---

# {{ page.title }}
{: .no_toc }

{: .fs-6 .fw-300 }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Download {{ page.title }}

```
dafter get mnist
```

## Load {{ page.title }}

#### Python 3

```python
import os
import gzip
import pickle

DATA_FOLDER = os.path.join(os.path.expanduser("~"), ".dafter", "mnist")
DATASET_PATH = os.path.join(DATA_FOLDER, "mnist.pkl.gz")

with gzip.open(DATASET_PATH, "rb") as f:
    train_set, valid_set, test_set = pickle.load(f, encoding='latin1')
```

#### Python 2

```python
import os
import gzip
import numpy
import pickle

DATA_FOLDER = os.path.join(os.path.expanduser("~"), ".dafter", "mnist")
DATASET_PATH = os.path.join(DATA_FOLDER, "mnist.pkl.gz")

with gzip.open(DATASET_PATH, 'rb') as f:
    train_set, valid_set, test_set = pickle.load(f)
```


## Description

The MNIST database of handwritten digits, has a training set of 60,000 examples, and a test set of 10,000 examples. It is a subset of a larger set available from NIST. The digits have been size-normalized and centered in a fixed-size image.  
It is a good database for people who want to try learning techniques and pattern recognition methods on real-world data while spending minimal efforts on preprocessing and formatting.

## Citations

Yann LeCun, Courant Institute, NYU  
Corinna Cortes, Google Labs, New York  
Christopher J.C. Burges, Microsoft Research, Redmond.  
