---
layout: default
title: the cloudyr project styleguide
---

**the cloudyr project** uses a standardized style package structure and programming style to streamline development, facilitate any future package maintenance, and ease contributions from new users. This document describes the essential features of a cloudyr package.

## Package Structure ##

cloudyr packages should follow the guidelines describe in [*Writing R Extensions*](cran.r-project.org/doc/manuals/r-devel/R-exts.html) and adopt a standard package structure:

```
+-- /data
+-- /inst
|   +-- CITATION
+-- /man
+-- /R
|   +-- *.R
+-- /tests
|   +-- /testthat
|   +-- test-all.R
+-- /vignettes
+-- .gitignore
+-- .Rbuildignore
+-- .travis.yml
+-- CONTRIBUTING.md
+-- DESCRIPTION
+-- drat.sh
+-- NAMESPACE
+-- NEWS
+-- README.md
```

The `/man` directory is generated automatically by roxygen2 (via `devtools::document()`). This directory will contain all function documentation plus a package-level documentation page accessible via `? packagename`. R code files in the `/R` directory should have capital `.R` extensions and be written using complete roxygen2 markup (see below). A `/tests` directory contains relevant testthat testing code.

Optional directories include `/data` for embedded package data and `/vignettes` can be used to store knitr-enabled vignettes where appropriate.

The following sections describe some of these files in detail.

### CITATION ###

All cloudyr packages must have a `CITATION` file of the following form:

```R
citHeader("To cite package 'aws.signature' in publications use:")
     
 year <- sub(".*(2[[:digit:]]{3})-.*", "\\1", meta$Date, perl = TRUE)
 vers <- paste("R package version", meta$Version)
 
 citEntry(entry="Manual",
          title = "aws.signature: Amazon Web Services Request Signatures",
          author = personList(as.person("Thomas J. Leeper")),
          year = year,
          note = vers,
          textVersion =
          paste("Thomas J. Leeper (",
                year,
                "). aws.signature: Amazon Web Services Request Signatures. ",
                vers, ".", sep=""))
```

### Documentation ###

All package documentation should be generated dynamically with roxygen2 (via `devtools::document()`). The `NAMESPACE` file is generated automatically, as well.


### Code ###

