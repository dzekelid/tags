---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Tags Get List Photo
  description: Get the tag list for a given photo.
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
  /rest/?method=flickr.machinetags.getRecentValues:
    get:
      summary: Machinetags Get Recent Values
      description: Fetch recently used (or created) machine tags values.
      operationId: getRestMethodFlickr.machinetags.getrecentvalues
      x-api-path-slug: restmethodflickr-machinetags-getrecentvalues-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: namespace
        description: A namespace that all values should be restricted to
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of values to return per page
      - in: query
        name: predicate
        description: A predicate that all values should be restricted to
      responses:
        200:
          description: OK
      tags:
      - Machinetags
      - GetRecentValues
  /rest/?method=flickr.machinetags.getValues:
    get:
      summary: Machinetags Get Values
      description: Return a list of unique values for a namespace and predicate.
      operationId: getRestMethodFlickr.machinetags.getvalues
      x-api-path-slug: restmethodflickr-machinetags-getvalues-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: namespace
        description: A namespace that all values should be restricted to
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of values to return per page
      - in: query
        name: predicate
        description: A predicate that all values should be restricted to
      responses:
        200:
          description: OK
      tags:
      - Machinetags
      - GetValues
  /rest/?method=flickr.photos.addTags:
    post:
      summary: Photos Add Tags
      description: Add tags to a photo.
      operationId: postRestMethodFlickr.photos.addtags
      x-api-path-slug: restmethodflickr-photos-addtags-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: photo_id
        description: The id of the photo to add tags to
      - in: query
        name: tags
        description: The tags to add to the photo
      responses:
        200:
          description: OK
      tags:
      - Photos
      - AddTags
  /rest/?method=flickr.photos.setTags:
    post:
      summary: Photos Set Tags
      description: Set the tags for a photo.
      operationId: postRestMethodFlickr.photos.settags
      x-api-path-slug: restmethodflickr-photos-settags-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: photo_id
        description: The id of the photo to set the tags for
      - in: query
        name: tags
        description: All tags for the photo (as a single space-delimited string)
      responses:
        200:
          description: OK
      tags:
      - Photos
      - SetTags
  /rest/?method=flickr.places.placesForTags:
    get:
      summary: Places Places For Tags
      description: Return a list of the top 100 unique places clustered by a given
        placetype for set of tags or machine tags.
      operationId: getRestMethodFlickr.places.placesfortags
      x-api-path-slug: restmethodflickr-places-placesfortags-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: machine_tags
        description: Machine tags
      - in: query
        name: machine_tag_mode
        description: Either any for an OR combination of tags, or all for an AND combination
      - in: query
        name: max_taken_date
        description: Maximum taken date
      - in: query
        name: max_upload_date
        description: Maximum upload date
      - in: query
        name: min_taken_date
        description: Minimum taken date
      - in: query
        name: min_upload_date
        description: Minimum upload date
      - in: query
        name: place_id
        description: A Flickr Places identifier to use to filter photo clusters
      - in: query
        name: place_type_id
        description: The numeric ID for a specific place type to cluster photos by
      - in: query
        name: tags
        description: A comma-delimited list of tags
      - in: query
        name: tag_mode
        description: Either any for an OR combination of tags, or all for an AND combination
      - in: query
        name: threshold
        description: The minimum number of photos that a place type must have to be
          included
      - in: query
        name: woe_id
        description: A Where on Earth (WOE) identifier to use to filter photo clusters
      responses:
        200:
          description: OK
      tags:
      - Places
      - PlacesForTags
  /rest/?method=flickr.places.tagsForPlace:
    get:
      summary: Places Tags For Place
      description: Return a list of the top 100 unique tags for a Flickr Places or
        Where on Earth (WOE) ID.
      operationId: getRestMethodFlickr.places.tagsforplace
      x-api-path-slug: restmethodflickr-places-tagsforplace-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: max_taken_date
        description: Maximum taken date
      - in: query
        name: max_upload_date
        description: Maximum upload date
      - in: query
        name: min_taken_date
        description: Minimum taken date
      - in: query
        name: min_upload_date
        description: Minimum upload date
      - in: query
        name: place_id
        description: A Flickr Places identifier to use to filter photo clusters
      - in: query
        name: woe_id
        description: A Where on Earth (WOE) identifier to use to filter photo clusters
      responses:
        200:
          description: OK
      tags:
      - Places
      - TagsForPlace
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