---
swagger: "2.0"
info:
  title: AWS WorkSpaces Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeTags:
    get:
      summary: ' Describe Tags '
      description: Describes tags for a WorkSpace
      operationId: describeTags
      parameters:
      - in: query
        name: ResourceId
        description: The resource ID of the request
        type: string
      responses:
        200:
          description: OK
      tags:
      - tags
definitions: []
x-collection-name: AWS WorkSpaces
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