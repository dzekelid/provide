---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateCustomerGateway:
    get:
      summary: Create Customer Gateway
      description: Provides information to AWS about your VPN customer gateway device.
      operationId: createcustomergateway
      x-api-path-slug: actioncreatecustomergateway-get
      parameters:
      - in: query
        name: CustomerGatewayId
        description: The ID of the customer gateway
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,             and provides an error response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Gateway
---