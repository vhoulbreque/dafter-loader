---
layout: default
title: Home
nav_order: 1
description: "Load and Download datasets with no effort."
permalink: /
---

# Focus on building good models
{: .fs-9 }

Dafter is a homebrew-like dataset downloader.
{: .fs-6 .fw-300 }

Before **dafter**, you used to spend hours looking for the perfect dataset that you needed. And when you finally found it, you noticed that the header of the first *csv* file was missing and that the extension was wrong..  

With **dafter**, things are getting better because now, you just need to do this:

```bash
dafter get mnist  # Example with the MNIST dataset
```

and **dafter** takes care of downloading and formatting the dataset's files so that you can spend hours **building models** instead of looking for datasets and their urls. Then, you just go on the [MNIST page](https://vinzeebreak.github.io/dafter-loader/docs/mnist/) to copy/paste the code needed to load and use the dataset in any script.
Easy!

{: .fs-6 .fw-300 }

## Install dafter

To install **dafter**, just do:
```bash
curl https://raw.githubusercontent.com/vinzeebreak/dafter-install/master/install.sh -sSf | bash
```

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

## Uninstall dafter

There are 2 ways of uninstalling **dafter**,

```
dafter uninstall
# or
curl https://raw.githubusercontent.com/vinzeebreak/dafter-install/master/uninstall.sh -sSf | bash
```

## Contributing

[View dafter on GitHub](https://github.com/vinzeebreak/dafter){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }

---
