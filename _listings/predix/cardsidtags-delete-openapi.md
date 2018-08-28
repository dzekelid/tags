---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Views Deletes all tags of this Card.
  version: 1.0.0
  description: Deletes all tags of this card..
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v2/config/orchestrations/defaulttagquery:
    get:
      summary: Get the default tag query corresponding for the tenant.
      description: Returns all information (query string, fieldnamespecifier, tagnamespecifer,
        description etc.) associated with the default tag query. An error is returned
        if tag query does not exist for the tenant.
      operationId: retrieveDefaultTagQuery
      x-api-path-slug: apiv2configorchestrationsdefaulttagquery-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Default
      - Tag
      - Query
      - Correspondingthe
      - Tenant
    post:
      summary: Create the default tag query corresponding for the tenant.
      description: Creates the default tag query including all information (query
        string, fieldnamespecifier, tagnamespecifer, description etc.) associated
        with the query.
      operationId: createDefaultTagQuery
      x-api-path-slug: apiv2configorchestrationsdefaulttagquery-post
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: body
        name: body
        description: tag names default query
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Default
      - Tag
      - Query
      - Correspondingthe
      - Tenant
    put:
      summary: Update the default tag query for the tenant.
      description: Updates the default tag query including all information (query
        string, fieldnamespecifier, tagnamespecifer, description etc.) associated
        with the query.
      operationId: updateDefaultTagQuery
      x-api-path-slug: apiv2configorchestrationsdefaulttagquery-put
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: body
        name: body
        description: tag names default query
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Default
      - Tag
      - Querythe
      - Tenant
    delete:
      summary: Delete the default tag query for the tenant.
      description: Deletes the default tag query.
      operationId: deleteDefaultTagQuery
      x-api-path-slug: apiv2configorchestrationsdefaulttagquery-delete
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Default
      - Tag
      - Querythe
      - Tenant
  /v1/tags:
    get:
      summary: Get all tags
      description: "Return all the ingested tag names.Response JSON (Status 200){\n\t\"results\":
        [\n\t\t\"ALT_SENSOR\",\n\t\t\"tagName1\",\n\t\t\"tagName2\"\n\t]\n}"
      operationId: getMetricNames
      x-api-path-slug: v1tags-get
      parameters:
      - in: header
        name: Authorization
      - in: header
        name: Content-Type
      - in: header
        name: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Tags
  /dags/tags:
    get:
      summary: Get Dags Tags
      description: Get dags tags.
      operationId: getAllDagTagsUsingGET
      x-api-path-slug: dagstags-get
      responses:
        200:
          description: Successful response
      tags:
      - Dags
      - Tags
  /dependencies/tags:
    get:
      summary: Get Dependencies Tags
      description: Get dependencies tags.
      operationId: getAllDependencyTagsUsingGET
      x-api-path-slug: dependenciestags-get
      responses:
        200:
          description: Successful response
      tags:
      - Dependencies
      - Tags
  /flow-templates/tags:
    get:
      summary: Get Flow Templates Tags
      description: Get flow templates tags.
      operationId: getAllFlowTemplateTagsUsingGET
      x-api-path-slug: flowtemplatestags-get
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Tags
  /flow-templates/{flowTemplateId}/flows/{flowId}/tags:
    get:
      summary: Get Flow Templates Flowtemplateid Flows Flowid Tags
      description: Get flow templates flowtemplateid flows flowid tags.
      operationId: getFlowTagsUsingGET
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowidtags-get
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
      - Tags
    post:
      summary: Post Flow Templates Flowtemplateid Flows Flowid Tags
      description: Post flow templates flowtemplateid flows flowid tags.
      operationId: saveFlowTagsUsingPOST_1
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowidtags-post
      parameters:
      - in: path
        name: flowId
        description: flowId
      - in: body
        name: tags
        description: tags
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
      - Tags
  /flow-templates/{flowTemplateId}/tags:
    get:
      summary: Get Flow Templates Flowtemplateid Tags
      description: Get flow templates flowtemplateid tags.
      operationId: getTemplateTagsUsingGET
      x-api-path-slug: flowtemplatesflowtemplateidtags-get
      parameters:
      - in: path
        name: flowTemplateId
        description: flowTemplateId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Tags
    post:
      summary: Post Flow Templates Flowtemplateid Tags
      description: Post flow templates flowtemplateid tags.
      operationId: saveTemplateTagsUsingPOST
      x-api-path-slug: flowtemplatesflowtemplateidtags-post
      parameters:
      - in: path
        name: flowTemplateId
        description: flowTemplateId
      - in: body
        name: tags
        description: tags
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Tags
  /flows/tags:
    get:
      summary: Get Flows Tags
      description: Get flows tags.
      operationId: getAllFlowTagsUsingGET
      x-api-path-slug: flowstags-get
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Tags
  /flows/{flowId}/tags:
    post:
      summary: Post Flows Flowid Tags
      description: Post flows flowid tags.
      operationId: saveFlowTagsUsingPOST
      x-api-path-slug: flowsflowidtags-post
      parameters:
      - in: path
        name: flowId
        description: flowId
      - in: body
        name: tags
        description: tags
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowid
      - Tags
  /decks/{id}/tags:
    get:
      summary: Queries tags of Deck.
      description: Queries tags of deck..
      operationId: getDecksTags
      x-api-path-slug: decksidtags-get
      parameters:
      - in: query
        name: filter
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Queries
      - Tags
      - Of
      - Deck
    post:
      summary: Creates a new instance in tags of this Tag.
      description: Creates a new instance in tags of this tag..
      operationId: postDecksTags
      x-api-path-slug: decksidtags-post
      parameters:
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Instance
      - In
      - Tags
      - Of
      - This
      - Tag
    delete:
      summary: Deletes all tags of this Deck.
      description: Deletes all tags of this deck..
      operationId: deleteDecksTags
      x-api-path-slug: decksidtags-delete
      parameters:
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - S
      - ""
      - Tags
      - Of
      - This
      - Deck
  /decks/tags:
    get:
      summary: Get all decks by tags
      description: Get all decks by tags.
      operationId: getDecksTags
      x-api-path-slug: deckstags-get
      parameters:
      - in: query
        name: values
      responses:
        200:
          description: OK
      tags:
      - Decks
      - By
      - Tags
  /cards/{id}/tags:
    get:
      summary: Queries tags of Card.
      description: Queries tags of card..
      operationId: getCardsTags
      x-api-path-slug: cardsidtags-get
      parameters:
      - in: query
        name: filter
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Queries
      - Tags
      - Of
      - Card
    post:
      summary: Creates a new instance in tags of this Card.
      description: Creates a new instance in tags of this card..
      operationId: postCardsTags
      x-api-path-slug: cardsidtags-post
      parameters:
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Instance
      - In
      - Tags
      - Of
      - This
      - Card
    delete:
      summary: Deletes all tags of this Card.
      description: Deletes all tags of this card..
      operationId: deleteCardsTags
      x-api-path-slug: cardsidtags-delete
      parameters:
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - S
      - ""
      - Tags
      - Of
      - This
      - Card
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