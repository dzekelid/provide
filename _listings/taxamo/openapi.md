---
swagger: "2.0"
x-collection-name: Taxamo
x-complete: 1
info:
  title: Taxamo
  description: taxamos-elegant-suite-of-apis-and-comprehensive-reporting-dashboard-enables-digital-merchants-to-easily-comply-with-eu-regulatory-requirements-on-tax-calculation-evidence-collection-tax-return-creation-and-data-storage-
  version: "1"
host: api.taxamo.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/geoip/{ip}:
    get:
      summary: Locate Provided IP Address
      description: Locate provided ip address.
      operationId: locateGivenIP
      x-api-path-slug: apiv1geoipip-get
      parameters:
      - in: path
        name: ip
        description: IP address
      responses:
        200:
          description: OK
      tags:
      - Locate
      - Provided
      - IP
      - Ress
---