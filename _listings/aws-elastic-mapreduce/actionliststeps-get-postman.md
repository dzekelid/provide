{
  "info": {
    "name": "AWS Elastic MapReduce API List Steps",
    "_postman_id": "fca5b461-741a-44e1-9abb-9c81c72ba07a",
    "description": "Provides a list of steps for the cluster in reverse order unless you specify stepIds with the request.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Job Flow Steps",
      "item": [
        {
          "id": "f97cee2f-4b0a-483c-97ab-5d6170dad318",
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
              "id": "dd75694d-1b85-4bba-80da-2caa114192d8"
            }
          ]
        }
      ]
    },
    {
      "name": "Steps",
      "item": [
        {
          "id": "ac6875b0-81a0-43e0-8feb-78deb8e49ae6",
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
              "id": "25bd224b-3c69-4d9e-8bdf-5b8a3cc2e6eb"
            }
          ]
        },
        {
          "id": "f2ac818d-ffda-4b51-bc48-51700784c35b",
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
              "id": "5570cf73-8f7a-4595-a578-2a05ca0c023c"
            }
          ]
        },
        {
          "id": "28f05d7c-0644-4315-894e-c05ede396596",
          "name": "listSteps",
          "request": {
            "url": "http://example.com/api/?Action=ListSteps?ClusterId=ClusterId&Marker=Marker&StepIds=StepIds&StepStates=StepStates",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides a list of steps for the cluster in reverse order unless you specify stepIds with the request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e26fc495-f846-4da6-97f7-12f2cc89cee2"
            }
          ]
        }
      ]
    }
  ]
}