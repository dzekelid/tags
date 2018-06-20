---
swagger: "2.0"
x-collection-name: AngelList
x-complete: 0
info:
  title: AngelList Get Tag Parents
  description: Get Tag Parents
  termsOfService: https://angel.co/terms
  contact:
    name: AngelList
    url: https://angel.co/api
    email: api@angel.co
  version: v1
host: api.angel.co
basePath: /1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tags/{tag_id}:
    get:
      summary: Get Tag
      description: Get Tag
      operationId: tags
      x-api-path-slug: tagstag-id-get
      parameters:
      - in: path
        name: tag_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Tags
  /tags/{tag_id}/children:
    get:
      summary: Get Tags Children
      description: Get Tags Children
      operationId: tagsChildren
      x-api-path-slug: tagstag-idchildren-get
      parameters:
      - in: path
        name: tag_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Tags
  /tags/{tag_id}/jobs:
    get:
      summary: Get Jobs by Tag
      description: Get Jobs by Tag
      operationId: jobs
      x-api-path-slug: tagstag-idjobs-get
      parameters:
      - in: path
        name: tag_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Tags
  /tags/{tag_id}/parents:
    get:
      summary: Get Tag Parents
      description: Get Tag Parents
      operationId: tagParents
      x-api-path-slug: tagstag-idparents-get
      parameters:
      - in: path
        name: tag_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
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