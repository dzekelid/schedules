---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 0
info:
  title: 'Xibo API Action: Revert to Schedule'
  description: Send the revert to schedule action to this DisplayGroup
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /displaygroup/{displayGroupId}/action/revertToSchedule:
    post:
      summary: 'Action: Revert to Schedule'
      description: Send the revert to schedule action to this DisplayGroup
      operationId: displayGroupActionRevertToSchedule
      x-api-path-slug: displaygroupdisplaygroupidactionreverttoschedule-post
      parameters:
      - in: path
        name: displayGroupId
        description: The display group id
      responses:
        200:
          description: OK
      tags:
      - 'Action:'
      - Revert
      - To
      - Schedule
  /schedule:
    post:
      summary: Add Schedule Event
      description: Add a new scheduled event for a Campaign/Layout to be shown on
        a Display Group/Display.
      operationId: scheduleAdd
      x-api-path-slug: schedule-post
      parameters:
      - in: formData
        name: campaignId
        description: The Campaign ID to use for this Event
      - in: formData
        name: commandId
        description: The Command ID to use for this Event
      - in: formData
        name: dayPartId
        description: The Day Part for this event
      - in: formData
        name: displayGroupIds
        description: The Display Group IDs for this event
      - in: formData
        name: displayOrder
        description: The display order for this event
      - in: formData
        name: eventTypeId
        description: The Event Type Id to use for this Event
      - in: formData
        name: fromDt
        description: The from date for this event
      - in: formData
        name: isPriority
        description: An integer indicating the priority of this event
      - in: formData
        name: recurrenceDetail
        description: The interval for the recurrence
      - in: formData
        name: recurrenceRange
        description: The end date for this events recurrence
      - in: formData
        name: recurrenceRepeatsOn
        description: The days of the week that this event repeats - weekly only
      - in: formData
        name: recurrenceType
        description: The type of recurrence to apply to this event
      - in: formData
        name: syncTimezone
        description: Should this schedule be synced to the resulting Display timezone?
      - in: formData
        name: toDt
        description: The to date for this event
      responses:
        200:
          description: OK
      tags:
      - Schedule
      - Event
  /schedule/{eventId}:
    put:
      summary: Edit Schedule Event
      description: Edit a scheduled event for a Campaign/Layout to be shown on a Display
        Group/Display.
      operationId: scheduleEdit
      x-api-path-slug: scheduleeventid-put
      parameters:
      - in: formData
        name: campaignId
        description: The Campaign ID to use for this Event
      - in: formData
        name: commandId
        description: The Command ID to use for this Event
      - in: formData
        name: dayPartId
        description: The Day Part for this event
      - in: formData
        name: displayGroupIds
        description: The Display Group IDs for this event
      - in: formData
        name: displayOrder
        description: The display order for this event
      - in: path
        name: eventId
        description: The Scheduled Event ID
      - in: formData
        name: eventTypeId
        description: The Event Type Id to use for this Event
      - in: formData
        name: fromDt
        description: The from date for this event
      - in: formData
        name: isPriority
        description: An integer indicating the priority of this event
      - in: formData
        name: recurrenceDetail
        description: The interval for the recurrence
      - in: formData
        name: recurrenceRange
        description: The end date for this events recurrence
      - in: formData
        name: recurrenceRepeatsOn
        description: The days of the week that this event repeats - weekly only
      - in: formData
        name: recurrenceType
        description: The type of recurrence to apply to this event
      - in: formData
        name: syncTimezone
        description: Should this schedule be synced to the resulting Display timezone?
      - in: formData
        name: toDt
        description: The to date for this event
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Schedule
      - Event
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