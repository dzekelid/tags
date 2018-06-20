---
name: AWS Storage Gateway Service
x-slug: aws-storage-gateway-service
description: The AWS Storage Gateway service seamlessly enables hybrid storage between
  on-premises storage environments andthe AWS Cloud. It combines a multi-protocol
  storage appliance with highly efficient network connectivity toAmazon cloud storageservices,
  delivering local performance with virtually unlimited scale. Customers use it in
  remote offices and datacenters for hybrid cloud workloads, backup and restore, archive,
  disaster recovery, and tiered storage.The Storage Gateway virtual appliance connects
  seamlessly to your local infrastructure as a file server, as a volume, or as a virtual
  tape library (VTL). This seamless connection makes it simple for organizations to
  augment existing on-premises storage investments with the high scalability, extreme
  durability and low cost of cloud storage.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Tags
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-storage-gateway-service/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Storage Gateway Service API Add Tags To Resource
  x-api-slug: aws-storage-gateway-service-api
  description: Adds one or more tags to the specified resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: ://///?Action=AddTagsToResource
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-storage-gateway-service/actionaddtagstoresource-get-openapi.md
- name: AWS Storage Gateway Service API List Tags For Resource
  x-api-slug: aws-storage-gateway-service-api
  description: Lists the tags that have been added to the specified resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: ://///?Action=ListTagsForResource
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-storage-gateway-service/actionlisttagsforresource-get-openapi.md
- name: AWS Storage Gateway Service API Remove Tags From Resource
  x-api-slug: aws-storage-gateway-service-api
  description: Removes one or more tags from the specified resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: ://///?Action=RemoveTagsFromResource
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-storage-gateway-service/actionremovetagsfromresource-get-openapi.md
- name: AWS Storage Gateway Service API
  x-api-slug: aws-storage-gateway-service-api
  description: The AWS Storage Gateway service seamlessly enables hybrid storage between
    on-premises storage environments andthe AWS Cloud. It combines a multi-protocol
    storage appliance with highly efficient network connectivity toAmazon cloud storageservices,
    delivering local performance with virtually unlimited scale. Customers use it
    in remote offices and datacenters for hybrid cloud workloads, backup and restore,
    archive, disaster recovery, and tiered storage.The Storage Gateway virtual appliance
    connects seamlessly to your local infrastructure as a file server, as a volume,
    or as a virtual tape library (VTL). This seamless connection makes it simple for
    organizations to augment existing on-premises storage investments with the high
    scalability, extreme durability and low cost of cloud storage.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-storage-gateway-service/openapi.md
x-common:
- type: x-documentation
  url: http://docs.aws.amazon.com/storagegateway/latest/APIReference
- type: x-faq
  url: https://aws.amazon.com/storagegateway/faqs/
- type: x-pricing
  url: https://aws.amazon.com/storagegateway/pricing/
- type: x-website
  url: https://aws.amazon.com/storagegateway/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---