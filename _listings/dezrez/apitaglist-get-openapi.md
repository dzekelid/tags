---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get  a list of tags by a list of ids
  version: 1.0.0
  description: Get  a list of tags by a list of ids.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/tag/list:
    get:
      summary: Get  a list of tags by a list of ids
      description: Get  a list of tags by a list of ids.
      operationId: Tag_GetBytagid
      x-api-path-slug: apitaglist-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: tagid
        description: the list of ids
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Tags
      - By
      - List
      - Of
      - Ids
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