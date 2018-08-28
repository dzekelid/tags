swagger: "2.0"
x-collection-name: HHS Media Services
x-complete: 1
info:
  title: HHS Media Services
  description: div-classswaggeruiwrap-extrafooterh3common-features--behaviorsh3----div-classfeatures--------ul------------listrong-sort-paramstrong-supports-multi-column-sorting-through-the-use-of-commas-as-delimiters-and-a-hyphen-to-denote-descending-order-----------------br----------------strongspanexamplesspanstrong----------------ul--------------------lispan-classexamplenamespanspan-classdescriptionsort-results-by-name-ascendingspanli--------------------lispan-classexamplenamespanspan-classdescriptionsort-results-by-name-descendingspanli--------------------lispan-classexamplenameidspanspan-classdescriptionsort-results-by-name-descending-and-then-by-id-ascendingspanli--------------------lispan-classexampleiddatecontentauthoredspanspan-classdescriptionsort-results-by-id-ascending-and-then-date-descendingspanli----------------ul------------li------------listrongdate-formatsstrong-date-input-format-is-expected-to-be-based-on-a-hrefhttpwww-ietf-orgrfcrfc3339-txtrfc-3339a--br----------------spanstrongexamplestrongspan----------------ulli20131118t184301zliul------------li--------ul----divdiv
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
  /resources/tags/tagTypes.json:
    get:
      summary: Get TagTypes
      description: Returns the list of TagTypes
      operationId: getTagTypes
      x-api-path-slug: resourcestagstagtypes-json-get
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Tags
      - TagTypes
  /resources/tags/{id}.json:
    get:
      summary: Get Tag by ID
      description: Returns the Tag identified by the 'id' in the specified 'format'.
      operationId: getTagById
      x-api-path-slug: resourcestagsid-json-get
      parameters:
      - in: path
        name: id
        description: The id of the record to look up
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Tags
      - Id
  /resources/tags/{id}/media.json:
    get:
      summary: Get MediaItems for Tag
      description: Returns the list of MediaItems associated with the Tag identified
        by the 'id'.
      operationId: getMediaByTagId
      x-api-path-slug: resourcestagsidmedia-json-get
      parameters:
      - in: path
        name: id
        description: The id of the record to look up
      - in: query
        name: max
        description: The maximum number of records to return
      - in: query
        name: offset
        description: The offset of the records set to return for pagination
      - in: query
        name: sort
        description: The name of the property to which sorting will be applied
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Tags
      - Id
      - Media
  /resources/tags/{id}/related.json:
    get:
      summary: Get related Tags by ID
      description: Returns the list of Tags related to the Tag identified by the 'id'
        in the specified format.
      operationId: getRelatedTagsById
      x-api-path-slug: resourcestagsidrelated-json-get
      parameters:
      - in: path
        name: id
        description: The id of the tag to look up
      - in: query
        name: max
        description: The maximum number of records to return
      - in: query
        name: offset
        description: The offset of the records set to return for pagination
      - in: query
        name: sort
        description: The name of the property to which sorting will be applied
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Tags
      - Id
      - Related
  /resources/tags/{id}/syndicate.json:
    get:
      summary: Get MediaItems for Tag
      description: Renders the list of MediaItems associated with the Tag identified
        by the 'id'.
      operationId: renders-the-list-of-mediaitems-associated-with-the-tag-identified-by-the-id-
      x-api-path-slug: resourcestagsidsyndicate-json-get
      parameters:
      - in: query
        name: displayMethod
        description: Method used to render an html request
      - in: path
        name: id
        description: The id of the record to look up
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Tags
      - Id
      - Syndicate