swagger: "2.0"
x-collection-name: 7digital
x-complete: 1
info:
  title: 7digital Purchasing API
  description: the-purchasing-api-allows-3rd-parties-to-deliver-digital-content-to-individual-users-
  version: "1.2"
host: api.7digital.com
basePath: 1.2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  tag:
    'get ':
      summary: tag
      description: This method returns a list of all available tags.
      operationId: tag
      x-api-path-slug: tag-get
      parameters:
      - ~
      - in: query
        name: artistId
        description: The unique identifier of the artist
      - in: query
        name: country
        description: nttttttt2 letter ISO country code of the country whose artists
          you would like to searchntttttt
      - in: query
        name: imageSize
        description: ntttttttThe requested width of the image in pixelsntttttt
      - in: query
        name: page
        description: Page number of the result set
      - in: query
        name: pageSize
        description: Number of items to be returned per page
      - in: query
        name: streamable
        description: If provided search results will contain only artists that can/cannot
          be streamed
      - in: query
        name: tags
        description: A single or comma separated list of tags
      responses:
        200:
          description: OK
      tags:
      - Tag