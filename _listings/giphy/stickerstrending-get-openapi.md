---
swagger: "2.0"
x-collection-name: Giphy
x-complete: 0
info:
  title: Giphy Gif API Trending Stickers
  description: Fetch Stickers currently trending online. Hand curated by the GIPHY
    editorial team. Returns 25 results by default.
  termsOfService: https://developers.giphy.com/
  version: v1
host: api.giphy.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /gifs/trending:
    get:
      summary: Trending GIFs
      description: Fetch GIFs currently trending online. Hand curated by the GIPHY
        editorial team.  The data returned mirrors the GIFs showcased on the GIPHY
        homepage. Returns 25 results by default.
      operationId: trendingGifs
      x-api-path-slug: gifstrending-get
      parameters:
      - in: query
        name: No Name
      responses:
        100:
          description: Invalid API Key - The API key passed was not valid or has expired
        105:
          description: Service currently unavailable - The requested service is temporarily
            unavailable
        106:
          description: Write operation failed - The requested operation failed due
            to a temporary issue
        111:
          description: Format "xxx" not found - The requested response format was
            not found
        112:
          description: Method "xxx" not found - The requested method was not found
        114:
          description: Invalid SOAP envelope - The SOAP envelope send in the request
            could not be parsed
        115:
          description: Invalid XML-RPC Method Call - The XML-RPC request document
            could not be parsed
        116:
          description: Bad URL found - One or more arguments contained a URL that
            has been used for abuse on Flickr
      tags:
      - Gifs
      - Trending
  /stickers/trending:
    get:
      summary: Trending Stickers
      description: Fetch Stickers currently trending online. Hand curated by the GIPHY
        editorial team. Returns 25 results by default.
      operationId: trendingStickers
      x-api-path-slug: stickerstrending-get
      parameters:
      - in: query
        name: No Name
      responses:
        100:
          description: Invalid API Key - The API key passed was not valid or has expired
        105:
          description: Service currently unavailable - The requested service is temporarily
            unavailable
        106:
          description: Write operation failed - The requested operation failed due
            to a temporary issue
        111:
          description: Format "xxx" not found - The requested response format was
            not found
        112:
          description: Method "xxx" not found - The requested method was not found
        114:
          description: Invalid SOAP envelope - The SOAP envelope send in the request
            could not be parsed
        115:
          description: Invalid XML-RPC Method Call - The XML-RPC request document
            could not be parsed
        116:
          description: Bad URL found - One or more arguments contained a URL that
            has been used for abuse on Flickr
      tags:
      - Stickers
      - Trending
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