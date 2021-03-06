---
swagger: "2.0"
x-collection-name: MotaWord
x-complete: 0
info:
  title: Mota Word Submit a comment to an activity.
  description: Submit a comment to an activity..
  version: alpha-0.1.0
host: api.motaword.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /projects/{projectId}/activities:
    get:
      summary: Get a list of realtime activities.
      description: Get a list of realtime activities on the project, such as translation
        suggestion and translation approval.
      operationId: getActivities
      x-api-path-slug: projectsprojectidactivities-get
      parameters:
      - in: query
        name: page
      - in: query
        name: per_page
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Activities
  /projects/{projectId}/activities/{activityId}:
    get:
      summary: Get a single realtime activity.
      description: Get a single realtime activity..
      operationId: getActivity
      x-api-path-slug: projectsprojectidactivitiesactivityid-get
      parameters:
      - in: path
        name: activityId
        description: Activity ID
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Activities
      - ActivityId
    post:
      summary: Submit a comment to an activity.
      description: Submit a comment to an activity..
      operationId: submitComment
      x-api-path-slug: projectsprojectidactivitiesactivityid-post
      parameters:
      - in: path
        name: activityId
        description: Activity ID
      - in: formData
        name: comment
        description: Comment text
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Activities
      - ActivityId
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