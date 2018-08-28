swagger: "2.0"
x-collection-name: Transport for London Unified
x-complete: 1
info:
  title: Transport for London Unified
  description: our-unified-api-brings-together-data-across-all-modes-of-transport-into-a-single-restful-api--this-api-provides-access-to-the-most-highly-requested-realtime-and-status-infomation-across-all-the-modes-of-transport-in-a-single-and-consistent-way--access-to-the-developer-documentation-is-available-at-httpsapi-tfl-gov-uk
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