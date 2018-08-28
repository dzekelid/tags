swagger: "2.0"
x-collection-name: AWS CloudSearch
x-complete: 1
info:
  title: AWS CloudSearch
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
      description: |-
        Attaches resource tags to an
         Amazon CloudSearch domain.
      operationId: AddTags
      x-api-path-slug: actionaddtags-get
      parameters:
      - in: query
        name: Base
        description: An                  error occurred while processing the request
        type: string
      - in: query
        name: InternalException
        description: The processing of the request failed because of an internal service
          error
        type: string
      - in: query
        name: LimitExceededException
        description: The request contains more than the allowed number and type of
          Amazon CloudSearch domain                  resources
        type: string
      - in: query
        name: ValidationException
        description: The request contains invalid input or is missing required input
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=ListTags:
    get:
      summary: List Tags
      description: |-
        Displays all of the resource
         tags for an Amazon CloudSearch domain.
      operationId: ListTags
      x-api-path-slug: actionlisttags-get
      parameters:
      - in: query
        name: Base
        description: An error occurred while                  processing the request
        type: string
      - in: query
        name: InternalException
        description: The                  processing of the request failed because
          of an internal service error
        type: string
      - in: query
        name: LimitExceededException
        description: The                  request contains more than the allowed number
          and type of Amazon CloudSearch domain resources
        type: string
      - in: query
        name: ValidationException
        description: The                  request contains invalid input or is missing
          required input
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=RemoveTags:
    get:
      summary: Remove Tags
      description: |-
        Removes the specified resource tags
         from an Amazon ES domain.
      operationId: RemoveTags
      x-api-path-slug: actionremovetags-get
      parameters:
      - in: query
        name: Base
        description: An error occurred while                  processing the request
        type: string
      - in: query
        name: InternalException
        description: The                  processing of the request failed because
          of an internal service error
        type: string
      - in: query
        name: ValidationException
        description: The                  request contains invalid input or is missing
          required input
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags