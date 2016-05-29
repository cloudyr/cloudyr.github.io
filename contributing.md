---
layout: default
title: the cloudyr project
---

## what the cloudyr project does ##

The cloudyr project aims to provide cloud computing functionality for R. To achieve this, the primary goal is to create new, easy-to-use packages in the following areas:

  1. Clients to manage cloud computing infrastructure. CUrrent examples of this in the cloudyr suite include [existing packages](../packages) for Amazon Web Services resources. Potential contributions could create analogous packages for Google Cloud Compute, Microsoft Azure, etc.
  2. Clients to manage cloud storage. Current examples of this in the cloudyr suite include [aws.s3](https://github.com/cloudyr/aws.s3).
  3. Clients for cloud-based package development and testing. Current examples in the cloudyr suite include [travisci](https://github.com/cloudyr/travisci).
  4. Packages to create and retrieve data from online survey and experimental platforms. Current examples include [Rmonkey](https://github.com/cloudyr/Rmonkey).
  5. Packages to manage human crowdsourcing tasks. Current examples include [MTurkR](https://github.com/leeper/MTurkR).
  6. Any other package that aims to used cloud-based resources to perform data analysis and other computational tasks from R.
  
Some areas that are generally off-topic for the cloudyr project include those that only *retrieve* open data, such as scientific data sources or government data. These types of packages would be more appropriate for [rOpenSci](https://ropensci.org/) or [rOpenGov](http://ropengov.github.io/), respectively. Similarly, packages for managing cloud services (e.g., social media accounts) are probably outside the scope of cloudyr. Finally, packages implementing purely local procedures (e.g., statistical algorithms, etc.) without an obvious cloud-based connection are probably not a good fit for cloudyr.

## contributing to the cloudyr project ##

Contributions to the cloudyr project are welcome from everyone anywhere in the world. Contributions can be made to existing packages and in the form of new packages that fit within the scope defined above.

Contributions to existing packages are best made in the form of GitHub issues and pull requests on the respective package pages. In lieu of that, emails to the appropriate package maintainer is a fallback.

Contributions in the form of new packages are also very welcome! There is currently no formal onboarding process for packages. If you would like to contribute a package, please do the following: 

  1. Look over the parameters at the top of this page to ensure the package is within the project's scope
  2. Check [the packages page](../packages) to make sure a package doesn't already exist (and you may also want to check [the webservices task view](https://github.com/ropensci/webservices) to see if anyone else has developed a similar package.
  3. Propose the package idea via [a GitHub issue](https://github.com/cloudyr/cloudyr.github.io/issues), with links to an existing repo if you have already drafted the package.
  4. Look over [the cloudyr style guide](../styleguide) to ensure the package is generally compliant. These are not strict rules. A [template package](https://github.com/cloudyr/pkgtemplate) is available, which provides a skeleton that complies with this guide if you are starting from scratch. 

If your package is accepted, you can host it under the cloudyr project GitHub organization, while retaining full control over the code, with administration rights to a GitHub "team" for the package, so you can invite others to contribute to the package, as well. Some modifications may be made to enable continuous integration testing, branding on the package's README, and deployment to the cloudyr project [drat](../drat). The package will then listed on the cloudyr project [package page](../packages).
