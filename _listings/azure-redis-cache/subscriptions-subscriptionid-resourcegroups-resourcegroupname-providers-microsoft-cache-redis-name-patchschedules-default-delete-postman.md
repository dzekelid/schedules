{
  "info": {
    "name": "Azure Redis Cache API Patch Schedules Delete",
    "_postman_id": "0885e5d6-82d5-4071-9a9a-18fe613a1dfc",
    "description": "Deletes the patching schedule of a redis cache (requires Premium SKU).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "schedules",
      "item": [
        {
          "id": "8d1e6a84-0e4a-49f4-8307-5aef8e877dd9",
          "name": "PatchSchedules_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Cache/Redis/:name/patchSchedules/default"
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
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the patching schedule of a redis cache (requires Premium SKU)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6613771-caf4-4738-9afa-02391d7c30e5"
            }
          ]
        }
      ]
    }
  ]
}