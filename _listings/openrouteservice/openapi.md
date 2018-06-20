---
swagger: "2.0"
x-collection-name: OpenRouteService
x-complete: 1
info:
  title: AP Metadata Services
  description: add-value-to-your-news-content-with-apu2019s-industryleading-metadata--accurate-comprehensive-richly-detailed-data-designed-specifically-for-use-by-news-publishers--ap-metadata-services-is-a-new-set-of-apis-that-gives-you-direct-access-to-the-same-metadata-system-that-supports-apu2019s-awardwinning-global-news-operation-
  version: v1
host: cv.ap.org
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  Tags/:
    post:
      summary: Tags
      description: Returns the set of AP standardized vocabulary terms that apply
        to the submitted news content. The  output can be limited to one or more authorities
        specified in the request; for example, you can choose  to apply only AP Organization,
        AP Subject and AP Geography tags to the submitted content, but not  AP Person
        or AP Company.
      operationId: postTags
      x-api-path-slug: tags-post
      parameters:
      - in: query
        name: apiKey
        description: API Key
      - in: body
        name: story
        description: URL-encoded content  submitted for tagging
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Tags
---