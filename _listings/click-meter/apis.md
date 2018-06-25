---
name: Click Meter
x-slug: click-meter
description: ClickMeter was founded in 2012 as a byproduct of an experienced web-marketing
  agency. The ClickMeter System was initially a web tool created to address the needs
  of our agency to precisely count and track the web-marketing actions we performed
  for our customers.The system evolved rapidly, and emerged as one of the most widely
  used software solutions in our agency to collect, analyze, and share data for and
  with our customers. After few years after the development of the first ClickMeter
  system, we decided to go live with a service that can be useful to everyone involved
  in web-marketing activities.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Tags
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/click-meter/apis.md
specificationVersion: "0.14"
apis:
- name: Click Meter List of all the groups associated to the user filtered by this
    tag.
  x-api-slug: click-meter
  description: List of all the groups associated to the user filtered by this tag..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////tags
  tags: Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/click-meter/tags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/click-meter/tags-get-openapi.md
- name: Click Meter Create a tag
  x-api-slug: click-meter
  description: Create a tag.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////tags
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/click-meter/tags-post-openapi.md
- name: Click Meter List of all the groups associated to the user filtered by this
    tag.
  x-api-slug: click-meter
  description: List of all the groups associated to the user filtered by this tag..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////tags/count
  tags: Tags,Count
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/click-meter/tagscount-get-openapi.md
- name: Click Meter Delete a tag
  x-api-slug: click-meter
  description: Delete a tag.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////tags/{tagId}
  tags: Tags,TagId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/click-meter/tagstagid-delete-openapi.md
- name: Click Meter Retrieve a tag
  x-api-slug: click-meter
  description: Retrieve a tag.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////tags/{tagId}
  tags: Tags,TagId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/click-meter/tagstagid-get-openapi.md
- name: Click Meter Delete the association of this tag with all datapoints
  x-api-slug: click-meter
  description: Delete the association of this tag with all datapoints.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////tags/{tagId}/datapoints
  tags: Tags,TagId,Datapoints
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/click-meter/tagstagiddatapoints-delete-openapi.md
- name: Click Meter List of all the datapoints associated to the user filtered by
    this tag
  x-api-slug: click-meter
  description: List of all the datapoints associated to the user filtered by this
    tag.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////tags/{tagId}/datapoints
  tags: Tags,TagId,Datapoints
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/click-meter/tagstagiddatapoints-get-openapi.md
- name: Click Meter Count the datapoints associated to the user filtered by this tag
  x-api-slug: click-meter
  description: Count the datapoints associated to the user filtered by this tag.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////tags/{tagId}/datapoints/count
  tags: Tags,TagId,Datapoints,Count
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/click-meter/tagstagiddatapointscount-get-openapi.md
- name: Click Meter Associate/Deassociate a tag with a datapoint
  x-api-slug: click-meter
  description: Associate/deassociate a tag with a datapoint.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////tags/{tagId}/datapoints/patch
  tags: Tags,TagId,Datapoints,Patch
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/click-meter/tagstagiddatapointspatch-put-openapi.md
- name: Click Meter Delete the association of this tag with all groups
  x-api-slug: click-meter
  description: Delete the association of this tag with all groups.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////tags/{tagId}/groups
  tags: Tags,TagId,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/click-meter/tagstagidgroups-delete-openapi.md
- name: Click Meter List of all the groups associated to the user filtered by this
    tag.
  x-api-slug: click-meter
  description: List of all the groups associated to the user filtered by this tag..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////tags/{tagId}/groups
  tags: Tags,TagId,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/click-meter/tagstagidgroups-get-openapi.md
- name: Click Meter Count the groups associated to the user filtered by this tag
  x-api-slug: click-meter
  description: Count the groups associated to the user filtered by this tag.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////tags/{tagId}/groups/count
  tags: Tags,TagId,Groups,Count
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/click-meter/tagstagidgroupscount-get-openapi.md
- name: Click Meter Associate/Deassociate a tag with a group
  x-api-slug: click-meter
  description: Associate/deassociate a tag with a group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////tags/{tagId}/groups/patch
  tags: Tags,TagId,Groups,Patch
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/click-meter/tagstagidgroupspatch-put-openapi.md
- name: Click Meter Fast patch a tag name
  x-api-slug: click-meter
  description: Fast patch a tag name.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////tags/{tagId}/name
  tags: Tags,TagId,Name
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/click-meter/tagstagidname-put-openapi.md
- name: Click Meter
  x-api-slug: click-meter
  description: ClickMeter was founded in 2012 as a byproduct of an experienced web-marketing
    agency. The ClickMeter System was initially a web tool created to address the
    needs of our agency to precisely count and track the web-marketing actions we
    performed for our customers.The system evolved rapidly, and emerged as one of
    the most widely used software solutions in our agency to collect, analyze, and
    share data for and with our customers. After few years after the development of
    the first ClickMeter system, we decided to go live with a service that can be
    useful to everyone involved in web-marketing activities.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80//
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/click-meter/openapi.md
x-common:
- type: x-blog
  url: https://blog.clickmeter.com/
- type: x-pricing
  url: http://clickmeter.com/pricing-signup
- type: x-support
  url: https://support.clickmeter.com/hc/en-us
- type: x-terms-of-service
  url: http://clickmeter.com/terms-conditions
- type: x-twitter
  url: https://twitter.com/clickmeter
- type: x-website
  url: http://clickmeter.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---