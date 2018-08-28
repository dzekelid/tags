---
swagger: "2.0"
x-collection-name: EhrScape
x-complete: 0
info:
  title: Ehr Scape Electronic Health Record APIs Delete a composition's tags.
  description: Delete a composition's tags..
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
host: rest.ehrscape.com
basePath: /rest/v1
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