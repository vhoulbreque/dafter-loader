---
layout: default
title: IMDB datasets
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

## Load {{ page.title }}

#### Python 3

```python
import os
import pandas as pd

DATA_FOLDER = os.path.join(os.path.expanduser("~"), ".dafter", "imdb-datasets")
NAME_BASIC_PATH = os.path.join(DATA_FOLDER, "imdb-datasets_0.gz")
TITLE_AKAS_PATH = os.path.join(DATA_FOLDER, "imdb-datasets_1.gz")
TITLE_BASICS_PATH = os.path.join(DATA_FOLDER, "imdb-datasets_2.gz")
TITLE_CREW_PATH = os.path.join(DATA_FOLDER, "imdb-datasets_3.gz")
TITLE_EPISODE_PATH = os.path.join(DATA_FOLDER, "imdb-datasets_4.gz")
TITLE_PRINCIPALS_PATH = os.path.join(DATA_FOLDER, "imdb-datasets_5.gz")
TITLE_RATINGS_PATH = os.path.join(DATA_FOLDER, "imdb-datasets_6.gz")

# Be careful, some of these datasets can be heavy in memory
# Add nrows=100 to load only 100 rows
df_name_basics = pd.read_csv(NAME_BASIC_PATH, compression='gzip', sep="\t")
df_title_akas = pd.read_csv(TITLE_AKAS_PATH, compression='gzip', sep="\t")
df_title_basics = pd.read_csv(TITLE_BASICS_PATH, compression='gzip', sep="\t")
df_title_crew = pd.read_csv(TITLE_CREW_PATH, compression='gzip', sep="\t")
df_title_episode = pd.read_csv(TITLE_EPISODE_PATH, compression='gzip', sep="\t")
df_title_principals = pd.read_csv(TITLE_PRINCIPALS_PATH, compression='gzip', sep="\t")
df_title_ratings = pd.read_csv(TITLE_RATINGS_PATH, compression='gzip', sep="\t")
```

#### Python 2

```python
import os
import pandas as pd

DATA_FOLDER = os.path.join(os.path.expanduser("~"), ".dafter", "imdb-datasets")
NAME_BASIC_PATH = os.path.join(DATA_FOLDER, "imdb-datasets_0.gz")
TITLE_AKAS_PATH = os.path.join(DATA_FOLDER, "imdb-datasets_1.gz")
TITLE_BASICS_PATH = os.path.join(DATA_FOLDER, "imdb-datasets_2.gz")
TITLE_CREW_PATH = os.path.join(DATA_FOLDER, "imdb-datasets_3.gz")
TITLE_EPISODE_PATH = os.path.join(DATA_FOLDER, "imdb-datasets_4.gz")
TITLE_PRINCIPALS_PATH = os.path.join(DATA_FOLDER, "imdb-datasets_5.gz")
TITLE_RATINGS_PATH = os.path.join(DATA_FOLDER, "imdb-datasets_6.gz")

# Be careful, some of these datasets can be heavy in memory
# Add nrows=100 to load only 100 rows
df_name_basics = pd.read_csv(NAME_BASIC_PATH, compression='gzip', sep="\t")
df_title_akas = pd.read_csv(TITLE_AKAS_PATH, compression='gzip', sep="\t")
df_title_basics = pd.read_csv(TITLE_BASICS_PATH, compression='gzip', sep="\t")
df_title_crew = pd.read_csv(TITLE_CREW_PATH, compression='gzip', sep="\t")
df_title_episode = pd.read_csv(TITLE_EPISODE_PATH, compression='gzip', sep="\t")
df_title_principals = pd.read_csv(TITLE_PRINCIPALS_PATH, compression='gzip', sep="\t")
df_title_ratings = pd.read_csv(TITLE_RATINGS_PATH, compression='gzip', sep="\t")
```


## Description

Each dataset is contained in a gzipped, tab-separated-values (TSV) formatted file in the UTF-8 character set. The first line in each file contains headers that describe what is in each column. A ‘\N’ is used to denote that a particular field is missing or null for that title/name.
