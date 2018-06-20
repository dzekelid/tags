---
name: Watchful
x-slug: watchful
description: Watchful resulted from the need for a single, unified dashboard to easily
  monitor all of the web sites in our portfolios. After years of evolution, our solution
  has matured into a simple, complete and professional service.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/watchful-li-logo.jpg
x-kinRank: "8"
x-alexaRank: "0"
tags: Tags
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/watchful/apis.md
specificationVersion: "0.14"
apis:
- name: Watchful Find Sites By ID
  x-api-slug: watchful
  description: Returns a report based on a site ID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/watchful-li-logo.jpg
  humanURL: http://watchful.li
  baseURL: https://watchful.li//api/v1//reports/tags/{id}
  tags: Reports,Tags,Id
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/watchful/reportstagsid-get-openapi.md
- name: Watchful Return Tags For A Specific Website
  x-api-slug: watchful
  description: Return tags for a specific website
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/watchful-li-logo.jpg
  humanURL: http://watchful.li
  baseURL: https://watchful.li//api/v1//sites/{id}/tags
  tags: Sites,Id,Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/watchful/sitesidtags-get-openapi.md
- name: Watchful Add Tags For A Specific Website
  x-api-slug: watchful
  description: Add tags for a specific website
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/watchful-li-logo.jpg
  humanURL: http://watchful.li
  baseURL: https://watchful.li//api/v1//sites/{id}/tags
  tags: Sites,Id,Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/watchful/sitesidtags-post-openapi.md
- name: Watchful Get A List Of Tags
  x-api-slug: watchful
  description: Returns a list of tags
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/watchful-li-logo.jpg
  humanURL: http://watchful.li
  baseURL: https://watchful.li//api/v1//tags
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/watchful/tags-get-openapi.md
- name: Watchful Create A Tag
  x-api-slug: watchful
  description: Create a tag
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/watchful-li-logo.jpg
  humanURL: http://watchful.li
  baseURL: https://watchful.li//api/v1//tags
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/watchful/tags-post-openapi.md
- name: Watchful Get The List Of Fields
  x-api-slug: watchful
  description: Returns a list of fields
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/watchful-li-logo.jpg
  humanURL: http://watchful.li
  baseURL: https://watchful.li//api/v1//tags/metadata
  tags: Tags,Metadata
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/watchful/tagsmetadata-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/watchful/tagsmetadata-get-openapi.md
- name: Watchful Delete A Specific Tag
  x-api-slug: watchful
  description: Delete a specific tag
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/watchful-li-logo.jpg
  humanURL: http://watchful.li
  baseURL: https://watchful.li//api/v1//tags/{id}
  tags: Tags,Id
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/watchful/tagsid-delete-openapi.md
- name: Watchful Find Tag By ID
  x-api-slug: watchful
  description: Returns a tag based on ID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/watchful-li-logo.jpg
  humanURL: http://watchful.li
  baseURL: https://watchful.li//api/v1//tags/{id}
  tags: Tags,Id
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/watchful/tagsid-get-openapi.md
- name: Watchful Update A Tag
  x-api-slug: watchful
  description: Update a tag
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/watchful-li-logo.jpg
  humanURL: http://watchful.li
  baseURL: https://watchful.li//api/v1//tags/{id}
  tags: Tags,Id
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/watchful/tagsid-put-openapi.md
- name: Watchful Find Sites By Tag ID
  x-api-slug: watchful
  description: Returns a list of sites based with a specific tag id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/watchful-li-logo.jpg
  humanURL: http://watchful.li
  baseURL: https://watchful.li//api/v1//tags/{id}/sites
  tags: Tags,Id,Sites
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/watchful/tagsidsites-get-openapi.md
- name: Watchful
  x-api-slug: watchful
  description: Watchful resulted from the need for a single, unified dashboard to
    easily monitor all of the web sites in our portfolios. After years of evolution,
    our solution has matured into a simple, complete and professional service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/watchful-li-logo.jpg
  humanURL: http://watchful.li
  baseURL: https://watchful.li//api/v1
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/watchful/openapi.md
x-common:
- type: x-application-gallery
  url: https://watchful.li/apps/
- type: x-blog
  url: https://watchful.li/news/
- type: x-blog-rss
  url: https://watchful.li/news/feed/rss.html
- type: x-developer
  url: https://watchful.li/support-services/kb/article/watchful-rest-api
- type: x-facebook
  url: https://www.facebook.com/watchfulli
- type: x-faq
  url: https://watchful.li/support-services/faq.html
- type: x-google-plus
  url: https://plus.google.com/+WatchfulLi
- type: x-knowledgebase
  url: https://watchful.li/support-services/kb.html
- type: x-pricing
  url: https://watchful.li/pricing
- type: x-privacy
  url: https://watchful.li/privacy-policy.html
- type: x-terms-of-service
  url: https://watchful.li/terms-of-service.html
- type: x-twitter
  url: https://twitter.com/watchfulli
- type: x-website
  url: http://watchful.li
- type: x-website
  url: https://watchful.li/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---