swagger: "2.0"
x-collection-name: EhrScape
x-complete: 1
info:
  title: EhrScape Terminology APIs
  description: validates-and-resolves-terminology-codes
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
host: rest.ehrscape.com
basePath: /terminology-adapter/rest
paths:
  /tagging:
    delete:
      summary: Delete a composition's tags.
      description: Delete a composition's tags..
      operationId: deleteTags
      x-api-path-slug: tagging-delete
      parameters:
      - in: body
        name: body
        description: The tag request object specifies tags on what AQL paths to delete
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Tagging
    get:
      summary: Returns objects matching the specified tags.
      description: Returns objects matching the specified tags..
      operationId: findObjectsWithTags
      x-api-path-slug: tagging-get
      parameters:
      - in: query
        name: includeCurrentlyDeleted
        description: Whether or not to include compositions whose current (last) version
          is deleted
      - in: query
        name: includeDeletedVersions
        description: Whether or not to include deleted composition versions
      - in: query
        name: tags
        description: A collection of tags that the returned objects need to be tagged
          with (a conjunction)
      - in: query
        name: versionsToReturn
        description: Which composition versions to return
      responses:
        200:
          description: OK
      tags:
      - Tagging
    post:
      summary: Tags the specified composition and/or its sub-structures.
      description: Tags the specified composition and/or its sub-structures..
      operationId: tag
      x-api-path-slug: tagging-post
      parameters:
      - in: body
        name: body
        description: The tag request object specifies what to tag and how
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Tagging
  /tagging/{compositionUid}:
    get:
      summary: Returns tags for the specified composition.
      description: Returns tags for the specified composition..
      operationId: getTags
      x-api-path-slug: taggingcompositionuid-get
      parameters:
      - in: path
        name: compositionUid
        description: The ID of the composition whose tags to return
      responses:
        200:
          description: OK
      tags:
      - Tagging
      - CompositionUid