---
swagger: "2.0"
x-collection-name: Lufthansa
x-complete: 1
info:
  title: LH Public
  version: "1.0"
host: api.lufthansa.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /operations/schedules/{origin}/{destination}/{fromDateTime}:
    get:
      summary: Flight Schedules
      description: Scheduled flights between given airports on a given date.
      operationId: OperationsSchedulesFromDateTimeByOriginAndDestinationGet
      x-api-path-slug: operationsschedulesorigindestinationfromdatetime-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: destination
        description: Destination airport
      - in: query
        name: directFlights
        description: Show only direct flights (false=0, true=1)
      - in: path
        name: fromDateTime
        description: Local departure date and optionally departure time (YYYY-MM-DD
          or YYYY-MM-DDTHH:mm)
      - in: query
        name: limit
        description: Number of records returned per request
      - in: query
        name: offset
        description: Number of records skipped
      - in: path
        name: origin
        description: Departure airport
      responses:
        200:
          description: OK
      tags:
      - Operations
      - Schedules
      - Origin
      - Destination
      - FromDateTime
---