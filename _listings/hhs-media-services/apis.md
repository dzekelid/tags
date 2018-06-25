---
name: HHS Media Services
x-slug: hhs-media-services
description: Use this API platform to create sites with text and multimedia content
  for syndication. CDC, FDA, HHS, and NIH have built syndication sites using this
  platform, which is available in Java and .NET.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Tags
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/hhs-media-services/apis.md
specificationVersion: "0.14"
apis:
- name: HHS Media Services Get Tags
  x-api-slug: hhs-media-services
  description: Returns the list of Tags matching the specified query parameters in
    the specified 'format'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/tags.json
  tags: Resources,Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/hhs-media-services/resourcestags-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/hhs-media-services/resourcestags-json-get-openapi.md
- name: HHS Media Services Get TagLanguages
  x-api-slug: hhs-media-services
  description: Returns the list of TagLanguages
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/tags/tagLanguages.json
  tags: Resources,Tags,TagLanguages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/hhs-media-services/resourcestagstaglanguages-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/hhs-media-services/resourcestagstaglanguages-json-get-openapi.md
- name: HHS Media Services Get TagTypes
  x-api-slug: hhs-media-services
  description: Returns the list of TagTypes
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/tags/tagTypes.json
  tags: Resources,Tags,TagTypes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/hhs-media-services/resourcestagstagtypes-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/hhs-media-services/resourcestagstagtypes-json-get-openapi.md
- name: HHS Media Services Get Tag by ID
  x-api-slug: hhs-media-services
  description: Returns the Tag identified by the 'id' in the specified 'format'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/tags/{id}.json
  tags: Resources,Tags,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/hhs-media-services/resourcestagsid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/hhs-media-services/resourcestagsid-json-get-openapi.md
- name: HHS Media Services Get MediaItems for Tag
  x-api-slug: hhs-media-services
  description: Returns the list of MediaItems associated with the Tag identified by
    the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/tags/{id}/media.json
  tags: Resources,Tags,Id,Media
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/hhs-media-services/resourcestagsidmedia-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/hhs-media-services/resourcestagsidmedia-json-get-openapi.md
- name: HHS Media Services Get related Tags by ID
  x-api-slug: hhs-media-services
  description: Returns the list of Tags related to the Tag identified by the 'id'
    in the specified format.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/tags/{id}/related.json
  tags: Resources,Tags,Id,Related
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/hhs-media-services/resourcestagsidrelated-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/hhs-media-services/resourcestagsidrelated-json-get-openapi.md
- name: HHS Media Services Get MediaItems for Tag
  x-api-slug: hhs-media-services
  description: Renders the list of MediaItems associated with the Tag identified by
    the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/tags/{id}/syndicate.json
  tags: Resources,Tags,Id,Syndicate
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/hhs-media-services/resourcestagsidsyndicate-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/hhs-media-services/resourcestagsidsyndicate-json-get-openapi.md
- name: HHS Media Services
  x-api-slug: hhs-media-services
  description: Use this API platform to create sites with text and multimedia content
    for syndication. CDC, FDA, HHS, and NIH have built syndication sites using this
    platform, which is available in Java and .NET.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/hhs-media-services/openapi.md
x-common:
- type: x-website
  url: https://api.digitalmedia.hhs.gov/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---