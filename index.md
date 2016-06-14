---
layout: default
title: the cloudyr project
---

Welcome to **the cloudyr project**! The goal of this initiative is to make cloud computing with R easier, starting with robust tools for working with cloud computing platforms. The project's inital work is with Amazon Web Services, various crowdsourcing platforms, and popular continuous integration services for R package development. Tools for Google Cloud Services and Microsoft Azure are also on the long-term agenda.

The motivation for the project is simple: cloud computing is a critical component of contemporary software development and data analysis. The reasons for this are numerous (e.g., speed, memory, storage capacity, parallel computing, etc.) and need not be rehashed here. Yet R does not currently have many tools for engaging in cloud computing. There are many tools for extracting data from the cloud (see [the Web Technologies Task View](http://cran.r-project.org/web/views/WebTechnologies.html)), but there are not very many tools for connecting a local R instance to cloud-based services.

Simply, the goal of the cloudyr project is to make cloud computing faster, easier, and more intuitive for R users through a unified cloud computing interface.

Indeed, the project's motto is simple: *make R cloudier!*

## current cloudyr packages ##

The project is [developing many packages](packages/index.html). As they are released, these packages are hosted in [a drat repository](https://github.com/eddelbuettel/drat) on this website (specifically: [http://cloudyr.github.io/drat](http://cloudyr.github.io/drat)) and versions are updated daily and are periodically released to CRAN. This means you can install and upgrade cloudyr packages quite simply directly from R:

```R
if (!require("drat")) {
    install.packages("drat")
}
drat::addRepo("cloudyr", "http://cloudyr.github.io/drat")
install.packages("NameOfPackage")
```

To make this even easier, you can add `drat::addRepo("cloudyr", "http://cloudyr.github.io/drat")` to your `.Rprofile` or `Rprofile.site` file, so that the cloudyr repository is available every time you open R.

See [the packages page](packages/index.html) for a complete list of what we've been working on.

To contribute your own project to the cloudyr project sutie, see [the contributing page](contributing/).

## recent news ##

You can follow the cloudyr project's work on [GitHub](https://github.com/cloudyr) and on [Twitter](https://github.com/cloudyRproject).

<a class="twitter-timeline" href="https://twitter.com/cloudyRproject" data-widget-id="735114108811550721">Tweets by @cloudyRproject</a>
<script>!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0],p=/^http:/.test(d.location)?'http':'https';if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src=p+"://platform.twitter.com/widgets.js";fjs.parentNode.insertBefore(js,fjs);}}(document,"script","twitter-wjs");</script>
