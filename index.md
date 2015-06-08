---
layout: default
title: the cloudyr project
---

# the cloudyr project #

Welcome to **the cloudyr project**! The goal of this initiative is to make cloud computing with R easier, starting with robust tools for working with cloud computing platforms. The project's inital work is with Amazon Web Services, but tools for Google Cloud Services are also in the works.

The motivation for the project is simple: cloud computing is a critical component of contemporary software development and data analysis. The reasons for this are numerous (e.g., speed, memory, storage capacity, parallel computing, etc.) and need not be rehashed here. Yet R does not currently have many tools for engaging in cloud computing. There are many tools for extracting data from the cloud (see [the Web Technologies Task View](http://cran.r-project.org/web/views/WebTechnologies.html)), but there are not very many tools for connecting a local R instance to cloud-based services.

This is unfortunate given the growing popularity of R and the fact that cloud providers often make software development kits available for numerous languages (such as Java, Python, Ruby, etc.). As an example, boto provides an incredibly robust framework for developing cloud computing applications in Python. R is currently underserved in by AWS software development kits and there are only a few disjointed third-party packages. Aiming to fill this void, the goal of the cloudyr project is to make cloud computing faster, easier, and more intuitive for R users through a unified cloud computing interface.

Indeed, the project's motto is simple: *Make R Cloudier!*

## Project Packages for AWS ##

The project is developing the following packages so far, with the goal to wrap all AWS APIs in the near future:

### Storage ###

 - [aws.s3](http://github.com/cloudyr/aws.s3): Simple Storage Service client
 - [aws.glacier](http://github.com/cloudyr/aws.glacier): Glacier storage client

### Infrastructure ###

 - [aws.ses](http://github.com/cloudyr/aws.ses): Simple Email Service client
 - [aws.sns](http://github.com/cloudyr/aws.sns): Simple Notification Service (multi-platform push notification) client
 - [aws.sqs](http://github.com/cloudyr/aws.sqs): Simple Queue Service client

### Computing ###
 
 - [aws.ec2](http://github.com/cloudyr/aws.ec2): EC2 client

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

 - [MTurkR](http://github.com/leeper/MTurkR): Amazon Mechanical Turk crowdsourcing client
 
### Administration ###

 - [aws.iam](http://github.com/cloudyr/aws.iam): Identity and Access Management client
 
<!--
 - [aws.config](http://github.com/cloudyr/aws.config): Config client
-->

 - [aws.cloudtrail](http://github.com/cloudyr/aws.cloudtrail): Cloudtrail (API usage tracking) client
 - [aws.cloudwatch](http://github.com/cloudyr/aws.cloudwatch): Cloudwatch (AWS usage monitoring) client
 - [aws.signature](http://github.com/cloudyr/aws.signature): Computes AWS Signature Version 4

<!--
### Project Packages for GCS ###

 - [goog.compute]()
 - [goog.container]()
 - [goog.storage]()
-->
