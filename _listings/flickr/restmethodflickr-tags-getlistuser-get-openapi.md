---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Tags Get List User
  description: Get the tag list for a given user (or the currently logged in user).
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
  /rest/?method=flickr.tags.getClusters:
    get:
      summary: Tags Get Clusters
      description: Returns a list of tag clusters for the given tag.
      operationId: getRestMethodFlickr.tags.getclusters
      x-api-path-slug: restmethodflickr-tags-getclusters-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: tag
        description: The tag to fetch clusters for
      responses:
        200:
          description: OK
      tags:
      - Tags
      - GetClusters
  /rest/?method=flickr.tags.getHotList:
    get:
      summary: Tags Get Hot List
      description: Returns a list of hot tags for the given period.
      operationId: getRestMethodFlickr.tags.gethotlist
      x-api-path-slug: restmethodflickr-tags-gethotlist-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: count
        description: The number of tags to return
      - in: query
        name: format
        description: Response format
      - in: query
        name: period
        description: The period for which to fetch hot tags
      responses:
        200:
          description: OK
      tags:
      - Tags
      - GetHotList
  /rest/?method=flickr.tags.getListPhoto:
    get:
      summary: Tags Get List Photo
      description: Get the tag list for a given photo.
      operationId: getRestMethodFlickr.tags.getlistphoto
      x-api-path-slug: restmethodflickr-tags-getlistphoto-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: photo_id
        description: The id of the photo to return tags for
      responses:
        200:
          description: OK
      tags:
      - Tags
      - GetListPhoto
  /rest/?method=flickr.tags.getListUser:
    get:
      summary: Tags Get List User
      description: Get the tag list for a given user (or the currently logged in user).
      operationId: getRestMethodFlickr.tags.getlistuser
      x-api-path-slug: restmethodflickr-tags-getlistuser-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: user_id
        description: The NSID of the user to fetch the tag list for
      responses:
        200:
          description: OK
      tags:
      - Tags
      - GetListUser
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