Code should be written cleanly, using roxygen2 inline documentation, comments where appropriate, and in a manner consistent with the [Google R Style Guide](https://google.github.io/styleguide/Rguide.xml) and [Hadley's guide](http://adv-r.had.co.nz/Style.html). A few key points:

 * `<-` is preferred over `=` for assignment
 * Indentation is with four spaces, not two or a tab. There should be no tabs in code files.
 * `if () {} else {}` constructions should always use full curly braces even when usage seems unnecessary from a clarity perspective.
 * TODO statements should be opened as GitHub issues with links to specific code files and code lines, rather than written inline.
 * Follow Hadley's suggestion for aligning long functions with many arguments:

    ```
    long_function_name <- function(a = "a long argument", 
                                   b = "another argument",
                                   c = "another long argument") {
      # As usual code is indented by two spaces.
    }
    ```
 
 * Never use `print()` to send text to the console. Instead use `message()`, `warning()`, and `error()` as appropriate.
 * Use environment variables, not `options()`, to store global arguments that are used by many or all functions.
 
For packages that interact with remote websites:

 * Use **httr** for web access and implement `stop_for_status()` or `warn_for_status()` checks.
 * Packages requiring authenticated HTTP requests should have credentials encrypted in `.travis.yml` to enable Travis-CI tests.


### .gitignore and .Rbuildignore ###

A `.gitignore` may be needed to mask files in a directory. A `.Rbuildignore` should cover all non-standard files in the top-level directory:

```
.travis.yml
drat.sh
```


### Continuous Integration ###

All cloudyr packages are tested automatically on the [Travis-CI Continuous Integration service](travis-ci.org). A reasonable `.travis.yml` file would look like the following:

```
language: r
sudo: required
r_github_packages:
- cloudyr/aws.signature
- jimhester/covr
- eddelbuettel/drat
after_success:
- Rscript -e 'library(covr);codecov()'
- test $TRAVIS_PULL_REQUEST == "false" && test $TRAVIS_BRANCH == "master" && bash drat.sh
env:
  global:
  - secure: jw8SjbwUlKz/zPczyqcvnm0r9jbUvNb4hplUn3bxlD2SniNkitqODk2/jmlfunrpmHJRS4GDx6X6omYTNwvNsyE51dK6XJE8nZuaeCPvGLl3xxgRL6dis2JGwy2itRm0C/P6UEAUSmuTbtR15N1JC7Y7ot0IRpfRZc0tOkuS8L0=
```

This indicates the use of native R support, which requires sudo permissions. `r_github_packages` should be used to install working versions of packages.

Packages should have **testthat** tests and should push code coverage results to [the cloudyr codecov.io page](https://codecov.io/github/cloudyr) using the **covr** package.

The **travisci** package should be used, where needed, to automatically trigger builds of dependent cloudyr packages using:

```
after_success:
- Rscript -e "travisci::restart_last_build('cloudyr/dependentpkg')"
```

This requires an encrypted `TRAVIS_CI_TOKEN` environment variable.


### drat ###

All packages, conditional on passing CI tests, are automatically posted to the cloudyr drat repository, so that they can be installed using `install.packages()` in addition to `devtools::install_github()`. The `drat.sh` file achieves this:

```bash
#!/bin/bash
set -o errexit -o nounset
addToDrat(){
  mkdir drat; cd drat

  ## Set up Repo parameters
  git init
  git config user.name "leeper"
  git config user.email "thosjleeper@gmail.com"
  git config --global push.default simple

  ## Get drat repo
  git remote add upstream "https://$GH_TOKEN@github.com/cloudyr/cloudyr.github.io.git"
  git fetch upstream
  git checkout master

  Rscript -e "drat::insertPackage('../$PKG_TARBALL', repodir = './drat')"
  git add --all
  git commit -m "add $PKG_TARBALL (build $TRAVIS_BUILD_ID)"
  git push

}
addToDrat
```

For this code to execute successfully, a `GH_TOKEN` environment variables needs to be encrypted in the repo.


### CONTRIBUTING.md ###

A `CONTRIBUTING.md` file should be written in markdown and include a reference to this page.


### DESCRIPTION ###

There is not much to say about `DESCRIPTION` beyond that described in Writing R Extensions. However, a few points:

 * Packages should use ["semantic versioning"](http://semver.org/) (see [Hadley's discussion](http://r-pkgs.had.co.nz/description.html#version)) of the form `major.minor.patch` with values such as `1.2.3`.

### NEWS ###

A `NEWS` files should be present and be used to store three types of information:

 1. Documentation changes
 2. Bug fixes
 3. Significant user-visible changes (such as API changes)
 
This does not need to be updated on every commit, but rather on significant changes. Changes that address GitHub issues should mention the issue number and other changes should attribute code authors or bug reporters where appropriate:

```
# CHANGES TO aws.signature v0.1.1 #

 * Fixed header encoding error. (#1, h/t Thomas Leeper)

```

### README ###

A `README.md` file should be included to display on GitHub and CRAN. This should provide a package description, installation instructions, and brief code examples. This can be generated from a `README.Rmd` file using `knitr::knit("README.Rmd")`, but it is not required.

The `README` should contain the cloudyr project footer with a link to the cloudyr project page.

```
---
[![cloudyr project logo](http://i.imgur.com/JHS98Y7.png)](https://github.com/cloudyr)
```


## Programming Style ##

A few rules about programming style:

 1. Commits are cheap and should be used frequently.
 2. Commit messages should reference issue numbers and close issues explicitly (e.g., `fix headers (closes #1)`) where appropriate.
 3. Pull requests on GitHub should be merged on the command line, not using the web interface, if possible.

