---
swagger: "2.0"
x-collection-name: Clover
x-complete: 0
info:
  title: Clover Get all items for a single tag
  version: 1.0.0
  description: Get all items for a single tag.
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/merchants/{mId}/tags:
    get:
      summary: Get all tags
      description: Similarly to how they are described by wikipedia, tags are an informal
        way of establishing a relationship. Tags currently may be associated with
        items and printers. When an tag is associated with both an item and a printer
        that establishes a special relationship that results in those items being
        printed out on the associated printer when printing an order. Other than that
        special case there is no effect when an item is associated with a tag. Developers
        may use tags to establish a relationship meaningful for their needs.
      operationId: GetTags
      x-api-path-slug: v3merchantsmidtags-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items, printers]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, deleted, name, id]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tags
    post:
      summary: Create a tag
      description: Create a tag.
      operationId: CreateTag
      x-api-path-slug: v3merchantsmidtags-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tags
  /v3/merchants/{mId}/tags/{tagId}:
    get:
      summary: Get a single tag
      description: Get a single tag.
      operationId: GetTag
      x-api-path-slug: v3merchantsmidtagstagid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items, printers]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: tagId
        description: Tag Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tags
      - TagId
    post:
      summary: Update a single tag
      description: Update a single tag.
      operationId: UpdateTag
      x-api-path-slug: v3merchantsmidtagstagid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [items, printers]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: tagId
        description: Tag Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tags
      - TagId
    delete:
      summary: Delete a tag
      description: Delete a tag.
      operationId: DeleteTag
      x-api-path-slug: v3merchantsmidtagstagid-delete
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: tagId
        description: Tag Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tags
      - TagId
  /v3/merchants/{mId}/items/{itemId}/tags:
    get:
      summary: Get tags for a single item
      description: Get tags for a single item.
      operationId: GetItemTags
      x-api-path-slug: v3merchantsmiditemsitemidtags-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items, printers]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, deleted, name, id]'
      - in: path
        name: itemId
        description: Item Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Items
      - ItemId
      - Tags
  /v3/merchants/{mId}/tags/{tagId}/items:
    get:
      summary: Get all items for a single tag
      description: Get all items for a single tag.
      operationId: GetTaggedItems
      x-api-path-slug: v3merchantsmidtagstagiditems-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items, printers]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, hidden, itemCode, alternateName,
          option'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: tagId
        description: Tag Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tags
      - TagId
      - Items
  /v3/merchants/{mId}/tag_items:
    post:
      summary: Create or delete tag items
      description: Create or delete tag items.
      operationId: CreateOrDeleteTagItems
      x-api-path-slug: v3merchantsmidtag-items-post
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tag
      - Items
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