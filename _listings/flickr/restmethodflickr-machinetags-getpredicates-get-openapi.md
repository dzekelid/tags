---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Machinetags Get Predicates
  description: Return a list of unique predicates, optionally limited by a given namespace.
  version: 1.0.0
host: api.flickr.com
basePath: /services/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/?method=flickr.machinetags.getNamespaces:
    get:
      summary: Machinetags Get Namespaces
      description: Return a list of unique namespaces, optionally limited by a given
        predicate, in alphabetical order.
      operationId: getRestMethodFlickr.machinetags.getnamespaces
      x-api-path-slug: restmethodflickr-machinetags-getnamespaces-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of photos to return per page
      - in: query
        name: predicate
        description: Limit the list of namespaces returned to those that have the
          following predicate
      responses:
        200:
          description: OK
      tags:
      - Machinetags
      - GetNamespaces
  /rest/?method=flickr.machinetags.getPairs:
    get:
      summary: Machinetags Get Pairs
      description: Return a list of unique namespace and predicate pairs, optionally
        limited by predicate or namespace, in alphabetical order.
      operationId: getRestMethodFlickr.machinetags.getpairs
      x-api-path-slug: restmethodflickr-machinetags-getpairs-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: namespace
        description: Limit the list of pairs returned to those that have the following
          namespace
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of photos to return per page
      - in: query
        name: predicate
        description: Limit the list of namespaces returned to those that have the
          following predicate
      responses:
        200:
          description: OK
      tags:
      - Machinetags
      - GetPairs
  /rest/?method=flickr.machinetags.getPredicates:
    get:
      summary: Machinetags Get Predicates
      description: Return a list of unique predicates, optionally limited by a given
        namespace.
      operationId: getRestMethodFlickr.machinetags.getpredicates
      x-api-path-slug: restmethodflickr-machinetags-getpredicates-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: namespace
        description: Limit the list of predicates returned to those that have the
          following namespace
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of predicates to return per page
      responses:
        200:
          description: OK
      tags:
      - Machinetags
      - GetPredicates
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