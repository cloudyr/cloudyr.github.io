---
layout: default
title: the cloudyr project
description: Here's the list of R packages that we are currently working on.
---

## current cloudyr packages

Here's what we're working on so far. Most of the packages are available in [our drat repository](../drat). The [Travis CI status page](https://travis-ci.org/cloudyr) can be used to check the build status of development versions (on GitHub).

| Category | Package | Service | Available From drat | On CRAN | 
|----------|---------|---------|---------------------|---------|
| Bundle | [awspack](https://github.com/cloudyr/awspack) | All Amazon Web Services | Yes | [![CRAN](http://www.r-pkg.org/badges/version/awspack)](https://cloud.r-project.org/package=awspack) |
| Storage  | [aws.s3](https://github.com/cloudyr/aws.s3) | [Amazon Simple Storage Service](http://aws.amazon.com/s3/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.s3)](https://cloud.r-project.org/package=aws.s3) |
| | [aws.efs](https://github.com/cloudyr/aws.efs) | [Amazon Elastic File System](http://aws.amazon.com/efs/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.efs)](https://cloud.r-project.org/package=aws.efs) |
| | [aws.glacier](https://github.com/cloudyr/aws.glacier) | [Amazon Glacier](http://aws.amazon.com/glacier/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.glacier)](https://cloud.r-project.org/package=aws.glacier) |
| | [googleCloudStorageR](https://github.com/cloudyr/googleCloudStorageR) | [Google Cloud Storage](https://cloud.google.com/storage/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/googleCloudStorageR)](https://cloud.r-project.org/package=googleCloudStorageR) |
| | [rdatastore](https://github.com/cloudyr/rdatastore) | [Google Data Store](https://cloud.google.com/datastore/docs/concepts/overview) | No | [![CRAN](http://www.r-pkg.org/badges/version/rdatastore)](https://cloud.r-project.org/package=rdatastore) |
| | [imguR](https://github.com/cloudyr/imguR) | [imgur](http://imgur.com/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/imguR)](https://cloud.r-project.org/package=imguR) |
| | [rcribd](https://github.com/cloudyr/rcribd) | [scribd](https://www.scribd.com/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/rscribd)](https://cloud.r-project.org/package=rscribd) |
| | [AzureStor](https://github.com/cloudyr/AzureStor) | [Azure Storage](https://azure.microsoft.com/en-au/services/storage/) (file, blob and ADLSgen2) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/AzureStor)](https://cloud.r-project.org/package=AzureStor) |
| | [AzureQstor](https://github.com/cloudyr/AzureQstor) | [Azure Queue Storage](https://azure.microsoft.com/services/storage/queues) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/AzureQstor)](https://cloud.r-project.org/package=AzureQstor) |
| Databases/Data stores | [bigQueryR](https://github.com/cloudyr/bigQueryR) | [Google BigQuery](https://cloud.google.com/bigquery/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/bigQueryR)](https://cloud.r-project.org/package=bigQueryR) |
| | [AzureKusto](https://github.com/cloudyr/AzureKusto) | [Azure Data Explorer (aka Kusto)](https://azure.microsoft.com/en-us/services/data-explorer/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/AzureKusto)](https://cloud.r-project.org/package=AzureKusto) |
| Infrastructure | [aws.ses](https://github.com/cloudyr/aws.ses) | [Amazon Simple Email Service](http://aws.amazon.com/ses/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.ses)](https://cloud.r-project.org/package=aws.ses) |
| | [aws.sns](https://github.com/cloudyr/aws.sns) | [Amazon Simple Notification Service](http://aws.amazon.com/sns/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.sns)](https://cloud.r-project.org/package=aws.sns) |
| | [aws.sqs](https://github.com/cloudyr/aws.sqs) | [Amazon Simple Queue Service](http://aws.amazon.com/sqs/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.sqs)](https://cloud.r-project.org/package=aws.sqs) |
| | [cloudcidrs](https://github.com/cloudyr/cloudcidrs) | Tools to Obtain and Work with Cloud Provider CIDR Blocks | Yes | [![CRAN](http://www.r-pkg.org/badges/version/cloudcidrs)](https://cloud.r-project.org/package=cloudcidrs) |
| | [AzureRMR](https://github.com/cloudyr/AzureRMR) | [Azure Resource Manager](https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-group-overview) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/AzureRMR)](https://cloud.r-project.org/package=AzureRMR) |
| | [AzureGraph](https://github.com/cloudyr/AzureGraph) | [Microsoft Graph](https://docs.microsoft.com/en-us/graph/overview) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/AzureGraph)](https://cloud.r-project.org/package=AzureGraph) |
| Computing | [aws.ec2](https://github.com/cloudyr/aws.ec2) | [Amazon EC2](http://aws.amazon.com/ec2/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.ec2)](https://cloud.r-project.org/package=aws.ec2) |
| | [aws.ec2metadata](https://github.com/cloudyr/aws.ec2metadata) | Access [EC2 Instance Metadata](http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-instance-metadata.html) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.ec2metadata)](https://cloud.r-project.org/package=aws.ec2metadata) |
| | [aws.lambda](https://github.com/cloudyr/aws.lambda) | [Amazon Lambda](https://aws.amazon.com/lambda/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/googleComputeEngineR)](https://cloud.r-project.org/package=aws.lambda) |
| | [googleComputeEngineR](https://github.com/cloudyr/googleComputeEngineR) | R Interface with Google Compute Engine | Yes | [![CRAN](http://www.r-pkg.org/badges/version/googleComputeEngineR)](https://cloud.r-project.org/package=googleComputeEngineR) |
| | [rmote](https://github.com/cloudyr/rmote) | Serve Graphics over HTTP from Remote Server | Yes | [![CRAN](http://www.r-pkg.org/badges/version/rmote)](https://cloud.r-project.org/package=rmote) |
| | [AzureVM](https://github.com/cloudyr/AzureVM) | [Azure Virtual Machines](https://azure.microsoft.com/en-us/services/virtual-machines/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/AzureVM)](https://cloud.r-project.org/package=AzureVM) |
| | [AzureVMmetadata](https://github.com/cloudyr/AzureVMmetadata) | Access [Azure VM Instance Metadata](https://docs.microsoft.com/en-us/azure/virtual-machines/windows/instance-metadata-service) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/AzureVMmetadata)](https://cloud.r-project.org/package=AzureVMmetadata) |
| | [AzureContainers](https://github.com/cloudyr/AzureContainers) | Containers in Azure: [ACI](https://azure.microsoft.com/en-us/services/container-instances/), [ACR](https://azure.microsoft.com/en-us/services/container-registry/), [AKS](https://azure.microsoft.com/en-us/services/kubernetes-service/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/AzureContainers)](https://cloud.r-project.org/package=AzureContainers) |
| Information | [aws.alexa](https://github.com/cloudyr/aws.alexa) | [Amazon Alexa](https://aws.amazon.com/awis/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.alexa)](https://cloud.r-project.org/package=aws.alexa) |
| Administration | [aws.iam](https://github.com/cloudyr/aws.iam) | [Amazon Identity and Access Management](https://aws.amazon.com/iam/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.iam)](https://cloud.r-project.org/package=aws.iam) |
| | [aws.cloudtrail](https://github.com/cloudyr/aws.cloudtrail) | [Amazon Cloudtrail](https://aws.amazon.com/cloudtrail/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.cloudtrail)](https://cloud.r-project.org/package=aws.cloudtrail) |
| | [aws.cloudwatch](https://github.com/cloudyr/aws.cloudwatch) | [Amazon Cloudwatch](https://aws.amazon.com/cloudwatch/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.cloudwatch)](https://cloud.r-project.org/package=aws.cloudwatch) |
| | [aws.kms](https://github.com/cloudyr/aws.kms) | [Amazon Key Management Service (KMS)](https://aws.amazon.com/kms/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.kms)](https://cloud.r-project.org/package=aws.kms) |
| | [aws.signature](https://github.com/cloudyr/aws.signature) | AWS API Request Signatures  | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.signature)](https://cloud.r-project.org/package=aws.signature) |
| | [AzureAuth](https://github.com/cloudyr/AzureAuth) | [Azure Active Directory](https://docs.microsoft.com/en-au/azure/active-directory/develop/) Authentication  | Yes | [![CRAN](http://www.r-pkg.org/badges/version/AzureAuth)](https://cloud.r-project.org/package=AzureAuth) |
| | [AzureKeyVault](https://github.com/cloudyr/AzureKeyVault) | [Azure Key Vault](https://azure.microsoft.com/services/key-vault/)  | Yes | [![CRAN](http://www.r-pkg.org/badges/version/AzureKeyVault)](https://cloud.r-project.org/package=AzureKeyVault) |
| Machine Learning as a Service | [RoogleVision](https://github.com/cloudyr/RoogleVision) | [Google Vision](https://cloud.google.com/vision/) | No | [![CRAN](http://www.r-pkg.org/badges/version/RoogleVision)](https://cloud.r-project.org/package=RoogleVision) |
| | [aws.comprehend](https://github.com/cloudyr/aws.comprehend) | [AWS Comprehend](https://aws.amazon.com/comprehend/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.comprehend)](https://cloud.r-project.org/package=aws.comprehend) |
| | [aws.polly](https://github.com/cloudyr/aws.polly) | [AWS Polly](https://aws.amazon.com/polly/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.polly)](https://cloud.r-project.org/package=aws.polly) |
| | [aws.transcribe](https://github.com/cloudyr/aws.transcribe) | [AWS Polly](https://aws.amazon.com/transcribe/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.transcribe)](https://cloud.r-project.org/package=aws.transcribe) |
| | [aws.translate](https://github.com/cloudyr/aws.translate) | [AWS Polly](https://aws.amazon.com/translate/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.translate)](https://cloud.r-project.org/package=aws.translate) |
| | [AzureCognitive](https://github.com/cloudyr/AzureCognitive) | Basic interface to [Azure Cognitive Services](https://azure.microsoft.com/services/cognitive-services/)  | Yes | [![CRAN](http://www.r-pkg.org/badges/version/AzureCognitive)](https://cloud.r-project.org/package=AzureCognitive) |
| | [AzureVision](https://github.com/cloudyr/AzureVision) | Azure [Computer Vision](https://azure.microsoft.com/services/cognitive-services/computer-vision/) and [Custom Vision](https://azure.microsoft.com/services/cognitive-services/custom-vision-service/)  | Yes | [![CRAN](http://www.r-pkg.org/badges/version/AzureVision)](https://cloud.r-project.org/package=AzureVision) |
| Crowdsourcing | [MTurkR](https://github.com/cloudyr/MTurkR) | [Amazon Mechanical Turk](https://www.mturk.com/mturk/welcome) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/MTurkR)](https://cloud.r-project.org/package=MTurkR) |
| | [MTurkRGUI](https://github.com/cloudyr/MTurkRGUI) | GUI for MTurkR | Yes | [![CRAN](http://www.r-pkg.org/badges/version/MTurkRGUI)](https://cloud.r-project.org/package=MTurkRGUI) |
| | [crowdflower](https://github.com/cloudyr/crowdflower) | [Crowdflower](https://www.crowdflower.com/) | No | [![CRAN](http://www.r-pkg.org/badges/version/crowdflower)](https://cloud.r-project.org/package=crowdflower) |
| | [microworkers](https://github.com/cloudyr/microworkers) | [Microworkers](https://microworkers.com/) | No | [![CRAN](http://www.r-pkg.org/badges/version/microworkers)](https://cloud.r-project.org/package=microworkers) |
| Web Surveys | [limer](https://github.com/cloudyr/limer) | [LimeSurvey](https://www.limesurvey.org/) | Yes | [![CRAN](http://www.r-pkg.org/badges/version/limer)](https://cloud.r-project.org/package=limer) |
| Package Development | [appveyor](https://github.com/cloudyr/appveyor) | [Appveyor](https://www.appveyor.com/) API Client  | No | [![CRAN](http://www.r-pkg.org/badges/version/appveyor)](https://cloud.r-project.org/package=appveyor) |
|  | [circleci](https://github.com/cloudyr/circleci) | [Circle-CI](https://circleci.com/) API Client  | Yes | [![CRAN](http://www.r-pkg.org/badges/version/circleci)](https://cloud.r-project.org/package=circleci) |
|  | [aws.code](https://github.com/cloudyr/aws.code) | [Amazon CodeCommit](https://aws.amazon.com/codecommit/)  | Yes | [![CRAN](http://www.r-pkg.org/badges/version/aws.code)](https://cloud.r-project.org/package=aws.code) |

Contributions are always welcome. See [the cloudyr style guide](../styleguide) for guidance on package development, structure, and coding style. Pull requests via GitHub are the preferred way to contribute code and documentation. Ideas, brainstorming, and general discussion are welcome as issues on project-specific repositories or in [cloudyr's gitter chatroom](https://gitter.im/cloudyr). If you would like to contribute a new package, have a look at [the contributing page](../contributing).

## Installation Instructions

As they are released, all packages are hosted in [a drat repository](https://github.com/eddelbuettel/drat) on this website (specifically: [http://cloudyr.github.io/drat](http://cloudyr.github.io/drat)) and versions are updated daily and are periodically released to CRAN. This means you can install and upgrade cloudyr packages quite simply directly from R:

```R
if (!require("drat")) {
    install.packages("drat")
    library("drat")
}
drat::addRepo("cloudyr", "http://cloudyr.github.io/drat")
install.packages("NameOfPackage")
```

To make this even easier, you can add `drat::addRepo("cloudyr")` to your `.Rprofile` or `Rprofile.site` file, so that the cloudyr repository is available every time you open R.


### Installation using devtools

You can also install packages using `remotes::install_github()` or `devtools::install_github()`. Note, however, that all stable versions of packages are automatically added to the cloudyr drat, so you can always retrieve a stable version using the above workflow. To obtain a potentially unstable version, use:

```R
if (!require("remotes")) {
    install.packages("remotes")
}
remotes::install_github("cloudyr/NameOfPackage")
```

