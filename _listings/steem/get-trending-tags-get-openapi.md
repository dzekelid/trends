---
swagger: "2.0"
x-collection-name: Steem
x-complete: 0
info:
  title: Steem get trending categories
  description: get tags
  version: 1.0.0
host: api.steemjs.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /get_trending_categories:
    get:
      summary: get trending categories
      description: get tags
      operationId: get-tags
      x-api-path-slug: get-trending-categories-get
      parameters:
      - in: query
        name: after
        description: after
      - in: query
        name: limit
        description: limits
      responses:
        200:
          description: OK
      tags:
      - Get
      - Trending
      - Categories
  /get_trending_tags:
    get:
      summary: get trending categories
      description: get tags
      operationId: get-tags
      x-api-path-slug: get-trending-tags-get
      parameters:
      - in: query
        name: afterTag
        description: category
      - in: query
        name: limit
        description: limits
      responses:
        200:
          description: OK
      tags:
      - Get
      - Trending
      - Categories
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