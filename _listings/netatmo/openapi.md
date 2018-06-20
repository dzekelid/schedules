---
swagger: "2.0"
x-collection-name: Netatmo
x-complete: 1
info:
  title: Netatmo
  description: we-develop-groundbreaking-intuitive-and-beautifullydesigned-connected-consumer-electronics--truly-smart-our-innovative-products-provide-a-seamless-experience-that-helps-users-create-a-safer-healthier-and-more-comfortable-home---we-carefully-design-the-mechanics-electronics-and-embedded-software-of-all-our-products-to-the-highest-standards--our-mobile-and-web-applications-are-designed-to-be-simple-to-operate-yet-deliver-a-rich-user-experience-
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
  /syncschedule:
    post:
      summary: Post Syncschedule
      description: The method syncschedule changes the Thermostat weekly schedule.
      operationId: syncschedule
      x-api-path-slug: syncschedule-post
      parameters:
      - in: query
        name: device_id
        description: The relay id
      - in: query
        name: module_id
        description: The thermostat id
      - in: body
        name: therm_program
        description: The thermostat program (zones, timetable and name)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Schedules
---