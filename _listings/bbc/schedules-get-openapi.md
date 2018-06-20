---
swagger: "2.0"
x-collection-name: BBC
x-complete: 0
info:
  title: BBC Nitro Build schedules and find metadata for TV and radio broadcasts and
    webcasts
  description: 'Dates, Times, Schedules: when and where are programmes being shown?'
  termsOfService: http://www.bbc.co.uk/terms/
  contact:
    name: Open Nitro Project
    url: http://developer.bbc.co.uk/
    email: nitro@bbc.co.uk
  version: 1.0.0
host: programmes.api.bbc.com
basePath: /nitro/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /schedules:
    get:
      summary: Build schedules and find metadata for TV and radio broadcasts and webcasts
      description: 'Dates, Times, Schedules: when and where are programmes being shown?'
      operationId: listSchedules
      x-api-path-slug: schedules-get
      parameters:
      - in: query
        name: authority
        description: filter for subset of broadcasts and webcasts that have given
          authority
      - in: query
        name: descendants_of
        description: filter for subset of broadcasts and webcasts that are descendants
          of the given programme PID
      - in: query
        name: end_from
        description: filter for subset of broadcasts and webcasts that end on or later
          than the specified datetime
      - in: query
        name: end_to
        description: filter for subset of broadcasts and webcasts that end on or earlier
          than the specified datetime
      - in: query
        name: format
        description: filter for subset of broadcasts and webcasts that are classified
          in the given format ID
      - in: query
        name: genre
        description: filter for subset of broadcasts and webcasts that are classified
          in the given genre ID
      - in: query
        name: group
        description: filter for subset of broadcasts and webcasts that have programmes
          in the given group
      - in: query
        name: id
        description: filter for subset of broadcasts and webcasts that have given
          identifier
      - in: query
        name: id_type
        description: filter for subset of broadcasts and webcasts that have given
          id type
      - in: query
        name: item
        description: filter for subset of broadcasts and webcasts with the given item
          performed on it
      - in: query
        name: mixin
        description: 'Mixins:* ancestor_titles: return ancestor programme titles*
          images: mixin to add image information for broadcasts and webcasts* titles:
          return ancestor programme titles'
      - in: query
        name: page
        description: which page of results to return
      - in: query
        name: page_size
        description: number of results in each page
      - in: query
        name: partner_id
        description: filter for broadcasts and webcasts by partner ID
      - in: query
        name: partner_pid
        description: filter for broadcasts and webcasts by partner PID
      - in: query
        name: people
        description: filter for subset of broadcasts and webcasts that have given
          contributor
      - in: query
        name: pid
        description: filter for subset of broadcasts and webcasts having given PID
      - in: query
        name: q
        description: filter for subset of broadcasts and webcasts matching supplied
          keyword/phrase (boolean operators permitted)
      - in: query
        name: repeat
        description: filter to show either only repeats or non-repeats
      - in: query
        name: schedule_day
        description: filter for subset of broadcasts and webcasts that start on the
          specified day (BBC time)
      - in: query
        name: schedule_day_from
        description: filter for subset of broadcasts and webcasts that start on or
          after the specified day (BBC time)
      - in: query
        name: schedule_day_to
        description: filter for subset of broadcasts and webcasts that start on or
          before the specified day (BBC time)
      - in: query
        name: service_master_brand
        description: filter for subset of broadcasts and webcasts with given service
          master brand
      - in: query
        name: sid
        description: filter for subset of broadcasts and webcasts that are on the
          specified linear service
      - in: query
        name: sort
        description: 'Sorts:* start_date: sort chronologically by scheduled start
          time/date, ascending'
      - in: query
        name: sort_direction
        description: Sort direction
      - in: query
        name: start_from
        description: filter for subset of broadcasts and webcasts that start on or
          later than the specified datetime
      - in: query
        name: start_to
        description: filter for subset of broadcasts and webcasts that start on or
          earlier than the specified datetime
      - in: query
        name: version
        description: filter for subset of broadcasts and webcasts with given PID as
          their parent version
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