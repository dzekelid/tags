---
name: AWS Elasticsearch Service
x-slug: aws-elasticsearch-service
description: Amazon Elasticsearch Service makes it easy to deploy, operate, and scale
  Elasticsearch for log analytics, full text search, application monitoring, and more.
  Amazon Elasticsearch Service is a fully managed service that delivers Elasticsearch&rsquo;s
  easy-to-use APIs and real-time capabilities along with the availability, scalability,
  and security required by production workloads. The service offers built-in integrations
  with Kibana, Logstash, and AWS services including Amazon Kinesis Firehose, AWS Lambda,
  and Amazon CloudWatch so that you can go from raw data to actionable insights quickly.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonElasticsearchService.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Tags
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-elasticsearch-service/apis.md
specificationVersion: "0.14"
apis:
- name: Amazon Elasticsearch Service API Add Tags
  x-api-slug: amazon-elasticsearch-service-api
  description: |-
    Attaches resource tags to an Amazon ES domain. Use the POST HTTP method
                    with this operation. For more information, see Tagging Amazon ES
                    Domains.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonElasticsearchService.png
  humanURL: https://aws.amazon.com/elasticsearch-service/
  baseURL: ://///2015-01-01/tags
  tags: Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-elasticsearch-service/20150101tags-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-elasticsearch-service/20150101tags-post-openapi.md
- name: Amazon Elasticsearch Service API List Tags
  x-api-slug: amazon-elasticsearch-service-api
  description: |-
    Displays all of the tags for an Amazon ES domain. Use the GET HTTP method
                    with this operation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonElasticsearchService.png
  humanURL: https://aws.amazon.com/elasticsearch-service/
  baseURL: ://///2015-01-01/tags?arn={domain_arn}
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-elasticsearch-service/20150101tagsarndomain-arn-get-openapi.md
- name: Amazon Elasticsearch Service API Remove Tags
  x-api-slug: amazon-elasticsearch-service-api
  description: |-
    Removes the specified resource tags from an Amazon ES domain. Use the POST
                    HTTP method with this operation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonElasticsearchService.png
  humanURL: https://aws.amazon.com/elasticsearch-service/
  baseURL: :////es.{aws_region}.amazonaws.com/2015-01-01/tags-removal
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-elasticsearch-service/es-aws-region-amazonaws-com20150101tagsremoval-post-openapi.md
- name: Amazon Elasticsearch Service API
  x-api-slug: amazon-elasticsearch-service-api
  description: Amazon Elasticsearch Service makes it easy to deploy, operate, and
    scale Elasticsearch for log analytics, full text search, application monitoring,
    and more. Amazon Elasticsearch Service is a fully managed service that delivers
    Elasticsearch&rsquo;s easy-to-use APIs and real-time capabilities along with the
    availability, scalability, and security required by production workloads. The
    service offers built-in integrations with Kibana, Logstash, and AWS services including
    Amazon Kinesis Firehose, AWS Lambda, and Amazon CloudWatch so that you can go
    from raw data to actionable insights quickly.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonElasticsearchService.png
  humanURL: https://aws.amazon.com/elasticsearch-service/
  baseURL: :///
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-elasticsearch-service/openapi.md
x-common:
- type: x-console
  url: https://console.aws.amazon.com/es/home?region=us-east-1
- type: x-documentation
  url: http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-configuration-api.html
- type: x-faq
  url: https://aws.amazon.com/elasticsearch-service/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/elasticsearch-service/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/elasticsearch-service/pricing/
- type: x-website
  url: https://aws.amazon.com/elasticsearch-service/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---