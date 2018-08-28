swagger: "2.0"
x-collection-name: AWS Key Management Service
x-complete: 1
info:
  title: AWS Key Management Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ScheduleKeyDeletion:
    get:
      summary: Schedule Key Deletion
      description: Schedules the deletion of a customer master key (CMK).
      operationId: scheduleKeyDeletion
      x-api-path-slug: actionschedulekeydeletion-get
      parameters:
      - in: query
        name: KeyId
        description: The unique identifier for the customer master key (CMK) to delete
        type: string
      - in: query
        name: PendingWindowInDays
        description: The waiting period, specified in number of days
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys