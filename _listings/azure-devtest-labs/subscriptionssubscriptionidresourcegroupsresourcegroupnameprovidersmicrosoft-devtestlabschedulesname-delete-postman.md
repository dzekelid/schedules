{
  "info": {
    "name": "Azure DevTest Labs API Global Schedules Delete",
    "_postman_id": "416e4b1a-7df5-44d8-aeb1-4b7568a8c777",
    "description": "Delete schedule.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "global schedules",
      "item": [
        {
          "id": "34426cb0-cb69-4c23-95f1-7ecc0f611a29",
          "name": "GlobalSchedules_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.DevTestLab/schedules/:name"
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete schedule"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "200fcf57-222b-4ead-8e23-d6ab6bd1a6d2"
            }
          ]
        }
      ]
    }
  ]
}