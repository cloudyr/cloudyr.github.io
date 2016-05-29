---
layout: default
title: the cloudyr project
---

## current cloudyr packages ##

Here's what we're working on so far. Most of the packages are available in [our drat repository](../drat).

| Category | Package | Service | Available From drat | On CRAN | 
|----------|---------|---------|---------------------|---------|
| Bundle | [awspack](https://github.com/cloudyr/awspack) | All Amazon Web Services | Yes | [![CRAN](http://www.r-pkg.org/badges/version/awspack)](https://cloud.r-project.org/package=awspack) |
| Storage  | [aws.s3](https://github.com/cloudyr/aws.s3) | Simple Storage Service | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.s3)](https://cloud.r-project.org/package=aws.s3) |
| | [aws.glacier](https://github.com/cloudyr/aws.glacier) | Glacier | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.glacier)](https://cloud.r-project.org/package=aws.glacier) |
| | [imguR](https://github.com/cloudyr/imguR) | [imgur](http://imgur.com/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/imguR)](https://cloud.r-project.org/package=imguR) |
| | [rcribd](https://github.com/cloudyr/rcribd) | [scribd](https://www.scribd.com/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/rscribd)](https://cloud.r-project.org/package=rscribd) |
| Infrastructure | [aws.ses](https://github.com/cloudyr/aws.ses) | Simple Email Service | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.ses)](https://cloud.r-project.org/package=aws.ses) |
| | [aws.sns](https://github.com/cloudyr/aws.sns) | Simple Notification Service | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.sns)](https://cloud.r-project.org/package=aws.sns) |
| | [aws.sqs](https://github.com/cloudyr/aws.sqs) | Simple Queue Service | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.sqs)](https://cloud.r-project.org/package=aws.sqs) |
| Computing | [aws.ec2](https://github.com/cloudyr/aws.ec2) | EC2 | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.ec2)](https://cloud.r-project.org/package=aws.ec2) |
| Information | [aws.alexa](https://github.com/cloudyr/aws.alexa) | Alexa | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.alexa)](https://cloud.r-project.org/package=aws.alexa) |
| Administration | [aws.iam](https://github.com/cloudyr/aws.iam) | Identity and Access Management | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.iam)](https://cloud.r-project.org/package=aws.iam) |
| | [aws.cloudtrail](https://github.com/cloudyr/aws.cloudtrail) | Cloudtrail | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.cloudtrail)](https://cloud.r-project.org/package=aws.cloudtrail) |
| | [aws.cloudwatch](https://github.com/cloudyr/aws.cloudwatch) | Cloudwatch | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.cloudwatch)](https://cloud.r-project.org/package=aws.cloudwatch) |
| | [aws.signature](https://github.com/cloudyr/aws.signature) | Computes AWS Signature Version 4  | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.signature)](https://cloud.r-project.org/package=aws.signature) |
| Crowdsourcing | [MTurkR](https://github.com/leeper/MTurkR) | Amazon Mechanical Turk | Yes | [![CRAN](http://www.r-pkg.org/badges/version/MTurkR)](https://cloud.r-project.org/package=MTurkR) |
| | [MTurkRGUI](https://github.com/leeper/MTurkRGUI) | MTurkR GUI | Yes | [![CRAN](http://www.r-pkg.org/badges/version/MTurkRGUI)](https://cloud.r-project.org/package=MTurkRGUI) |
| | [crowdflower](https://github.com/cloudyr/crowdflower) | Crowdflower | No | [![CRAN](http://www.r-pkg.org/badges/version/crowdflower)](https://cloud.r-project.org/package=crowdflower) |
| | [microworkers](https://github.com/cloudyr/microworkers) | Microworkers | No | [![CRAN](http://www.r-pkg.org/badges/version/microworkers)](https://cloud.r-project.org/package=microworkers) |
| Web Surveys | [Rmonkey](https://github.com/cloudyr/Rmonkey) | Survey Monkey | Yes | [![CRAN](http://www.r-pkg.org/badges/version/Rmonkey)](https://cloud.r-project.org/package=Rmonkey) |
| Package Development | [travisci](https://github.com/cloudyr/travisci) | Travis-CI API Client  | Yes | [![CRAN](http://www.r-pkg.org/badges/version/travisci)](https://cloud.r-project.org/package=travisci) |
|  | [appveyor](https://github.com/cloudyr/appveyor) | Appveyor API Client  | No | [![CRAN](http://www.r-pkg.org/badges/version/appveyor)](https://cloud.r-project.org/package=appveyor) |
|  | [circleci](https://github.com/cloudyr/circleci) | Circle-CI API Client  | Yes | [![CRAN](http://www.r-pkg.org/badges/version/circleci)](https://cloud.r-project.org/package=circleci) |

Contributions are always welcome. See [the cloudyr style guide](../styleguide) for guidance on package development, structure, and coding style. Pull requests via GitHub are the preferred way to contribute code and documentation. Ideas, brainstorming, and general discussion are welcome as issues on project-specific repositories or in [cloudyr's gitter chatroom](https://gitter.im/cloudyr). If you would like to contribute a new package, have a look at [the contributing page](../contributing).

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

