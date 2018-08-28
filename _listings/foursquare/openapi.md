swagger: "2.0"
x-collection-name: Foursquare
x-complete: 1
info:
  title: Foursquare
  version: 1.0.0
host: api.foursquare.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /venues/trending:
    get:
      summary: Get Venues Trending
      description: /venues/timeseries
      operationId: venuestimeseries
      x-api-path-slug: venuestrending-get
      parameters:
      - in: query
        name: limit
        description: Number of results to return, up to 50
      - in: query
        name: ll
        description: Latitude and longitude of the users location
      - in: query
        name: radius
        description: Radius in meters, up to approximately 2000 meters
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Venues
      - Trending