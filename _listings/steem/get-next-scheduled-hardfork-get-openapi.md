---
swagger: "2.0"
x-collection-name: Steem
x-complete: 0
info:
  title: Steem get_next_scheduled_hardfork
  description: get_next_scheduled_hardfork
  version: 1.0.0
host: api.steemjs.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /get_witness_schedule:
    get:
      summary: get_witness_schedule
      description: get_witness_schedule
      operationId: get-witness-schedule
      x-api-path-slug: get-witness-schedule-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Witness
      - Schedule
  /get_next_scheduled_hardfork:
    get:
      summary: get_next_scheduled_hardfork
      description: get_next_scheduled_hardfork
      operationId: get-next-scheduled-hardfork
      x-api-path-slug: get-next-scheduled-hardfork-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Next
      - Scheduled
      - Hardfork
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