swagger: "2.0"
x-collection-name: Fluxiom
x-complete: 1
info:
  title: Fluxiom API
  description: the-fluxiom-api-allows-you-to-hook-into-fluxiom-and-connect-it-with-other-apps-
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