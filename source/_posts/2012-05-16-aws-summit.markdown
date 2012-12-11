---
layout: post
title: "AWS Summit, Melbourne"
date: 2012-05-16 12:00
comments: true
categories: aws conference cloud
---
Yesterday (15th May 2012), I attended the [AWS Summit](http://aws.amazon.com/apac/awssummit-au/) in Melbourne.  This was a single day event covering the future of the AWS Cloud and incorporating some deeper dive sessions.  In the middle of the day there were three (3) breakout tracks.  I attended the AWS "Ninja" Training track (the other two were Executive and Architecture tracks).

Most of the sessions were by Amazon AWS speakers; except for a couple by ThoughtWorks and one by TrendMicro.  I particularly liked the "Continuous Delivery in the Cloud, The Devops Warrior Workshop" session by Nigel Fernandes and Fabio Lessa of ThoughtWorks; mostly because it was a bit deeper than the other sessions and showed some real-world application of Continuous Delivery on the AWS cloud.

The presentations and supplemental materials will be available in about a week's time at the following URL: [http://aws.amazon.com/awssummit](http://aws.amazon.com/awssummit).  Nigel and Fabio's code for the presentation are on Github and will be referenced in the slides that are published.

The event is being repeated tomorrow in Sydney.  To follow along on Twitter, see the hashtag: [#awssummit](https://twitter.com/#!/search/%23awssummit).

Some useful topics/resources mentioned in various talk were:

* Guidance for designing different types of applications in the cloud at [AWS Reference Architectures](http://aws.amazon.com/architecture/)
* Automating the provisioning of AWS resources with [CloudFormation](http://aws.amazon.com/cloudformation/) and building CloudFormation templates with [CloudFormer](http://aws.amazon.com/developertools/6460180344805680) from an existing set of resources
* Taking advantage of [Auto Scaling](http://aws.amazon.com/autoscaling/) to automatically scale your fleet of servers up or down; particularly [Scaling by Policy](http://docs.amazonwebservices.com/AutoScaling/latest/DeveloperGuide/scaling_typesof.html)
* Using [ElasticCache](http://aws.amazon.com/elasticache/) for storing user session data in memory externally from your web tier to allow scaling up/down and deploys to happen more easily
* Using [IAM](http://aws.amazon.com/iam/) credentials in EC2 AMIs rather than your AWS credentials to limit potential damage if credentials are compromised
* Bootstrapping launched AMIs via User Data scripts (e.g. passing in credentials)
* Taking advantage of metadata [Tags](http://docs.amazonwebservices.com/AWSEC2/latest/UserGuide/Using_Tags.html) on AWS resources to more easily manage them
* Using [DynamoDB](http://aws.amazon.com/dynamodb/) to support [Big Data](http://en.wikipedia.org/wiki/Big_data) scenarios and have a fully managed and scalable database

There was also mention of the [AWS re:Invent](http://reinvent.awsevents.com/) conference later in the year in Las Vegas.  I'll see if I can use my training budget for this :)
