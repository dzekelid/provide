---
swagger: "2.0"
x-collection-name: AWS Key Management Service
x-complete: 0
info:
  title: AWS Key Management Service API Describe Key
  version: 1.0.0
  description: Provides detailed information about the specified customer master key.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeKey:
    get:
      summary: Describe Key
      description: Provides detailed information about the specified customer master
        key.
      operationId: describeKey
      x-api-path-slug: actiondescribekey-get
      parameters:
      - in: query
        name: GrantTokens
        description: A list of grant tokens
        type: string
      - in: query
        name: KeyId
        description: A unique identifier for the customer master key
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
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