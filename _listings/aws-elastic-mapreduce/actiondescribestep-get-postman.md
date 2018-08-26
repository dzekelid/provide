{
  "info": {
    "name": "AWS Elastic MapReduce API Describe Step",
    "_postman_id": "2cb8baf9-ef56-400e-bc56-58bde06b3d37",
    "description": "Provides more detail about the cluster step.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Job Flow Steps",
      "item": [
        {
          "id": "6a600363-979f-49d6-9e72-a6e5d84f932c",
          "name": "addJobFlowSteps",
          "request": {
            "url": "http://example.com/api/?Action=AddJobFlowSteps?JobFlowId=JobFlowId&Steps=Steps",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "AddJobFlowSteps adds new steps to a running job flow."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "886f4a0b-e207-440f-985d-3cf7cf9180f1"
            }
          ]
        }
      ]
    },
    {
      "name": "Steps",
      "item": [
        {
          "id": "37e8bb30-b8c4-458f-8a1c-524a87a3b8f5",
          "name": "cancelSteps",
          "request": {
            "url": "http://example.com/api/?Action=CancelSteps?ClusterId=ClusterId&StepIds=StepIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels a pending step or steps in a running cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff1fed19-eaae-48cf-9b7a-80d754200434"
            }
          ]
        },
        {
          "id": "58f19ce5-7aef-4f75-995a-e10b41ec1c60",
          "name": "describeStep",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStep?ClusterId=ClusterId&StepId=StepId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides more detail about the cluster step."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe56fc58-ccae-45c9-94f4-bc455a4df2d2"
            }
          ]
        }
      ]
    }
  ]
}