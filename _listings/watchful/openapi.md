---
swagger: "2.0"
x-collection-name: Watchful
x-complete: 1
info:
  title: Watchful
  description: watchful-resulted-from-the-need-for-a-single-unified-dashboard-to-easily-monitor-all-of-the-web-sites-in-our-portfolios--after-years-of-evolution-our-solution-has-matured-into-a-simple-complete-and-professional-service--
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
  /tags/{id}:
    delete:
      summary: Delete A Specific Tag
      description: Delete a specific tag
      operationId: tags.id.delete
      x-api-path-slug: tagsid-delete
      parameters:
      - in: path
        name: id
        description: ID of tag that needs to be deleted
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Id
    get:
      summary: Find Tag By ID
      description: Returns a tag based on ID
      operationId: getTagById
      x-api-path-slug: tagsid-get
      parameters:
      - in: query
        name: fields
        description: 'Fields to return separate by comas: name,id'
      - in: path
        name: id
        description: ID of tag that needs to be fetched
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Id
    put:
      summary: Update A Tag
      description: Update a tag
      operationId: UpdateTag
      x-api-path-slug: tagsid-put
      parameters:
      - in: body
        name: body
        description: JSON object of the updated tag
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of tag
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Id
  /tags/{id}/sites:
    get:
      summary: Find Sites By Tag ID
      description: Returns a list of sites based with a specific tag id
      operationId: getSitesByTags
      x-api-path-slug: tagsidsites-get
      parameters:
      - in: query
        name: access_url
        description: Do a LIKE search, you can also use %
      - in: query
        name: error
        description: have errors
      - in: query
        name: fields
        description: 'Fields to return separate by comas: name,id'
      - in: path
        name: id
        description: ID of tag that needs to be fetched
      - in: query
        name: ip
        description: Do a LIKE search, you can also use %
      - in: query
        name: jUpdate
        description: Joomla core update
      - in: query
        name: j_version
        description: Do a LIKE search, you can also use %
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
        name: nbUpdates
      - in: query
        name: order
        description: ORDER by this field separete by comas
      - in: query
        name: published
        description: is published
      - in: query
        name: up
        description: is the website online
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Id
      - Sites
---