---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 1
info:
  title: AWS EC2 Systems Manager API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListTagsForResource:
    get:
      summary: List Tags For Resource
      description: Returns a list of the tags assigned to the specified resource.
      operationId: listTagsForResource
      x-api-path-slug: actionlisttagsforresource-get
      parameters:
      - in: query
        name: ResourceId
        description: The resource ID for which you want to see a list of tags
        type: string
      - in: query
        name: ResourceType
        description: Returns a list of tags for a specific resource type
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - TagsResource
  /?Action=RemoveTagsFromResource:
    get:
      summary: Remove Tags From Resource
      description: Removes all tags from the specified resource.
      operationId: removeTagsFromResource
      x-api-path-slug: actionremovetagsfromresource-get
      parameters:
      - in: query
        name: ResourceId
        description: The resource ID for which you want to remove tags
        type: string
      - in: query
        name: ResourceType
        description: The type of resource of which you want to remove a tag
        type: string
      - in: query
        name: TagKeys
        description: Tag keys that you want to remove from the specified resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Tags
      - From
      - Resource
---