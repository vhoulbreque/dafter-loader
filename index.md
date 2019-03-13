---
layout: default
title: Home
nav_order: 1
description: "Load and Download datasets with no effort."
permalink: /
---

# Focus on building good models
{: .fs-9 }

### Ancient times

Before dafter, you used to spend several hours finding the right dataset that you needed. Sometimes, it's after several days that you found it. And when you finally did find it, you noticed that the header of the first csv file was missing and that the extension was wrong..
It was a nightmare.

### Now

With dafter, things are getting better because you just need to do this:

```bash
dafter get mnist
```

and dafter takes care of downloading and formatting the dataset so that you can spend hours **building models** instead of looking for datasets. Then, you just go on the [MNIST page](https://vinzeebreak.github.io/dafter-loader/docs/mnist/) to copy/paste the code needed to load and use the dataset in any script.
Easy!

{: .fs-6 .fw-300 }

## Install dafter

To install dafter, just do:
```bash
curl https://raw.githubusercontent.com/vinzeebreak/dafter-install/master/install.sh -sSf | bash -s -- --up-to-date
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

To search for the available datasets with particular tags, say `image` and `deep-learning`, do:
```
dafter search image deep-learning
```

To list all the downloaded datasets do:
```
dafter list
```

## Uninstall dafter

There are 2 ways of uninstalling dafter,

```
dafter uninstall
# or
curl https://raw.githubusercontent.com/vinzeebreak/dafter-install/master/uninstall.sh -sSf | bash
```

## Contributing

To contribute, there are 2 main repositories:  

For the command line interface:  
  [View dafter on GitHub](https://github.com/vinzeebreak/dafter){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }

For this website:  
  [View this website on GitHub](https://github.com/vinzeebreak/dafter-loader){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }

---
