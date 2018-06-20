---
swagger: "2.0"
x-collection-name: AWS Machine Learning
x-complete: 1
info:
  title: AWS Machine Learning API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddTags:
    get:
      summary: Add Tags
      description: Adds one or more tags to an object, up to a limit of 10.
      operationId: addTags
      x-api-path-slug: actionaddtags-get
      parameters:
      - in: query
        name: ResourceId
        description: The ID of the ML object to tag
        type: string
      - in: query
        name: ResourceType
        description: The type of the ML object to tag
        type: string
      - in: query
        name: Tags
        description: The key-value pairs to use to create tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Tags
  /?Action=DeleteTags:
    get:
      summary: Delete Tags
      description: Deletes the specified tags associated with an ML object.
      operationId: deleteTags
      x-api-path-slug: actiondeletetags-get
      parameters:
      - in: query
        name: ResourceId
        description: The ID of the tagged ML object
        type: string
      - in: query
        name: ResourceType
        description: The type of the tagged ML object
        type: string
      - in: query
        name: TagKeys
        description: One or more tags to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Tags
---