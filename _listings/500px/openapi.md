---
swagger: "2.0"
x-collection-name: 500px
x-complete: 1
info:
  title: 500px
  description: 500px-is-a-photo-community-powered-by-creative-people-worldwide-that-lets-you-discover-share-buy-and-sell-inspiring-photographs-
  version: v1
host: api.500px.com
basePath: /v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /photos/:id/tags:
    delete:
      summary: Delete Photos Tags
      description: Removes tags from the photo. Accepts one or multiple coma separated
        tags.
      operationId: deletePhotosTags
      x-api-path-slug: photosidtags-delete
      parameters:
      - in: query
        name: id (required)
        description: The Photo ID to remove tags from
      - in: query
        name: tags (required)
        description: Coma separated tags
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Tags
    post:
      summary: Post Photos Tags
      description: Adds tags to the photo. Accepts one or multiple coma separated
        tags.
      operationId: postPhotosTags
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
      - Tags
  /photos/{id}/tags:
    post:
      summary: Post Photos Tags
      description: Adds tags to the photo. Accepts one or multiple coma separated
        tags.
      operationId: postPhotosTags
      x-api-path-slug: photosidtags-post
      parameters:
      - in: path
        name: id
        description: The Photo ID to add tags for
      - in: query
        name: tags
        description: Coma separated tags
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Tags
    delete:
      summary: Delete Photos Tags
      description: Removes tags from the photo. Accepts one or multiple coma separated
        tags.
      operationId: deletePhotosTags
      x-api-path-slug: photosidtags-delete
      parameters:
      - in: path
        name: id
        description: The Photo ID to remove tags from
      - in: query
        name: tags
        description: Coma separated tags
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Tags
---