---
swagger: "2.0"
x-collection-name: Azure Automation
x-complete: 0
info:
  title: Azure Automation API Schedule Delete
  version: 1.0.0
  description: Delete the schedule identified by schedule name.
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/jobSchedules/{jobScheduleId}
  : delete:
      summary: Job Schedule Delete
      description: Delete the job schedule identified by job schedule name.
      operationId: JobSchedule_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamejobschedulesjobscheduleid-delete
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: jobScheduleId
        description: The job schedule name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Job
      - Schedule
    get:
      summary: Job Schedule Get
      description: Retrieve the job schedule identified by job schedule name.
      operationId: JobSchedule_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamejobschedulesjobscheduleid-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: jobScheduleId
        description: The job schedule name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Job
      - Schedule
    put:
      summary: Job Schedule Create
      description: Create a job schedule.
      operationId: JobSchedule_Create
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamejobschedulesjobscheduleid-put
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: jobScheduleId
        description: The job schedule name
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The parameters supplied to the create job schedule operation
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Job
      - Schedule
      - Create
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/jobSchedules
  : get:
      summary: Job Schedule List By Automation Account
      description: Retrieve a list of job schedules.
      operationId: JobSchedule_ListByAutomationAccount
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamejobschedules-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Job
      - Schedule
      - List
      - Automation
      - Account
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/schedules/{scheduleName}
  : put:
      summary: Schedule Create Or Update
      description: Create a schedule.
      operationId: Schedule_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnameschedulesschedulename-put
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The parameters supplied to the create or update schedule operation
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: scheduleName
        description: The schedule name
      responses:
        200:
          description: OK
      tags:
      - Schedule
      - Or
    patch:
      summary: Schedule Update
      description: Update the schedule identified by schedule name.
      operationId: Schedule_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnameschedulesschedulename-patch
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The parameters supplied to the update schedule operation
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: scheduleName
        description: The schedule name
      responses:
        200:
          description: OK
      tags:
      - Schedule
    get:
      summary: Schedule Get
      description: Retrieve the schedule identified by schedule name.
      operationId: Schedule_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnameschedulesschedulename-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: query
        name: No Name
      - in: path
        name: scheduleName
        description: The schedule name
      responses:
        200:
          description: OK
      tags:
      - Schedule
    delete:
      summary: Schedule Delete
      description: Delete the schedule identified by schedule name.
      operationId: Schedule_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnameschedulesschedulename-delete
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: query
        name: No Name
      - in: path
        name: scheduleName
        description: The schedule name
      responses:
        200:
          description: OK
      tags:
      - Schedule
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/schedules
  : get:
      summary: Schedule List By Automation Account
      description: Retrieve a list of schedules.
      operationId: Schedule_ListByAutomationAccount
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnameschedules-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Schedule
      - List
      - Automation
      - Account
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