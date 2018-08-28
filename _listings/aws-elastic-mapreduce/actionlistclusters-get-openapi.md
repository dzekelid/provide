---
swagger: "2.0"
x-collection-name: AWS Elastic MapReduce
x-complete: 0
info:
  title: AWS Elastic MapReduce API List Clusters
  version: 1.0.0
  description: Provides the status of all clusters visible to this AWS account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeCluster:
    get:
      summary: Describe Cluster
      description: Provides cluster-level details including status, hardware and software
        configuration, VPC settings, and so on.
      operationId: describeCluster
      x-api-path-slug: actiondescribecluster-get
      parameters:
      - in: query
        name: ClusterId
        description: The identifier of the cluster to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=DescribeSecurityConfiguration:
    get:
      summary: Describe Security Configuration
      description: Provides the details of a security configuration by returning the
        configuration JSON.
      operationId: describeSecurityConfiguration
      x-api-path-slug: actiondescribesecurityconfiguration-get
      parameters:
      - in: query
        name: Name
        description: The name of the security configuration
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Configurations
  /?Action=DescribeStep:
    get:
      summary: Describe Step
      description: Provides more detail about the cluster step.
      operationId: describeStep
      x-api-path-slug: actiondescribestep-get
      parameters:
      - in: query
        name: ClusterId
        description: The identifier of the cluster with steps to describe
        type: string
      - in: query
        name: StepId
        description: The identifier of the step to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Steps
  /?Action=ListBootstrapActions:
    get:
      summary: List Bootstrap Actions
      description: Provides information about the bootstrap actions associated with
        a cluster.
      operationId: listBootstrapActions
      x-api-path-slug: actionlistbootstrapactions-get
      parameters:
      - in: query
        name: ClusterId
        description: The cluster identifier for the bootstrap actions to list
        type: string
      - in: query
        name: Marker
        description: The pagination token that indicates the next set of results to
          retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Bootstrap Actions
  /?Action=ListClusters:
    get:
      summary: List Clusters
      description: Provides the status of all clusters visible to this AWS account.
      operationId: listClusters
      x-api-path-slug: actionlistclusters-get
      parameters:
      - in: query
        name: ClusterStates
        description: The cluster state filters to apply when listing clusters
        type: string
      - in: query
        name: CreatedAfter
        description: The creation date and time beginning value filter for listing
          clusters
        type: string
      - in: query
        name: CreatedBefore
        description: The creation date and time end value filter for listing clusters
        type: string
      - in: query
        name: Marker
        description: The pagination token that indicates the next set of results to
          retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
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