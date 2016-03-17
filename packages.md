---
layout: default
title: the cloudyr project
---

## Current cloudyr Packages ##

Here's what we're working on so far:

| Category | Package | Service | Available From drat | On CRAN | 
|----------|---------|---------|---------------------|---------|
| Bundle | [awspack](http://github.com/cloudyr/awspack) | All Amazon Web Services | Yes | [![CRAN](http://www.r-pkg.org/badges/version/awspack)](http://cran.rstudio.com/package=awspack) |
| Storage  | [aws.s3](http://github.com/cloudyr/aws.s3) | Simple Storage Service | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.s3)](http://cran.rstudio.com/package=aws.s3) |
| | [aws.glacier](http://github.com/cloudyr/aws.glacier) | Glacier | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.glacier)](http://cran.rstudio.com/package=aws.glacier) |
| Infrastructure | [aws.ses](http://github.com/cloudyr/aws.ses) | Simple Email Service | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.ses)](http://cran.rstudio.com/package=aws.ses) |
| | [aws.sns](http://github.com/cloudyr/aws.sns) | Simple Notification Service | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.sns)](http://cran.rstudio.com/package=aws.sns) |
| | [aws.sqs](http://github.com/cloudyr/aws.sqs) | Simple Queue Service | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.sqs)](http://cran.rstudio.com/package=aws.sqs) |
| Computing | [aws.ec2](http://github.com/cloudyr/aws.ec2) | EC2 | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.ec2)](http://cran.rstudio.com/package=aws.ec2) |
| Administration | [aws.iam](http://github.com/cloudyr/aws.iam) | Identity and Access Management | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.iam)](http://cran.rstudio.com/package=aws.iam) |
| | [aws.cloudtrail](http://github.com/cloudyr/aws.cloudtrail) | Cloudtrail | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.cloudtrail)](http://cran.rstudio.com/package=aws.cloudtrail) |
| | [aws.cloudwatch](http://github.com/cloudyr/aws.cloudwatch) | Cloudwatch | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.cloudwatch)](http://cran.rstudio.com/package=aws.cloudwatch) |
| | [aws.signature](http://github.com/cloudyr/aws.signature) | Computes AWS Signature Version 4  | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.signature)](http://cran.rstudio.com/package=aws.signature) |
| Crowdsourcing | [MTurkR](http://github.com/leeper/MTurkR) | Amazon Mechanical Turk | Yes | [![CRAN](http://www.r-pkg.org/badges/version/MTurkR)](http://cran.rstudio.com/package=MTurkR) |
| | [MTurkRGUI](http://github.com/leeper/MTurkRGUI) | MTurkR GUI | Yes | [![CRAN](http://www.r-pkg.org/badges/version/MTurkRGUI)](http://cran.rstudio.com/package=MTurkRGUI) |
| | [crowdflower](http://github.com/cloudyr/crowdflower) | Crowdflower | No | [![CRAN](http://www.r-pkg.org/badges/version/crowdflower)](http://cran.rstudio.com/package=crowdflower) |
| | [microworkers](http://github.com/cloudyr/microworkers) | Microworkers | No | [![CRAN](http://www.r-pkg.org/badges/version/microworkers)](http://cran.rstudio.com/package=microworkers) |
| Web Surveys | [Rmonkey](http://github.com/cloudyr/Rmonkey) | Survey Monkey | Yes | [![CRAN](http://www.r-pkg.org/badges/version/Rmonkey)](http://cran.rstudio.com/package=Rmonkey) |
| Package Development | [travisci](http://github.com/cloudyr/travisci) | Travis-CI API Client  | Yes | [![CRAN](http://www.r-pkg.org/badges/version/travisci)](http://cran.rstudio.com/package=travisci) |
|  | [appveyor](http://github.com/cloudyr/appveyor) | Appveyor API Client  | No | [![CRAN](http://www.r-pkg.org/badges/version/appveyor)](http://cran.rstudio.com/package=appveyor) |
|  | [circleci](http://github.com/cloudyr/circleci) | Circle-CI API Client  | Yes | [![CRAN](http://www.r-pkg.org/badges/version/circleci)](http://cran.rstudio.com/package=circleci) |

Contributions are always welcome. See [the cloudyr style guide](styleguide.html) for guidance on package development, structure, and coding style. Pull requests via GitHub are the preferred way to contribute code and documentation. Ideas, brainstorming, and general discussion are welcome as issues on project-specific repositories or in [cloudyr's gitter chatroom](https://gitter.im/cloudyr).

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

## Installation Instructions ##

As they are released, all packages are hosted in [a drat repository](https://github.com/eddelbuettel/drat) on this website (specifically: [http://cloudyr.github.io/drat](http://cloudyr.github.io/drat)) and versions are updated daily and are periodically released to CRAN. This means you can install and upgrade cloudyr packages quite simply directly from R:

```R
if(!require("drat")) {
    install.packages("drat")
    library("drat")
}
addRepo("cloudyr")
install.packages("NameOfPackage")
```

To make this even easier, you can add `drat::addRepo("cloudyr")` to your `.Rprofile` or `Rprofile.site` file, so that the cloudyr repository is available every time you open R.


### Installation using devtools ###

You can also install packages using `devtools::install_github()`. Note, however, that all stable versions of packages are automatically added to the cloudyr drat, so you can always retrieve a stable version using the above workflow. To obtain a potentially unstable version, use:

```R
if(!require("devtools")) {
    install.packages("devtools")
    library("devtools")
}
install_github("cloudyr/NameOfPackage")
```

