---
swagger: "2.0"
x-collection-name: Twitter
x-complete: 0
info:
  title: Twitter Show Closes Trends
  description: Returns the location that Twitter has trending topic information for
  version: "1.1"
host: api.twitter.com
basePath: /1.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /trends/place.json:
    get:
      summary: Show Place Trends
      description: Returns the top 10 trending topics for a specific WOEID
      operationId: returns-the-top-10-trending-topics-for-a-specific-woeid
      x-api-path-slug: trendsplace-json-get
      parameters:
      - in: query
        name: exclude
        description: Setting this equal to hashtages will remove all hashtages from
          the trends list
      - in: query
        name: id
        description: The yahoo where on earch id
      responses:
        200:
          description: OK
      tags:
      - Social
      - Trends
  /trends/available.json:
    get:
      summary: Show Available Trends
      description: Returns the availability
      operationId: returns-the-availability
      x-api-path-slug: trendsavailable-json-get
      responses:
        200:
          description: OK
      tags:
      - Social
      - Trends
  /trends/closest.json:
    get:
      summary: Show Closes Trends
      description: Returns the location that Twitter has trending topic information
        for
      operationId: returns-the-location-that-twitter-has-trending-topic-information-for
      x-api-path-slug: trendsclosest-json-get
      parameters:
      - in: query
        name: lat
        description: If provided with a long parameter the available trend locations
          wil be stored by distance
      - in: query
        name: long
        description: If provided with a lat parameters the available trend locations
          will be sorted by distance
      responses:
        200:
          description: OK
      tags:
      - Social
      - Trends
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