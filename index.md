---
layout: default
title: the cloudyr project
---

Welcome to **the cloudyr project**! The goal of this initiative is to make cloud computing with R easier, starting with robust tools for working with cloud computing platforms. The project's inital work is with Amazon Web Services, various crowdsourcing platforms, and popular continuous integration services for R package development. Tools for Google Cloud Services and Microsoft Azure are also on the long-term agenda.

The motivation for the project is simple: cloud computing is a critical component of contemporary software development and data analysis. The reasons for this are numerous (e.g., speed, memory, storage capacity, parallel computing, etc.) and need not be rehashed here. Yet R does not currently have many tools for engaging in cloud computing. There are many tools for extracting data from the cloud (see [the Web Technologies Task View](http://cran.r-project.org/web/views/WebTechnologies.html)), but there are not very many tools for connecting a local R instance to cloud-based services.

This is unfortunate given the growing popularity of R and the fact that cloud providers often make software development kits available for numerous languages (such as Java, Python, Ruby, etc.). As an example, boto provides an incredibly robust framework for developing cloud computing applications in Python. R is currently underserved in by AWS software development kits and there are only a few disjointed third-party packages. Aiming to fill this void, the goal of the cloudyr project is to make cloud computing faster, easier, and more intuitive for R users through a unified cloud computing interface.

Indeed, the project's motto is simple: *Make R Cloudier!*

## Current cloudyr Packages ##

The project is [developing many packages](packages/index.html), especially those provided by AWS, with a goal to wrap all AWS APIs in the near future.

As they are released, these packages are hosted in [a drat repository](https://github.com/eddelbuettel/drat) on this website (specifically: [http://cloudyr.github.io/drat](http://cloudyr.github.io/drat)) and versions are updated daily and are periodically released to CRAN. This means you can install and upgrade cloudyr packages quite simply directly from R:

```R
if(!require("drat")) {
    install.packages("drat")
    library("drat")
}
addRepo("cloudyr")
install.packages("NameOfPackage")
```

To make this even easier, you can add `drat::addRepo("cloudyr")` to your `.Rprofile` or `Rprofile.site` file, so that the cloudyr repository is available every time you open R.

See [the packages page](packages/index.html) for a complete list of what we've been working on.
