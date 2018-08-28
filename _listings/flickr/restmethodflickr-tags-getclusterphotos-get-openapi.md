---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Tags Get Cluster Photos
  description: Returns the first 24 photos for a given tag cluster.
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
  /rest/?method=flickr.tags.getClusterPhotos:
    get:
      summary: Tags Get Cluster Photos
      description: Returns the first 24 photos for a given tag cluster.
      operationId: getRestMethodFlickr.tags.getclusterphotos
      x-api-path-slug: restmethodflickr-tags-getclusterphotos-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: cluster_id
        description: The top three tags for the cluster, separated by dashes (just
          like the url)
      - in: query
        name: format
        description: Response format
      - in: query
        name: tag
        description: The tag that this cluster belongs to
      responses:
        200:
          description: OK
      tags:
      - Tags
      - GetClusterPhotos
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