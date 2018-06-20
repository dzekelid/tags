---
name: AWS CloudFront
x-slug: aws-cloudfront
description: Amazon CloudFront is a global content delivery network (CDN) service
  that accelerates delivery of your websites, APIs, video content or other web assets.
  It integrates with other Amazon Web Services products to give developers and businesses
  an easy way to accelerate content to end users with no minimum usage commitments.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonCloudFront.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Tags
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-cloudfront/apis.md
specificationVersion: "0.14"
apis:
- name: AWS CloudFront API Create Distribution With Tags
  x-api-slug: aws-cloudfront-api
  description: Create a new distribution with tags.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonCloudFront.png
  humanURL: https://aws.amazon.com/cloudfront/
  baseURL: ://///?Action=CreateDistributionWithTags
  tags: Distribution, Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-cloudfront/actioncreatedistributionwithtags-get-openapi.md
- name: AWS CloudFront API Create Streaming Distribution With Tags
  x-api-slug: aws-cloudfront-api
  description: Create a new streaming distribution with tags.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonCloudFront.png
  humanURL: https://aws.amazon.com/cloudfront/
  baseURL: ://///?Action=CreateStreamingDistributionWithTags
  tags: Streaming, Distribution, Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-cloudfront/actioncreatestreamingdistributionwithtags-get-openapi.md
- name: AWS CloudFront API List Tags For Resource
  x-api-slug: aws-cloudfront-api
  description: List tags for a CloudFront resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonCloudFront.png
  humanURL: https://aws.amazon.com/cloudfront/
  baseURL: ://///?Action=ListTagsForResource
  tags: List, Tags, Resource
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-cloudfront/actionlisttagsforresource-get-openapi.md
- name: AWS CloudFront API
  x-api-slug: aws-cloudfront-api
  description: Amazon CloudFront is a global content delivery network (CDN) service
    that accelerates delivery of your websites, APIs, video content or other web assets.
    It integrates with other Amazon Web Services products to give developers and businesses
    an easy way to accelerate content to end users with no minimum usage commitments.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonCloudFront.png
  humanURL: https://aws.amazon.com/cloudfront/
  baseURL: :///
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-cloudfront/openapi.md
x-common:
- type: x-analysis
  url: https://aws.amazon.com/cloudfront/reporting/
- type: x-documentation
  url: http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/cloudfront/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/cloudfront/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/cloudfront/pricing/
- type: x-service-level-agreement
  url: https://aws.amazon.com/cloudfront/sla/
- type: x-webinars
  url: https://aws.amazon.com/cloudfront/webinars/
- type: x-website
  url: https://aws.amazon.com/cloudfront/
- type: x-whats-new
  url: https://aws.amazon.com/cloudfront/whats-new/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---