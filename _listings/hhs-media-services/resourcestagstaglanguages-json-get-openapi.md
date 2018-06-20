---
swagger: "2.0"
x-collection-name: HHS Media Services
x-complete: 0
info:
  title: HHS Media Services Get TagLanguages
  description: Returns the list of TagLanguages
  termsOfService: http://www.hhs.gov/web/socialmedia/policies/tos.html#ready
  version: "2"
host: api.digitalmedia.hhs.gov
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /resources/tags.json:
    get:
      summary: Get Tags
      description: Returns the list of Tags matching the specified query parameters
        in the specified 'format'.
      operationId: getTags
      x-api-path-slug: resourcestags-json-get
      parameters:
      - in: query
        name: max
        description: The maximum number of records to return
      - in: query
        name: mediaId
        description: Return tags associated with the supplied media id
      - in: query
        name: name
        description: Return tags[s] matching the supplied name
      - in: query
        name: nameContains
        description: Return tags which contain the supplied partial name
      - in: query
        name: offset
        description: Return records starting at the offset index
      - in: query
        name: sort
        description: The name of the property to which sorting will be applied
      - in: query
        name: typeId
        description: Return tags belonging to the supplied tag type id
      - in: query
        name: typeName
        description: Return tags belonging to the supplied tag type name
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Tags
  /resources/tags/tagLanguages.json:
    get:
      summary: Get TagLanguages
      description: Returns the list of TagLanguages
      operationId: getTagLanguages
      x-api-path-slug: resourcestagstaglanguages-json-get
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Tags
      - TagLanguages
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