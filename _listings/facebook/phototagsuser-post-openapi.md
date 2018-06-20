---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Post Photo Tags User
  description: Updates the position of a tag on this photo for the user.
  version: 1.0.0
host: graph.facebook.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{photo}/tags:
    get:
      summary: Get Photo Tags
      description: Tags for this photo.
      operationId: getPhotoTags
      x-api-path-slug: phototags-get
      parameters:
      - in: path
        name: photo
        description: Represents the ID of the photo object
      responses:
        200:
          description: OK
      tags:
      - Photo
      - Tags
    post:
      summary: Post Photo Tags
      description: Creates a tag on this photo.
      operationId: postPhotoTags
      x-api-path-slug: phototags-post
      parameters:
      - in: path
        name: photo
        description: Represents the ID of the photo object
      - in: query
        name: to
        description: USER_ID of the User to tag; can also be provided in URL path
      - in: query
        name: x
        description: x coordinate of tag, as a percentage offset from the left edge
          of the picture
      - in: query
        name: "y"
        description: y coordinate of tag, as a percentage offset from the top edge
          of the picture
      responses:
        200:
          description: OK
      tags:
      - Photo
      - Tags
  /{photo}/tags/{user}:
    post:
      summary: Post Photo Tags User
      description: Updates the position of a tag on this photo for the user.
      operationId: postPhotoTagsUser
      x-api-path-slug: phototagsuser-post
      parameters:
      - in: path
        name: photo
        description: Represents the ID of the photo object
      - in: path
        name: user
        description: Represents the ID of the user
      - in: query
        name: x
        description: x coordinate of tag, as a percentage offset from the left edge
          of the picture
      - in: query
        name: "y"
        description: y coordinate of tag, as a percentage offset from the top edge
          of the picture
      responses:
        200:
          description: OK
      tags:
      - Photo
      - Tags
      - User
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