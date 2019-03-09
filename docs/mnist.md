---
layout: default
title: Mnist
nav_order: 2
---

# MNIST
{: .no_toc }

Yann LeCun, Courant Institute, NYU
Corinna Cortes, Google Labs, New York
Christopher J.C. Burges, Microsoft Research, Redmond.
The MNIST database of handwritten digits, available from this page, has a training set of 60,000 examples, and a test set of 10,000 examples. It is a subset of a larger set available from NIST. The digits have been size-normalized and centered in a fixed-size image.
It is a good database for people who want to try learning techniques and pattern recognition methods on real-world data while spending minimal efforts on preprocessing and formatting.
{: .fs-6 .fw-300 }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Load MNIST

### In Python

```python
import gzip
import pickle

from os.path import expanduser
DATASET_PATH = os.path.join(expanduser("~"), ".datasets-data-fetcher", "mnist")

with gzip.open(DATASET_PATH, "rb") as f:
    train_set, valid_set, test_set = pickle.load(f)
```
