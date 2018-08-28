---
swagger: "2.0"
x-collection-name: AWS Device Farm
x-complete: 0
info:
  title: AWS Device Farm API Schedule Run
  version: 1.0.0
  description: Schedules a run.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ScheduleRun:
    get:
      summary: Schedule Run
      description: Schedules a run.
      operationId: scheduleRun
      x-api-path-slug: actionschedulerun-get
      parameters:
      - in: query
        name: appArn
        description: The ARN of the app to schedule a run
        type: string
      - in: query
        name: configuration
        description: Information about the settings for the run to be scheduled
        type: string
      - in: query
        name: devicePoolArn
        description: The ARN of the device pool for the run to be scheduled
        type: string
      - in: query
        name: name
        description: The name for the run to be scheduled
        type: string
      - in: query
        name: projectArn
        description: The ARN of the project for the run to be scheduled
        type: string
      - in: query
        name: test
        description: Information about the test for the run to be scheduled
        type: string
      responses:
        200:
          description: OK
      tags:
      - Runs
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