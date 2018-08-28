swagger: "2.0"
x-collection-name: Pinboard
x-complete: 1
info:
  title: Pinboard
  description: store-manage-and-share-bookmarks-on-pinboard
  version: 1.0.0
host: api.pinboard.in
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tags/get:
    get:
      summary: Get Tags
      description: Returns a full list of the user's tags along with the number of
        times they were used.
      operationId: tags.get.get
      x-api-path-slug: tagsget-get
      parameters:
      - in: query
        name: format
        description: the format to return
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /tags/delete:
    get:
      summary: Deletes Tag
      description: Delete an existing tag.
      operationId: tags.delete.get
      x-api-path-slug: tagsdelete-get
      responses:
        200:
          description: OK
      tags:
      - Tags
  /tags/rename:
    get:
      summary: Rename Tags
      description: Rename an tag, or fold it in to an existing tag.
      operationId: tags.rename.get
      x-api-path-slug: tagsrename-get
      responses:
        200:
          description: OK
      tags:
      - Tags