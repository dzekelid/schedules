{
  "info": {
    "name": "Azure DevTest Labs API Global Schedules Execute",
    "_postman_id": "4ba1ff17-af47-4054-9aa5-93429ace6ba2",
    "description": "Execute a schedule. This operation can take a while to complete.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "global schedules",
      "item": [
        {
          "id": "0d35ad77-6cab-4ae7-b85f-1f867e26ea77",
          "name": "GlobalSchedules_Execute",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.DevTestLab/schedules/:name/execute"
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
            "description": "Execute a schedule"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4bcec45-3494-4472-ae6b-ae7867b9f49b"
            }
          ]
        }
      ]
    }
  ]
}