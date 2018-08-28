swagger: "2.0"
x-collection-name: AWS Direct Connect
x-complete: 1
info:
  title: AWS Direct Connect API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeTags:
    get:
      summary: Describe Tags
      description: Describes the tags associated with the specified Direct Connect
        resources.
      operationId: describeTags
      x-api-path-slug: actiondescribetags-get
      parameters:
      - in: query
        name: resourceArns
        description: The Amazon Resource Names (ARNs) of the Direct Connect resources
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=TagResource:
    get:
      summary: Tag Resource
      description: Adds the specified tags to the specified Direct Connect resource.
      operationId: tagResource
      x-api-path-slug: actiontagresource-get
      parameters:
      - in: query
        name: resourceArn
        description: The Amazon Resource Name (ARN) of the Direct Connect resource
        type: string
      - in: query
        name: tags
        description: The list of tags to add
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Tags