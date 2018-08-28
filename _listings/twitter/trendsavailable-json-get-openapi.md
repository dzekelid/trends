---
swagger: "2.0"
x-collection-name: Twitter
x-complete: 0
info:
  title: Twitter Show Available Trends
  description: Returns the availability
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
x-streamrank:
  polling_total_time_average: "0.15"
  polling_size_download_average: "87374.32"
  streaming_total_time_average: "0.08"
  streaming_size_download_average: "43945.5"
  change_yes: "4"
  change_no: "167"
  time_percentage: "45"
  size_percentage: "50"
  change_percentage: "2"
  last_run: "2018-05-06"
  days_run: "1"
  minute_run: "0"
---