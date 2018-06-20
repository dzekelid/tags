---
swagger: "2.0"
x-collection-name: Fluxiom
x-complete: 0
info:
  title: Fluxiom API Delete tag
  description: Delete tag
  termsOfService: http://www.fluxiom.com/terms
  version: v1
host: '{subdomain}.fluxiom.com'
basePath: /api/{format}
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/tags:
    get:
      summary: Get tags
      description: Get tags
      operationId: get-tags
      x-api-path-slug: apitags-get
      responses:
        200:
          description: OK
      tags:
      - Tags
    post:
      summary: Create tag
      description: Create tag
      operationId: create-tag
      x-api-path-slug: apitags-post
      parameters:
      - in: query
        name: tag
        description: tag tt string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /api/tags/ID:
    get:
      summary: Get single tag
      description: Get single tag
      operationId: get-single-tag
      x-api-path-slug: apitagsid-get
      responses:
        200:
          description: OK
      tags:
      - Tags
    put:
      summary: Update tag
      description: Update tag
      operationId: update-tag
      x-api-path-slug: apitagsid-put
      parameters:
      - in: query
        name: tag
        description: tag tt string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /api/tags/{id}:
    delete:
      summary: Delete tag
      description: Delete tag
      operationId: delete-tag
      x-api-path-slug: apitagsid-delete
      parameters:
      - in: path
        name: id
        description: Unique id of the tag
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Id
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