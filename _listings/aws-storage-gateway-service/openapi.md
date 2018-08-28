swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 1
info:
  title: AWS Storage Gateway Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddTagsToResource:
    get:
      summary: Add Tags To Resource
      description: Adds one or more tags to the specified resource.
      operationId: addTagsToResource
      x-api-path-slug: actionaddtagstoresource-get
      parameters:
      - in: query
        name: ResourceARN
        description: The Amazon Resource Name (ARN) of the resource you want to add
          tags to
        type: string
      - in: query
        name: Tags
        description: The key-value pair that represents the tag you want to add to
          the resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=ListTagsForResource:
    get:
      summary: List Tags For Resource
      description: Lists the tags that have been added to the specified resource.
      operationId: listTagsForResource
      x-api-path-slug: actionlisttagsforresource-get
      parameters:
      - in: query
        name: Limit
        description: Specifies that the list of tags returned be limited to the specified
          number of         items
        type: string
      - in: query
        name: Marker
        description: An opaque string that indicates the position at which to begin
          returning the list of         tags
        type: string
      - in: query
        name: ResourceARN
        description: The Amazon Resource Name (ARN) of the resource for which you
          want to list         tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=RemoveTagsFromResource:
    get:
      summary: Remove Tags From Resource
      description: Removes one or more tags from the specified resource.
      operationId: removeTagsFromResource
      x-api-path-slug: actionremovetagsfromresource-get
      parameters:
      - in: query
        name: ResourceARN
        description: The Amazon Resource Name (ARN) of the resource you want to remove
          the tags         from
        type: string
      - in: query
        name: TagKeys
        description: The keys of the tags you want to remove from the specified resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags