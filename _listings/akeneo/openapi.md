swagger: "2.0"
x-collection-name: Akeneo
x-complete: 1
info:
  title: Official Akeneo PIM API
  description: the-akeneo-api-brought-to-youfind-out-how-this-postman-collection-works-by-visiting-httpapi-akeneo-com
  version: 1.0.0
host: example.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/v1/asset-tags:
    get:
      summary: asset tags (2.1 only)
      description: Asset tags (2.1 only).
      operationId: RestV1AssetTagsGet
      x-api-path-slug: restv1assettags-get
      parameters:
      - in: query
        name: limit
      - in: query
        name: with_count
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Tags
      - (2
      - "1"
      - Only)
  /rest/v1/asset-tags/colored:
    get:
      summary: asset tag (2.1 only)
      description: Assuming that the given code is the code of an existing asset tag
      operationId: RestV1AssetTagsColoredGet
      x-api-path-slug: restv1assettagscolored-get
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Tag
      - (2
      - "1"
      - Only)
    patch:
      summary: asset tag (2.1 only)
      description: Asset tag (2.1 only).
      operationId: RestV1AssetTagsColoredPatch
      x-api-path-slug: restv1assettagscolored-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Tag
      - (2
      - "1"
      - Only)