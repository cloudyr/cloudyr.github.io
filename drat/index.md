---
layout: default
title: the cloudyr project
---

Welcome to [**the cloudyr project**](http://cloudyr.github.io/)'s drat repository! This contains the latest stable builds of all cloudyr R packages. This means you can install and upgrade cloudyr packages quite simply directly from R:

```R
if (!require("drat")) {
    install.packages("drat")
    library("drat")
}
drat::addRepo("cloudyr", "http://cloudyr.github.io/drat")
install.packages("NameOfPackage")
```

To make this even easier, you can add `drat::addRepo("cloudyr", "http://cloudyr.github.io/drat")` to your `.Rprofile` or `Rprofile.site` file, so that the cloudyr repository is available every time you open R.

See [the packages page](../packages/index.html) for a complete list of what we've been working on.
