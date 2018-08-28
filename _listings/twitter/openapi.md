swagger: "2.0"
x-collection-name: Twitter
x-complete: 1
info:
  title: Twitter
  description: the-twitter-api-gives-you-programmatic-control-over-any-twitter-account-and-most-aspect-of-the-platform--allowing-developers-to-build-social-applications-that-use-the-platform-and-automate-interactions-between-users-
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