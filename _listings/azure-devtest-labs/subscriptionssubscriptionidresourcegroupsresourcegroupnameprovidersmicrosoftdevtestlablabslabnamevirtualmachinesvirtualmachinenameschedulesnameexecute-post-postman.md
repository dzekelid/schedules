{
  "info": {
    "name": "Azure DevTest Labs API Virtual Machine Schedules Execute",
    "_postman_id": "0ebc7a6c-1561-4e5a-bbba-2b7b76c734a5",
    "description": "Execute a schedule. This operation can take a while to complete.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "virtual machine schedules execute",
      "item": [
        {
          "id": "667b6d96-e6f2-4bdc-99a0-3794d447eec6",
          "name": "VirtualMachineSchedules_Execute",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.DevTestLab/labs/:labName/virtualmachines/:virtualMachineName/schedules/:name/execute"
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
                  "id": "virtualMachineName",
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
              "id": "f087dc20-7379-42c3-9148-79a9c048f65e"
            }
          ]
        }
      ]
    }
  ]
}