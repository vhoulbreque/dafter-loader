---
layout: default
title: How to use dafter
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

## Use dafter

To download a dataset, say the `mnist` dataset, do:
```
dafter get mnist
```

To delete a dataset from the downloaded datasets, do:
```
dafter delete mnist
```

To search among available datasets:
```bash
# Search datasets available for download
dafter search
```

```bash
# Search datasets available for download that have the tags "image" and "deep-learning"
# and whose name contains "mni"
dafter search mni --tags image deep-learning
```

To list already downloaded datasets:
```bash
# Lists already downloaded datasets
dafter list
```

```bash
# Lists already downloaded datasets that have the tag "twitter" and whose name contains "sentiment"
dafter list sentiment --tags twitter
```
