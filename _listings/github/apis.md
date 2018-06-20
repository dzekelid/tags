---
name: GitHub
x-slug: github
description: With a community of more than 10 million people, developers can discover,
  use and contribute to over 24 million projects using a powerful, collaborative workflow.    Whether
  using GitHub.com or your own instance of GitHub Enterprise, you can integrate ...
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
x-kinRank: "10"
x-alexaRank: "70"
tags: Tags
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/github/apis.md
specificationVersion: "0.14"
apis:
- name: Github Add Repos Owner Repo Git Tags
  x-api-slug: github
  description: |-
    Create a Tag Object.
    Note that creating a tag object does not create the reference that makes a
    tag in Git. If you want to create an annotated tag in Git, you have to do
    this call to create the tag object, and then create the refs/tags/[tag]
    reference. If you want to create a lightweight tag, you only have to create
    the tag reference - this call would be unnecessary.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/git/tags
  tags: Repos, Owner, Repo, Git, Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/github/reposownerrepogittags-post-openapi.md
- name: Github Get Repos Owner Repo Git Tags Shacode
  x-api-slug: github
  description: Get a Tag.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/git/tags/{shaCode}
  tags: Repos, Owner, Repo, Git, Tags, Shacode
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/github/reposownerrepogittagsshacode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/github/reposownerrepogittagsshacode-get-openapi.md
- name: Github Get Repos Owner Repo Tags
  x-api-slug: github
  description: Get list of tags.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/tags
  tags: Repos, Owner, Repo, Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/github/reposownerrepotags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/github/reposownerrepotags-get-openapi.md
- name: Github
  x-api-slug: github
  description: With a community of more than 10 million people, developers can discover,
    use and contribute to over 24 million projects using a powerful, collaborative
    workflow.    Whether using GitHub.com or your own instance of GitHub Enterprise,
    you can integrate ...
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/github/openapi.md
x-common:
- type: x--net-library
  url: https://github.com/octokit/octokit.net
- type: x-base
  url: https://api.github.com
- type: x-blog
  url: http://github.com/blog
- type: x-blog-rss
  url: https://github.com/blog/subscribe
- type: x-change-log
  url: https://developer.github.com/changes/
- type: x-contact-form
  url: https://github.com/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/github
- type: x-crunchbase
  url: https://crunchbase.com/organization/github
- type: x-developer
  url: https://developer.github.com/
- type: x-github
  url: https://github.com/github
- type: x-guides
  url: https://developer.github.com/guides/
- type: x-ios-sdk
  url: https://github.com/octokit/octokit.objc
- type: x-pricing
  url: https://github.com/pricing
- type: x-privacy
  url: http://help.github.com/privacy-policy/
- type: x-ruby-library
  url: https://github.com/octokit/octokit.rb
- type: x-security
  url: http://help.github.com/security/
- type: x-status
  url: https://status.github.com/
- type: x-terms-of-service
  url: http://help.github.com/terms-of-service/
- type: x-transparency-report
  url: https://github.com/blog/1987-github-s-2014-transparency-report
- type: x-twitter
  url: https://twitter.com/github
- type: x-webhooks
  url: https://developer.github.com/webhooks/
- type: x-website
  url: https://github.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---