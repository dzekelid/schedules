{
  "info": {
    "name": "Azure DevTest Labs API Schedules List Applicable",
    "_postman_id": "c912d37f-c938-49d4-a2ec-28571afff682",
    "description": "Lists all applicable schedules",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "schedules",
      "item": [
        {
          "id": "928237b4-a94b-44de-9989-d2c2d8e68de4",
          "name": "Schedules_ListApplicable",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.DevTestLab/labs/:labName/schedules/:name/listApplicable"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "labName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all applicable schedules"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d735abd-5226-4fef-a981-f321e71c3388"
            }
          ]
        }
      ]
    }
  ]
}