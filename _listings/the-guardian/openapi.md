swagger: "2.0"
x-collection-name: The Guardian
x-complete: 1
info:
  title: The Guardian
  version: 1.0.0
host: content.guardianapis.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tags:
    get:
      summary: Tags
      description: Retrieves the tags used across the Guardian news platform.
      operationId: tags
      x-api-path-slug: tags-get
      responses:
        200:
          description: OK
      tags:
      - Tags