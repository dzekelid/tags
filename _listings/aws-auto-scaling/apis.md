---
name: AWS Auto Scaling
x-slug: aws-auto-scaling
description: Auto Scaling helps you maintain application availability and allows you
  to scale yourAmazon EC2capacity up or down automatically according to conditions
  you define. You can use Auto Scaling to help ensure that you are running your desired
  number of Amazon EC2 instances. Auto Scaling can also automatically increase the
  number of Amazon EC2 instances during demand spikes to maintain performance and
  decrease capacity during lulls to reduce costs. Auto Scaling is well suited both
  to applications that have stable demand patterns or that experience hourly, daily,
  or weekly variability in usage.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2_AutoScaling.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Tags
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-auto-scaling/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Auto Scaling API Create Or Update Tags
  x-api-slug: aws-auto-scaling-api
  description: Creates or updates tags for the specified Auto Scaling group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2_AutoScaling.png
  humanURL: https://aws.amazon.com/autoscaling/
  baseURL: ://///?Action=CreateOrUpdateTags
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-auto-scaling/actioncreateorupdatetags-get-openapi.md
- name: AWS Auto Scaling API Delete Tags
  x-api-slug: aws-auto-scaling-api
  description: Deletes the specified tags.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2_AutoScaling.png
  humanURL: https://aws.amazon.com/autoscaling/
  baseURL: ://///?Action=DeleteTags
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-auto-scaling/actiondeletetags-get-openapi.md
- name: AWS Auto Scaling API Describe Tags
  x-api-slug: aws-auto-scaling-api
  description: Describes the specified tags.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2_AutoScaling.png
  humanURL: https://aws.amazon.com/autoscaling/
  baseURL: ://///?Action=DescribeTags
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-auto-scaling/actiondescribetags-get-openapi.md
- name: AWS Auto Scaling API
  x-api-slug: aws-auto-scaling-api
  description: Auto Scaling helps you maintain application availability and allows
    you to scale yourAmazon EC2capacity up or down automatically according to conditions
    you define. You can use Auto Scaling to help ensure that you are running your
    desired number of Amazon EC2 instances. Auto Scaling can also automatically increase
    the number of Amazon EC2 instances during demand spikes to maintain performance
    and decrease capacity during lulls to reduce costs. Auto Scaling is well suited
    both to applications that have stable demand patterns or that experience hourly,
    daily, or weekly variability in usage.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2_AutoScaling.png
  humanURL: https://aws.amazon.com/autoscaling/
  baseURL: :///
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-auto-scaling/openapi.md
x-common:
- type: x-articles
  url: http://developer.amazonwebservices.com/connect/kbcategory.jspa?categoryID=100
- type: x-change-log
  url: http://developer.amazonwebservices.com/connect/kbcategory.jspa?categoryID=86
- type: x-code
  url: http://developer.amazonwebservices.com/connect/kbcategory.jspa?categoryID=85
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/reference/autoscaling/index.html
- type: x-documentation
  url: http://docs.aws.amazon.com/AutoScaling/latest/APIReference/
- type: x-forum
  url: http://developer.amazonwebservices.com/connect/forum.jspa?forumID=30
- type: x-getting-started
  url: https://aws.amazon.com/autoscaling/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/autoscaling/pricing/
- type: x-service-health
  url: http://status.aws.amazon.com/
- type: x-website
  url: https://aws.amazon.com/autoscaling/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---