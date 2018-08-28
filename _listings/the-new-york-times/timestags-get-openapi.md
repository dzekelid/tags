---
swagger: "2.0"
x-collection-name: The New York Times
x-complete: 0
info:
  title: The New York Times Times Tag
  description: With the TimesTags API, you can mine the riches of the New York Times
    tag set. The TimesTags service matches your query to the controlled vocabularies
    that fuel NYTimes.com metadata. You supply a string of characters, and the service
    returns a ranked list of suggested terms.
  termsOfService: https://developer.nytimes.com/tou
  version: 2.0.0
host: api.nytimes.com
basePath: /svc
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /timestags:
    get:
      summary: Times Tag
      description: With the TimesTags API, you can mine the riches of the New York
        Times tag set. The TimesTags service matches your query to the controlled
        vocabularies that fuel NYTimes.com metadata. You supply a string of characters,
        and the service returns a ranked list of suggested terms.
      operationId: getTimesTag
      x-api-path-slug: timestags-get
      parameters:
      - in: query
        name: filter
        description: 'If you do not specify a value for filter (see the Optional Parameters),
          your query will be matched to tags in all four Times dictionaries: subject,
          geographic location, organization and person'
      - in: query
        name: max
        description: Sets the maximum number of results
      - in: query
        name: query
        description: Your search query
      responses:
        200:
          description: OK
      tags:
      - Tags
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