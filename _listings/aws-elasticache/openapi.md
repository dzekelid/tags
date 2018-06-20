---
swagger: "2.0"
x-collection-name: AWS ElastiCache
x-complete: 1
info:
  title: AWS ElastiCache API
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
      description: Adds up to 10 cost allocation tags to the named resource.
      operationId: addTagsToResource
      x-api-path-slug: actionaddtagstoresource-get
      parameters:
      - in: query
        name: ResourceName
        description: The Amazon Resource Name (ARN) of the resource to which the tags
          are to be added,             for example arn:aws:elasticache:us-west-2:0123456789:cluster:myCluster             or
          arn:aws:elasticache:us-west-2:0123456789:snapshot:mySnapshot
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of cost allocation tags to be added to this resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Tags
  /?Action=ListTagsForResource:
    get:
      summary: List Tags For Resource
      description: Lists all cost allocation tags currently on the named resource.
      operationId: listTagsForResource
      x-api-path-slug: actionlisttagsforresource-get
      parameters:
      - in: query
        name: ResourceName
        description: The Amazon Resource Name (ARN) of the resource for which you
          want the list of tags,             for example arn:aws:elasticache:us-west-2:0123456789:cluster:myCluster             or
          arn:aws:elasticache:us-west-2:0123456789:snapshot:mySnapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Tags
  /?Action=RemoveTagsFromResource:
    get:
      summary: Remove Tags From Resource
      description: "Removes the tags identified by the TagKeys \n            list
        from the named resource."
      operationId: removeTagsFromResource
      x-api-path-slug: actionremovetagsfromresource-get
      parameters:
      - in: query
        name: ResourceName
        description: The Amazon Resource Name (ARN) of the resource from which you
          want the tags removed,             for example arn:aws:elasticache:us-west-2:0123456789:cluster:myCluster             or
          arn:aws:elasticache:us-west-2:0123456789:snapshot:mySnapshot
        type: string
      - in: query
        name: TagKeys.member.N
        description: A list of TagKeys identifying the tags you want removed from
          the named resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Tags
---