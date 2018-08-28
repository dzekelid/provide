swagger: "2.0"
x-collection-name: AWS Database Migration Service
x-complete: 1
info:
  title: AWS Database Migration Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeCertificates:
    get:
      summary: Describe Certificates
      description: Provides a description of the certificate.
      operationId: describeCertificates
      x-api-path-slug: actiondescribecertificates-get
      parameters:
      - in: query
        name: Filters
        description: Filters applied to the certificate described in the form of key-value
          pairs
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous         request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates