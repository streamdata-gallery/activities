---
swagger: "2.0"
x-collection-name: YouTube
x-complete: 0
info:
  title: Youtube Add Activities
  description: |-
    Posts a bulletin for a specific channel. (The user submitting the request must be authorized to act on the channel's behalf.)

    Note: Even though an activity resource can contain information about actions like a user rating a video or marking a video as a favorite, you need to use other API methods to generate those activity resources. For example, you would use the API's videos.rate() method to rate a video and the playlistItems.insert() method to mark a video as a favorite.
  termsOfService: https://developers.google.com/terms/
  contact:
    name: Google
    url: https://google.com
  version: 1.0.0
host: www.googleapis.com
basePath: /youtube/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /activities:
    get:
      summary: Get Activities
      description: Returns a list of channel activity events that match the request
        criteria. For example, you can retrieve events associated with a particular
        channel, events associated with the user's subscriptions and Google+ friends,
        or the YouTube home page feed, which is customized for each user.
      operationId: getActivities
      x-api-path-slug: activities-get
      parameters:
      - in: query
        name: channelId
        description: The channelId parameter specifies a unique YouTube channel ID
      - in: query
        name: home
        description: Set this parameters value to true to retrieve the activity feed
          that displays on the YouTube home page for the currently authenticated user
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: mine
        description: Set this parameters value to true to retrieve a feed of the authenticated
          users activities
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more activity resource properties that the API response will include
      - in: query
        name: publishedAfter
        description: The publishedAfter parameter specifies the earliest date and
          time that an activity could have occurred for that activity to be included
          in the API response
      - in: query
        name: publishedBefore
        description: The publishedBefore parameter specifies the date and time before
          which an activity must have occurred for that activity to be included in
          the API response
      - in: query
        name: regionCode
        description: The regionCode parameter instructs the API to return results
          for the specified country
      responses:
        200:
          description: OK
      tags:
      - Activities
    post:
      summary: Add Activities
      description: |-
        Posts a bulletin for a specific channel. (The user submitting the request must be authorized to act on the channel's behalf.)

        Note: Even though an activity resource can contain information about actions like a user rating a video or marking a video as a favorite, you need to use other API methods to generate those activity resources. For example, you would use the API's videos.rate() method to rate a video and the playlistItems.insert() method to mark a video as a favorite.
      operationId: postActivities
      x-api-path-slug: activities-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: part
        description: The part parameter serves two purposes in this operation
      responses:
        200:
          description: OK
      tags:
      - Activities
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