---
name: Strava
x-slug: strava
description: Strava is software as a service used to track cycling, running, and swimming
  activity via GPS.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28739-strava.jpg
x-kinRank: "7"
x-alexaRank: "887"
tags: Activities
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/activities/master/_listings/strava/apis.md
specificationVersion: "0.14"
apis:
- name: Strava API v3 - List Athlete Activities
  x-api-slug: athleteactivities-get
  description: Returns the activities of an athlete for a specific identifier.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28739-strava.jpg
  humanURL: ""
  baseURL: https://www.strava.com//api/v3
  tags: Mobile, Technology, internet, Sports, Athletes, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/activities/master/_listings/strava/athleteactivities-get-openapi.md
- name: Strava API v3 - List Club Activities
  x-api-slug: clubsidactivities-get
  description: Retrieve recent activities from members of a specific club. The authenticated
    athlete must belong to the requested club in order to hit this endpoint. Pagination
    is supported. Enhanced Privacy Mode is respected for all activities.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28739-strava.jpg
  humanURL: ""
  baseURL: https://www.strava.com//api/v3
  tags: Mobile, Technology, internet, Sports, Athletes, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/activities/master/_listings/strava/clubsidactivities-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://storecove.api.gallery.streamdata.io
- type: x-api-stack
  url: http://strava.stack.network
- type: x-code
  url: https://developers.strava.com/docs/#client-code
- type: x-crunchbase
  url: https://crunchbase.com/organization/strava
- type: x-documentation
  url: https://developers.strava.com/docs/reference/
- type: x-email
  url: developers@strava.com
- type: x-email
  url: dpo@strava.com
- type: x-email
  url: ip@strava.com
- type: x-github
  url: https://github.com/strava
- type: x-openapi
  url: https://developers.strava.com/swagger/swagger.json
- type: x-twitter
  url: https://twitter.com/Strava
- type: x-developer
  url: https://developers.strava.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---