---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Saves a tag to location match
  version: 1.0.0
  description: Saves a tag to location match.
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
  /api/location/tag/match:
    post:
      summary: Saves a tag to location match
      description: Saves a tag to location match.
      operationId: Location_ProcessTagLocationMatchesBycommands
      x-api-path-slug: apilocationtagmatch-post
      parameters:
      - in: body
        name: commands
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Saves
      - Tag
      - To
      - Location
      - Match
  /api/tag/{name}:
    get:
      summary: Get a tag by its name
      description: Get a tag by its name.
      operationId: Tag_GetByname
      x-api-path-slug: apitagname-get
      parameters:
      - in: path
        name: name
        description: The name of the tag to get
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Tag
      - By
      - Its
      - Name
  /api/tag/suggest:
    get:
      summary: Get tag suggestions for value
      description: Get tag suggestions for value.
      operationId: Tag_SuggestByname
      x-api-path-slug: apitagsuggest-get
      parameters:
      - in: query
        name: name
        description: The value to retrieve suggestions for
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Tag
      - Suggestionsvalue
  /api/TagDescription/{id}:
    get:
      summary: ""
      description: .
      operationId: TagDescription_GetByid
      x-api-path-slug: apitagdescriptionid-get
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - ""
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