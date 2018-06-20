---
swagger: "2.0"
x-collection-name: Netatmo
x-complete: 0
info:
  title: Netatmo Post Switchschedule
  description: The method switchschedule switches the Thermostat's schedule to another
    existing schedule.
  termsOfService: https://dev.netatmo.com/dev/resources/legal/introduction
  contact:
    name: Netatmo
    email: contact-api@netatmo.com
  version: 1.1.1
host: api.netatmo.net
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /createnewschedule:
    post:
      summary: Post Createnewschedule
      description: The method createnewschedule creates a new schedule stored in the
        backup list.
      operationId: createnewschedule
      x-api-path-slug: createnewschedule-post
      parameters:
      - in: query
        name: device_id
        description: The relay id
      - in: query
        name: module_id
        description: The thermostat id
      - in: body
        name: therm_program
        description: The thermostat program (zones and timetable)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Schedules
  /switchschedule:
    post:
      summary: Post Switchschedule
      description: The method switchschedule switches the Thermostat's schedule to
        another existing schedule.
      operationId: switchschedule
      x-api-path-slug: switchschedule-post
      parameters:
      - in: query
        name: device_id
        description: The relay id
      - in: query
        name: module_id
        description: The thermostat id
      - in: query
        name: schedule_id
        description: The schedule id
      responses:
        200:
          description: OK
      tags:
      - Schedules
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