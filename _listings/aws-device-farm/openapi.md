swagger: "2.0"
x-collection-name: AWS Device Farm
x-complete: 1
info:
  title: AWS Device Farm API
  version: 1.0.0
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