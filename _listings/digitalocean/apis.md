---
name: DigitalOcean
x-slug: digitalocean
description: DigitalOcean is a simple and fast cloud hosting service built for developers.
  Customers can create a cloud server in 55 seconds, and pricing plans start at only
  $5 per month for 512MB of RAM, 20GB SSD, 1 CPU, and 1TB Transfer. Featuring a 99.99%
  Uptime SLA, DigitalOcean has servers located in New York, San Francisco, and Amsterdam.
  The DigitalOcean control panel interface is simple and intuitive, which power users
  can replicate on a larger scale with the company&rsquo;s API. DigitalOcean uses
  KVM virtualization and additionally hosts a library of helpful walkthroughs and
  tutorials that cover server configuration and optimization.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Tags
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/digitalocean/apis.md
specificationVersion: "0.14"
apis:
- name: DigitalOcean API-V2 - List all Tags
  x-api-slug: tags-get
  description: "To list all of your tags, you can send a GET request to /v2/tags.\r\n\r\nThe
    response will be a JSON object with a key called _tags_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/digitalocean/tags-get-openapi.md
- name: DigitalOcean API-V2 - Listing Droplets by Tag
  x-api-slug: droplets-get
  description: "To list Droplets by a tag, send a GET request to /v2/droplets?tag_name=$TAG_NAME.\r\n\r\nThe
    response will match that of regular droplet listing request but will be filtered
    to only include the tagged Droplets."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/digitalocean/droplets-get-openapi.md
- name: DigitalOcean API-V2 - Create a new Tag
  x-api-slug: tags-post
  description: "To create a Tag you can send a POST request to /v2/tags with a name
    attribute.\r\n\r\nThe response will be a JSON object with a key called _tag_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/digitalocean/tags-post-openapi.md
- name: DigitalOcean API-V2 - Tag a Resource
  x-api-slug: tagspostmandotagresources-post
  description: "Resources can be tagged by sending a POST request to /v2/tags/$TAG_NAME/resources
    with an array of json objects containing resource_id and resource_type attributes.\r\n\r\nCurrently
    only tagging of Droplets is supported. resource_id is expected to be the Droplet's
    id attribute as a string, and resource_type is expected to be the string droplet."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/digitalocean/tagspostmandotagresources-post-openapi.md
- name: DigitalOcean API-V2 - Tag a Resource
  x-api-slug: tagspostmandotagresources-post
  description: "Resources can be tagged by sending a POST request to /v2/tags/$TAG_NAME/resources
    with an array of json objects containing resource_id and resource_type attributes.\r\n\r\nCurrently
    only tagging of Droplets is supported. resource_id is expected to be the Droplet's
    id attribute as a string, and resource_type is expected to be the string droplet."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/digitalocean/tagspostmandotagresources-post-openapi.md
- name: DigitalOcean API-V2 - Tag a Resource
  x-api-slug: tagspostmandotagresources-post
  description: "Resources can be tagged by sending a POST request to /v2/tags/$TAG_NAME/resources
    with an array of json objects containing resource_id and resource_type attributes.\r\n\r\nCurrently
    only tagging of Droplets is supported. resource_id is expected to be the Droplet's
    id attribute as a string, and resource_type is expected to be the string droplet."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/digitalocean/tagspostmandotagresources-post-openapi.md
- name: DigitalOcean API-V2 - Create a new Tag
  x-api-slug: tags-post
  description: "To create a Tag you can send a POST request to /v2/tags with a name
    attribute.\r\n\r\nThe response will be a JSON object with a key called _tag_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/digitalocean/tags-post-openapi.md
- name: DigitalOcean API-V2 - Create a new Tag
  x-api-slug: tags-post
  description: "To create a Tag you can send a POST request to /v2/tags with a name
    attribute.\r\n\r\nThe response will be a JSON object with a key called _tag_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/digitalocean/tags-post-openapi.md
- name: DigitalOcean API-V2 - Listing Droplets by Tag
  x-api-slug: droplets-get
  description: "To list Droplets by a tag, send a GET request to /v2/droplets?tag_name=$TAG_NAME.\r\n\r\nThe
    response will match that of regular droplet listing request but will be filtered
    to only include the tagged Droplets."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/digitalocean/droplets-get-openapi.md
- name: DigitalOcean API-V2 - Listing Droplets by Tag
  x-api-slug: droplets-get
  description: "To list Droplets by a tag, send a GET request to /v2/droplets?tag_name=$TAG_NAME.\r\n\r\nThe
    response will match that of regular droplet listing request but will be filtered
    to only include the tagged Droplets."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/digitalocean/droplets-get-openapi.md
- name: DigitalOcean API-V2 - Listing Droplets by Tag
  x-api-slug: droplets-get
  description: "To list Droplets by a tag, send a GET request to /v2/droplets?tag_name=$TAG_NAME.\r\n\r\nThe
    response will match that of regular droplet listing request but will be filtered
    to only include the tagged Droplets."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/digitalocean/droplets-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://digital.river.api.gallery.streamdata.io
- type: x-api-stack
  url: http://digitalocean.stack.network
- type: x-base
  url: https://api.digitalocean.com/
- type: x-blog
  url: https://www.digitalocean.com/company/blog/
- type: x-blog-rss
  url: https://www.digitalocean.com/company/blog/feed.xml
- type: x-command-line-interface
  url: https://github.com/digitalocean/doctl
- type: x-developer
  url: https://developers.digitalocean.com/
- type: x-github
  url: https://github.com/digitalocean
- type: x-twitter
  url: https://twitter.com/digitalocean
- type: x-website
  url: https://www.digitalocean.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---