---
layout: default
title: the cloudyr project
---

Welcome to **the cloudyr project**! The goal of this initiative is to make cloud computing with R easier, starting with robust tools for working with cloud computing platforms. The project's inital work is with Amazon Web Services, various crowdsourcing platforms, and popular continuous integration services for R package development. Tools for Google Cloud Services and Microsoft Azure are also on the long-term agenda.

The motivation for the project is simple: cloud computing is a critical component of contemporary software development and data analysis. The reasons for this are numerous (e.g., speed, memory, storage capacity, parallel computing, etc.) and need not be rehashed here. Yet R does not currently have many tools for engaging in cloud computing. There are many tools for extracting data from the cloud (see [the Web Technologies Task View](http://cran.r-project.org/web/views/WebTechnologies.html)), but there are not very many tools for connecting a local R instance to cloud-based services.

This is unfortunate given the growing popularity of R and the fact that cloud providers often make software development kits available for numerous languages (such as Java, Python, Ruby, etc.). As an example, boto provides an incredibly robust framework for developing cloud computing applications in Python. R is currently underserved in by AWS software development kits and there are only a few disjointed third-party packages. Aiming to fill this void, the goal of the cloudyr project is to make cloud computing faster, easier, and more intuitive for R users through a unified cloud computing interface.

Indeed, the project's motto is simple: *Make R Cloudier!*

## Current cloudyr Packages ##

The project is developing the following packages so far, with the goal to wrap all AWS APIs in the near future.

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

You can also install packages between releases using devtools:

```R
if(!require("devtools")) {
    install.packages("devtools")
    library("devtools")
}
install_github("cloudyr/NameOfPackage")
```

Here's what we're working on so far:

| Category | Package | Service | Available From drat | On CRAN | 
|----------|---------|---------|---------------------|---------|
| Storage  | [aws.s3](http://github.com/cloudyr/aws.s3) | Simple Storage Service | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.s3)](http://cran.rstudio.com/package=aws.s3) |
| | [aws.glacier](http://github.com/cloudyr/aws.glacier) | Glacier | No | [![CRAN](http://www.r-pkg.org/badges/version/aws.glacier)](http://cran.rstudio.com/package=aws.glacier) |
| Infrastructure | [aws.ses](http://github.com/cloudyr/aws.ses) | Simple Email Service | No | [![CRAN](http://www.r-pkg.org/badges/version/aws.ses)](http://cran.rstudio.com/package=aws.ses) |
| | [aws.sns](http://github.com/cloudyr/aws.sns) | Simple Notification Service | No | [![CRAN](http://www.r-pkg.org/badges/version/aws.sns)](http://cran.rstudio.com/package=aws.sns) |
| | [aws.sqs](http://github.com/cloudyr/aws.sqs) | Simple Queue Service | No | [![CRAN](http://www.r-pkg.org/badges/version/aws.sqs)](http://cran.rstudio.com/package=aws.sqs) |
| Computing | [aws.ec2](http://github.com/cloudyr/aws.ec2) | EC2 | No | [![CRAN](http://www.r-pkg.org/badges/version/aws.ec2)](http://cran.rstudio.com/package=aws.ec2) |
| Administration | [aws.iam](http://github.com/cloudyr/aws.iam) | Identity and Access Management | No | [![CRAN](http://www.r-pkg.org/badges/version/aws.iam)](http://cran.rstudio.com/package=aws.iam) |
| | [aws.cloudtrail](http://github.com/cloudyr/aws.cloudtrail) | Cloudtrail | No | [![CRAN](http://www.r-pkg.org/badges/version/aws.cloudtrail)](http://cran.rstudio.com/package=aws.cloudtrail) |
| | [aws.cloudwatch](http://github.com/cloudyr/aws.cloudwatch) | Cloudwatch | No | [![CRAN](http://www.r-pkg.org/badges/version/aws.cloudwatch)](http://cran.rstudio.com/package=aws.cloudwatch) |
| | [aws.signature](http://github.com/cloudyr/aws.signature) | Computes AWS Signature Version 4  | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.signature)](http://cran.rstudio.com/package=aws.signature) |
| Crowdsourcing | [MTurkR](http://github.com/leeper/MTurkR) | Amazon Mechanical Turk | Yes | [![CRAN](http://www.r-pkg.org/badges/version/MTurkR)](http://cran.rstudio.com/package=MTurkR) |
| | [crowdflower](http://github.com/cloudyr/crowdflower) | Crowdflower | No | [![CRAN](http://www.r-pkg.org/badges/version/crowdflower)](http://cran.rstudio.com/package=crowdflower) |
| | [microworkers](http://github.com/cloudyr/microworkers) | Microworkers | No | [![CRAN](http://www.r-pkg.org/badges/version/microworkers)](http://cran.rstudio.com/package=microworkers) |
| Package Development | [travisci](http://github.com/cloudyr/travisci) | Travis-CI API Client  | Yes | [![CRAN](http://www.r-pkg.org/badges/version/travisci)](http://cran.rstudio.com/package=travisci) |
|  | [appveyor](http://github.com/cloudyr/appveyor) | Appveyor API Client  | No | [![CRAN](http://www.r-pkg.org/badges/version/appveyor)](http://cran.rstudio.com/package=appveyor) |
|  | [circleci](http://github.com/cloudyr/circleci) | Circle-CI API Client  | Yes | [![CRAN](http://www.r-pkg.org/badges/version/circleci)](http://cran.rstudio.com/package=circleci) |

Contributions are always welcome. Pull requests via GitHub are the preferred way to contribute code and documentation. Ideas, brainstorming, and general discussion are welcome as issues on project-specific repositories or in [cloudyr's gitter chatroom](https://gitter.im/cloudyr).

<!--
 - [aws.container](http://github.com/cloudyr/aws.container): EC2 container client
 - [aws.vpc](http://github.com/cloudyr/aws.vpc): Virtual Private Cloud client
 - [aws.emr](http://github.com/cloudyr/aws.emr): Elastic Map Reduce (Hadoop) client
 - [aws.lambda](http://github.com/cloudyr/aws.lamda): Lamda (event-driven computing) client
 - [aws.kinesis](http://github.com/cloudyr/aws.kinesis): Kinesis (data stream processing) client
 - [aws.datapipeline](http://github.com/cloudyr/aws.datapipeline): Data Pipeline (task scheduling) client
 - [aws.elb](http://github.com/cloudyr/aws.elb): Elastic Load Balancing (EC2 distribution) client
 - [aws.cf](http://github.com/cloudyr/aws.cf): CloudFormation client
-->

<!--
 - [aws.config](http://github.com/cloudyr/aws.config): Config client
-->
 
 
<!--
### Project Packages for GCS ###

 - [goog.compute]()
 - [goog.container]()
 - [goog.storage]()
-->
