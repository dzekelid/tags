---
swagger: "2.0"
x-collection-name: OpenRouteService
x-complete: 0
info:
  title: AP Metadata Services Tags
  description: Returns the set of AP standardized vocabulary terms that apply to the
    submitted news content. The  output can be limited to one or more authorities
    specified in the request; for example, you can choose  to apply only AP Organization,
    AP Subject and AP Geography tags to the submitted content, but not  AP Person
    or AP Company.
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---