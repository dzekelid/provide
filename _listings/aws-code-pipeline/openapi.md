swagger: "2.0"
x-collection-name: AWS Code Pipeline
x-complete: 1
info:
  title: AWS Code Pipeline API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=PutActionRevision:
    get:
      summary: Put Action Revision
      description: Provides information to AWS CodePipeline about new revisions to
        a source.
      operationId: putActionRevision
      x-api-path-slug: actionputactionrevision-get
      parameters:
      - in: query
        name: actionName
        description: The name of the action that will process the revision
        type: string
      - in: query
        name: actionRevision
        description: Represents information about the version (or revision) of an
          action
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,     and provides an error response
        type: string
      - in: query
        name: pipelineName
        description: The name of the pipeline that will start processing the revision
          to the            source
        type: string
      - in: query
        name: PublicIp
        description: The Elastic IP address
        type: string
      - in: query
        name: stageName
        description: The name of the stage that contains the action that will act
          upon the            revision
        type: string
      responses:
        200:
          description: OK
      tags:
      - Put
      - Action
      - Revision
  /?Action=PutApprovalResult:
    get:
      summary: Put Approval Result
      description: Provides the response to a manual approval request to AWS CodePipeline.
      operationId: putApprovalResult
      x-api-path-slug: actionputapprovalresult-get
      parameters:
      - in: query
        name: actionName
        description: The name of the action for which approval is requested
        type: string
      - in: query
        name: AllocationId
        description: '[EC2-VPC] The allocation ID'
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: pipelineName
        description: The name of the pipeline that contains the action
        type: string
      - in: query
        name: PublicIp
        description: '[EC2-Classic] The Elastic IP address'
        type: string
      - in: query
        name: result
        description: Represents information about the result of the approval request
        type: string
      - in: query
        name: stageName
        description: The name of the stage that contains the action
        type: string
      - in: query
        name: token
        description: The system-generated token used to identify a unique approval
          request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Put
      - Approval
      - Result