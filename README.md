AWS CloudFormation Template of Mesosphere DCOS Tracking
=================================================================

An easy repository to track Mesosphere DCOS Community version for AWS CloudFormation. The major problem of the mesosphere community template is hard to customize and track upstream, although Mesosphere guys already release the advanced version of it in their 1.6 release notes. This is another approach for such topic.

## Features

* Split Mesosphere DCOS community template to parts for easy editting
* Multiple Zones support with customized VPC
* Docker Hub integration and ready to pull from private docker hub repository
* S3 Bucket for Log and Software repository rules in IAM, ready to have more customized tasks
* External Admin Node ready to access the cluster
* Memory and disk usage monitor by CloudWatch [go-aws-mon](https://github.com/a3linux/go-aws-mon)
* Docker stale images clean task

## How to deploy

* Deploy your VPC with VPC-Template.json first, you need your VPC network plan, AWS SSH Key pair and so forth
* Deploy your DCOS Cluster with DCOS-Template.json
* If you want to customize the DCOS Cluster, please edit the files under templates/ and re-generate(join) them to your own DCOS-Template.json and update the existed CF stack or deploy new one

Enjoy it.

Allen Chen(a3linux@gmail.com)
