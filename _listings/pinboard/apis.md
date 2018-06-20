---
name: Pinboard
x-slug: pinboard
description: veni, vidi, tweeti
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/240-pinboard.jpg
x-kinRank: "9"
x-alexaRank: "44671"
tags: Tags
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pinboard/apis.md
specificationVersion: "0.14"
apis:
- name: Pinboard Get Tags
  x-api-slug: pinboard
  description: Returns a full list of the user's tags along with the number of times
    they were used.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/240-pinboard.jpg
  humanURL: http://pinboard.in
  baseURL: https://api.pinboard.in//v1//tags/get
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pinboard/tagsget-get-openapi.md
- name: Pinboard Deletes Tag
  x-api-slug: pinboard
  description: Delete an existing tag.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/240-pinboard.jpg
  humanURL: http://pinboard.in
  baseURL: https://api.pinboard.in//v1//tags/delete
  tags: Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pinboard/tagsdelete-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pinboard/tagsdelete-get-openapi.md
- name: Pinboard Rename Tags
  x-api-slug: pinboard
  description: Rename an tag, or fold it in to an existing tag.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/240-pinboard.jpg
  humanURL: http://pinboard.in
  baseURL: https://api.pinboard.in//v1//tags/rename
  tags: Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pinboard/tagsrename-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pinboard/tagsrename-get-openapi.md
- name: Pinboard
  x-api-slug: pinboard
  description: veni, vidi, tweeti
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/240-pinboard.jpg
  humanURL: http://pinboard.in
  baseURL: https://api.pinboard.in//v1
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pinboard/openapi.md
x-common:
- type: x-base
  url: https://api.pinboard.in
- type: x-blog
  url: http://www.pinboard.in/blog/
- type: x-blog-rss
  url: https://blog.pinboard.in/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/pinboard
- type: x-crunchbase
  url: http://www.crunchbase.com/company/pinboard
- type: x-developer
  url: https://pinboard.in/api
- type: x-github
  url: https://github.com/pinboard
- type: x-pricing
  url: https://www.pinboard.in/about/
- type: x-privacy
  url: https://www.pinboard.in/privacy/
- type: x-security
  url: https://www.pinboard.in/security/
- type: x-terms-of-service
  url: https://www.pinboard.in/tos/
- type: x-twitter
  url: https://twitter.com/pinboard
- type: x-website
  url: http://pinboard.in
- type: x-website
  url: http://www.pinboard.in
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---