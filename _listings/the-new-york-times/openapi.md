---
swagger: "2.0"
x-collection-name: The New York Times
x-complete: 1
info:
  title: New York Times
  description: you-already-know-that-nytimes-com-is-an-unparalleled-source-of-news-and-information--but-now-its-a-premier-source-of-data-too--why-just-read-the-news-when-you-can-hack-it
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
---