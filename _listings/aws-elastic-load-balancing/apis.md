---
name: AWS Elastic Load Balancing
x-slug: aws-elastic-load-balancing
description: Elastic Load Balancing automatically distributes incoming application
  traffic across multiple Amazon EC2 instances. It enables you to achieve fault tolerance
  in your applications, seamlessly providing the required amount of load balancing
  capacity needed to route application traffic.Elastic Load Balancing offers two types
  of load balancers that both feature high availability, automatic scaling, and robust
  security. These include theClassic Load Balancerthat routes traffic based on either
  application or network level information, and theApplication Load Balancerthat routes
  traffic based on advanced application level information that includes the content
  of the request. The Classic Load Balancer is ideal for simple load balancing of
  traffic across multiple EC2 instances, while the Application Load Balancer is ideal
  for applications needing advanced routing capabilities, microservices, and container-based
  architectures. Application Load Balancer offers ability to route traffic to multiple
  services or load balance across multiple ports on the same EC2 instance.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_ElasticLoadBalancing.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Tags
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-elastic-load-balancing/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Elastic Load Balancing API Add Tags
  x-api-slug: aws-elastic-load-balancing-api
  description: Adds the specified tags to the specified resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_ElasticLoadBalancing.png
  humanURL: https://aws.amazon.com/elasticloadbalancing/
  baseURL: ://///?Action=AddTags
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-elastic-load-balancing/actionaddtags-get-openapi.md
- name: AWS Elastic Load Balancing API Describe Tags
  x-api-slug: aws-elastic-load-balancing-api
  description: Describes the tags for the specified resources.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_ElasticLoadBalancing.png
  humanURL: https://aws.amazon.com/elasticloadbalancing/
  baseURL: ://///?Action=DescribeTags
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-elastic-load-balancing/actiondescribetags-get-openapi.md
- name: AWS Elastic Load Balancing API Remove Tags
  x-api-slug: aws-elastic-load-balancing-api
  description: Removes the specified tags from the specified resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_ElasticLoadBalancing.png
  humanURL: https://aws.amazon.com/elasticloadbalancing/
  baseURL: ://///?Action=RemoveTags
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-elastic-load-balancing/actionremovetags-get-openapi.md
- name: AWS Elastic Load Balancing API
  x-api-slug: aws-elastic-load-balancing-api
  description: Elastic Load Balancing automatically distributes incoming application
    traffic across multiple Amazon EC2 instances. It enables you to achieve fault
    tolerance in your applications, seamlessly providing the required amount of load
    balancing capacity needed to route application traffic.Elastic Load Balancing
    offers two types of load balancers that both feature high availability, automatic
    scaling, and robust security. These include theClassic Load Balancerthat routes
    traffic based on either application or network level information, and theApplication
    Load Balancerthat routes traffic based on advanced application level information
    that includes the content of the request. The Classic Load Balancer is ideal for
    simple load balancing of traffic across multiple EC2 instances, while the Application
    Load Balancer is ideal for applications needing advanced routing capabilities,
    microservices, and container-based architectures. Application Load Balancer offers
    ability to route traffic to multiple services or load balance across multiple
    ports on the same EC2 instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_ElasticLoadBalancing.png
  humanURL: https://aws.amazon.com/elasticloadbalancing/
  baseURL: :///
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-elastic-load-balancing/openapi.md
x-common:
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/reference/elbv2/index.html
- type: x-documentation
  url: http://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/elasticloadbalancing/classicloadbalancer/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/elasticloadbalancing/classicloadbalancer/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/elasticloadbalancing/classicloadbalancer/pricing/
- type: x-website
  url: https://aws.amazon.com/elasticloadbalancing/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---