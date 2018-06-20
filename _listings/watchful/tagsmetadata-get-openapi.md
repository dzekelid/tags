---
swagger: "2.0"
x-collection-name: Watchful
x-complete: 0
info:
  title: Watchful Get The List Of Fields
  description: Returns a list of fields
  version: 1.0.0
host: watchful.li
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /reports/tags/{id}:
    get:
      summary: Find Sites By ID
      description: Returns a report based on a site ID
      operationId: reports.tags.id.get
      x-api-path-slug: reportstagsid-get
      parameters:
      - in: query
        name: compare
        description: Define if you want show previous values in Google Analytics graph
      - in: query
        name: from
        description: Start of the report, format YYYY-MM-DD, default today-30day
      - in: path
        name: id
        description: ID that needs to be fetched
      - in: query
        name: log_type
        description: Type of the log to show in the report
      - in: query
        name: reports
        description: 'Type of reports separate by comas: Ga,Logs,Uptime'
      - in: query
        name: to
        description: End of the report, format YYYY-MM-DD, default today
      responses:
        200:
          description: OK
      tags:
      - Reports
      - Tags
      - Id
  /sites/{id}/tags:
    get:
      summary: Return Tags For A Specific Website
      description: Return tags for a specific website
      operationId: sites.id.tags.get
      x-api-path-slug: sitesidtags-get
      parameters:
      - in: query
        name: fields
        description: 'Fields to return separate by comas: name,id'
      - in: path
        name: id
        description: ID of the website
      - in: query
        name: limit
        description: Number of object to return (max 100, default 25)
      - in: query
        name: limitstart
        description: Start of the return (default 0)
      - in: query
        name: name
        description: Do a LIKE search, you can also use %
      - in: query
        name: order
        description: ORDER by this field
      - in: query
        name: type
        description: Bootstrap color of the tag
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Tags
    post:
      summary: Add Tags For A Specific Website
      description: Add tags for a specific website
      operationId: postTags
      x-api-path-slug: sitesidtags-post
      parameters:
      - in: body
        name: body
        description: JSON object Tag
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of the website
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Tags
  /tags:
    get:
      summary: Get A List Of Tags
      description: Returns a list of tags
      operationId: tags.get
      x-api-path-slug: tags-get
      parameters:
      - in: query
        name: fields
        description: 'Fields to return separate by comas: name,id'
      - in: query
        name: limit
        description: Number of object to return (max 100, default 25)
      - in: query
        name: limitstart
        description: Start of the return (default 0)
      - in: query
        name: name
        description: Do a LIKE search, you can also use %
      - in: query
        name: order
        description: ORDER by this field separete by comas
      - in: query
        name: type
        description: Bootstrap color of the tag
      responses:
        200:
          description: OK
      tags:
      - Tags
    post:
      summary: Create A Tag
      description: Create a tag
      operationId: CreateTags
      x-api-path-slug: tags-post
      parameters:
      - in: body
        name: body
        description: JSON object Tag
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Tags
  /tags/metadata:
    get:
      summary: Get The List Of Fields
      description: Returns a list of fields
      operationId: tags.metadata.get
      x-api-path-slug: tagsmetadata-get
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Metadata
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