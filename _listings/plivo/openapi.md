---
swagger: "2.0"
x-collection-name: Plivo
x-complete: 1
info:
  title: Codenvy Account API
  description: this-is-the-api-for-managing-codenvy-account-
  version: 1.0.0
host: /account
basePath: https://codenvy.com/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /photos/:id/tags:
    post:
      summary: Post Photos Tags
      description: Adds tags to the photo. Accepts one or multiple coma separated
        tags.
      operationId: adds-tags-to-the-photo-accepts-one-or-multiple-coma-separated-tags
      x-api-path-slug: photosidtags-post
      parameters:
      - in: query
        name: id (required)
        description: The Photo ID to add tags for
      - in: query
        name: tags (required)
        description: Coma separated tags
      responses:
        200:
          description: OK
      tags:
      - Photos
      - :id
      - Tags
---