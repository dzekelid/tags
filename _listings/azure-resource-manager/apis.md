---
name: Azure Resource Manager
x-slug: azure-resource-manager
description: Azure Resource Manager enables you to deploy and manage the infrastructure
  for your Azure solutions. You organize related resources in resource groups, and
  deploy your resources with JSON templates. For an introduction to deploying and
  managing resources with Resource Manager, see Azure Resource Manager overview.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Tags
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/azure-resource-manager/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Resource Manager API Tags Delete Value
  x-api-slug: azure-resource-manager-api
  description: Deletes a tag value.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/tagNames/{tagName}/tagValues/{tagValue}
  tags: Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/azure-resource-manager/subscriptionssubscriptionidtagnamestagnametagvaluestagvalue-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/azure-resource-manager/subscriptionssubscriptionidtagnamestagnametagvaluestagvalue-delete-openapi.md
- name: Azure Resource Manager API Tags Create Or Update Value
  x-api-slug: azure-resource-manager-api
  description: Creates a tag value. The name of the tag must already exist.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/tagNames/{tagName}/tagValues/{tagValue}
  tags: Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/azure-resource-manager/subscriptionssubscriptionidtagnamestagnametagvaluestagvalue-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/azure-resource-manager/subscriptionssubscriptionidtagnamestagnametagvaluestagvalue-put-openapi.md
- name: Azure Resource Manager API Creates a tag in the subscription.
  x-api-slug: azure-resource-manager-api
  description: The tag name can have a maximum of 512 characters and is case insensitive.
    Tag names created by Azure have prefixes of microsoft, azure, or windows. You
    cannot create tags with one of these prefixes.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/tagNames/{tagName}
  tags: Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/azure-resource-manager/subscriptionssubscriptionidtagnamestagname-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/azure-resource-manager/subscriptionssubscriptionidtagnamestagname-put-openapi.md
- name: Azure Resource Manager API Deletes a tag from the subscription.
  x-api-slug: azure-resource-manager-api
  description: You must remove all values from a resource tag before you can delete
    it.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/tagNames/{tagName}
  tags: Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/azure-resource-manager/subscriptionssubscriptionidtagnamestagname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/azure-resource-manager/subscriptionssubscriptionidtagnamestagname-delete-openapi.md
- name: Azure Resource Manager API Tags List
  x-api-slug: azure-resource-manager-api
  description: Gets the names and values of all resource tags that are defined in
    a subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/tagNames
  tags: Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/azure-resource-manager/subscriptionssubscriptionidtagnames-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/azure-resource-manager/subscriptionssubscriptionidtagnames-get-openapi.md
- name: Azure Resource Manager API
  x-api-slug: azure-resource-manager-api
  description: Azure Resource Manager enables you to deploy and manage the infrastructure
    for your Azure solutions. You organize related resources in resource groups, and
    deploy your resources with JSON templates. For an introduction to deploying and
    managing resources with Resource Manager, see Azure Resource Manager overview.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/azure-resource-manager/openapi.md
x-common:
- type: x-website
  url: https://docs.microsoft.com/en-us/rest/api/resources/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---