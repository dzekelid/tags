swagger: "2.0"
x-collection-name: Xibo
x-complete: 1
info:
  title: Xibo API
  description: xibo-cms-api
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /layout/{layoutId}/tag:
    post:
      summary: Tag Layout
      description: Tag a Layout with one or more tags
      operationId: layoutTag
      x-api-path-slug: layoutlayoutidtag-post
      parameters:
      - in: path
        name: layoutId
        description: The Layout Id to Tag
      - in: formData
        name: tag
        description: An array of tags
      responses:
        200:
          description: OK
      tags:
      - Tag
      - Layout
  /library/{mediaId}/tag:
    post:
      summary: Tag Media
      description: Tag a Media with one or more tags
      operationId: mediaTag
      x-api-path-slug: librarymediaidtag-post
      parameters:
      - in: path
        name: mediaId
        description: The Media Id to Tag
      - in: formData
        name: tag
        description: An array of tags
      responses:
        200:
          description: OK
      tags:
      - Tag
      - Media