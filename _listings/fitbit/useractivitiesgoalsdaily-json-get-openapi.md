---
swagger: "2.0"
x-collection-name: Fitbit
x-complete: 0
info:
  title: Fitbit Get User Activities Goals Daily.json
  description: Get a user's current daily activity goals in the format requested using
    units in the unit system which corresponds to the Accept-Language header provided.
  version: 1.0.0
host: api.fitbit.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /activities/{id}.json:
    get:
      summary: Get Activities .json
      description: Get the details of a specific activity in Fitbit activities database
        in the format requested. If activity has levels, also get list of activity
        level details.
      operationId: getActivities.json
      x-api-path-slug: activitiesid-json-get
      responses:
        200:
          description: OK
      tags:
      - Activities
      - Id.json
  /user/-/activities/goals/weekly.json:
    get:
      summary: Get User Activities Goals Weekly.json
      description: Get a user's current weekly activity goals in the format requested
        using units in the unit system which corresponds to the Accept-Language header
        provided.
      operationId: getUserActivitiesGoalsWeekly.json
      x-api-path-slug: useractivitiesgoalsweekly-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Activities
      - Goals
      - Weekly.json
  /user/-/activities/goals/daily.json:
    get:
      summary: Get User Activities Goals Daily.json
      description: Get a user's current daily activity goals in the format requested
        using units in the unit system which corresponds to the Accept-Language header
        provided.
      operationId: getUserActivitiesGoalsDaily.json
      x-api-path-slug: useractivitiesgoalsdaily-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Activities
      - Goals
      - Daily.json
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