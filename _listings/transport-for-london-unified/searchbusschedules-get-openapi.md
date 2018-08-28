---
swagger: "2.0"
x-collection-name: Transport for London Unified
x-complete: 0
info:
  title: Transport for London Unified Search  Bus Schedules
  description: Searches the bus schedules folder on s3 for a given bus number..
  version: v1
host: api.tfl.gov.uk
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Search/BusSchedules:
    get:
      summary: Search  Bus Schedules
      description: Searches the bus schedules folder on s3 for a given bus number..
      operationId: Search_BusSchedules
      x-api-path-slug: searchbusschedules-get
      parameters:
      - in: query
        name: query
        description: The search query
      responses:
        200:
          description: OK
      tags:
      - Search
      - ""
      - Bus
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