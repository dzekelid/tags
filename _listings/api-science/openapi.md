---
swagger: "2.0"
x-collection-name: API Science
x-complete: 1
info:
  title: API Science
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tags:
    get:
      summary: List All Tags
      description: List All Tags
      operationId: listAllTags
      x-api-path-slug: tags-get
      parameters:
      - in: query
        name: detailed
        description: Detailed List All Tags
      responses:
        200:
          description: OK
      tags:
      - Tags
  /inventory/tags:
    "":
      summary: Deleting a tag
      description: ""
      operationId: deleting-a-tag
      x-api-path-slug: inventorytags-
      parameters:
      - in: body
        name: color
        description: The color of the tag in hexcode
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: name
        description: Name of the tag
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: token
        description: Your API token
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Tags
---