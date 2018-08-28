---
swagger: "2.0"
x-collection-name: AWS CloudFront
x-complete: 0
info:
  title: AWS CloudFront API Create Streaming Distribution With Tags
  version: 1.0.0
  description: Create a new streaming distribution with tags.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateDistributionWithTags:
    get:
      summary: Create Distribution With Tags
      description: Create a new distribution with tags.
      operationId: createDistributionWithTags
      x-api-path-slug: actioncreatedistributionwithtags-get
      parameters:
      - in: query
        name: CreateDistributionWithTagsRequest
        description: Root level tag for the CreateDistributionWithTagsRequest parameters
        type: string
      - in: query
        name: DistributionConfigWithTags
        description: The distributions configuration information
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,     and provides an error response
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance to unlink from the VPC
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC to which the instance is linked
        type: string
      responses:
        200:
          description: OK
      tags:
      - Distribution
      - Tags
  /?Action=CreateStreamingDistributionWithTags:
    get:
      summary: Create Streaming Distribution With Tags
      description: Create a new streaming distribution with tags.
      operationId: createStreamingDistributionWithTags
      x-api-path-slug: actioncreatestreamingdistributionwithtags-get
      parameters:
      - in: query
        name: CreateStreamingDistributionWithTagsRequest
        description: Root level tag for the CreateStreamingDistributionWithTagsRequest
          parameters
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,     and provides an error response
        type: string
      - in: query
        name: StreamingDistributionConfigWithTags
        description: The streaming distributions configuration information
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - Streaming
      - Distribution
      - Tags
  /?Action=ListTagsForResource:
    get:
      summary: List Tags For Resource
      description: List tags for a CloudFront resource.
      operationId: listTagsForResource
      x-api-path-slug: actionlisttagsforresource-get
      parameters:
      - in: query
        name: DhcpOptionsId
        description: The ID of the DHCP options set
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Resource
        description: An ARN of a CloudFront resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Tags
      - Resource
  /?Action=TagResource:
    get:
      summary: Tag Resource
      description: Add tags to a CloudFront resource.
      operationId: tagResource
      x-api-path-slug: actiontagresource-get
      parameters:
      - in: query
        name: DhcpOptionsId.N
        description: The IDs of one or more DHCP options sets
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: Resource
        description: An ARN of a CloudFront resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tag
      - Resource
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