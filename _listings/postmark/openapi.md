---
swagger: "2.0"
x-collection-name: Postmark
x-complete: 1
info:
  title: Postmark
  description: send-emails-retrieve-bounces-and-start-accepting-inbound-emails-all-via-an-easytouse-http-api-
  version: 1.0.0
host: spamcheck.postmarkapp.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /bounces/tags:
    parameters:
      summary: Parameters Bounces Tags
      description: Parameters bounces tags.
      operationId: parametersBouncesTags
      x-api-path-slug: bouncestags-parameters
      responses:
        200:
          description: OK
      tags:
      - Bounces
      - Tags
    get:
      summary: Get Bounces Tags
      description: Returns a list of tags used for the current server.
      operationId: getBouncesTags
      x-api-path-slug: bouncestags-get
      parameters:
      - in: query
        name: Accept
        description: The accepted type for the response
      - in: query
        name: Content-Type
        description: The content type of the request
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Bounces
      - Tags
  /triggers/tags:
    get:
      summary: Get Triggers Tags
      description: Get triggers tags.
      operationId: getTriggersTags
      x-api-path-slug: triggerstags-get
      parameters:
      - in: query
        name: count
        description: Number of records to return per request
      - in: query
        name: match_name
        description: Filter by delivery tag
      - in: query
        name: offset
        description: Number of records to skip
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Triggers
      - Tags
    post:
      summary: Post Triggers Tags
      description: Post triggers tags.
      operationId: postTriggersTags
      x-api-path-slug: triggerstags-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Triggers
      - Tags
  /triggers/tags/{triggerid}:
    delete:
      summary: Delete Triggers Tags Trigger
      description: Delete triggers tags trigger.
      operationId: deleteTriggersTagsTrigger
      x-api-path-slug: triggerstagstriggerid-delete
      parameters:
      - in: path
        name: triggerid
        description: The ID for the Tag Trigger that should be deleted
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Triggers
      - Tags
      - Triggerid
    get:
      summary: Get Triggers Tags Trigger
      description: Get triggers tags trigger.
      operationId: getTriggersTagsTrigger
      x-api-path-slug: triggerstagstriggerid-get
      parameters:
      - in: path
        name: triggerid
        description: The ID for the Tag Trigger for which data should be retrieved
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Triggers
      - Tags
      - Triggerid
    put:
      summary: Put Triggers Tags Trigger
      description: Put triggers tags trigger.
      operationId: putTriggersTagsTrigger
      x-api-path-slug: triggerstagstriggerid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: triggerid
        description: The ID of the Tag Trigger that should be modified by this request
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Triggers
      - Tags
      - Triggerid
---