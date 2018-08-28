swagger: "2.0"
x-collection-name: Steem
x-complete: 1
info:
  title: Interactive Steem API
  description: interactive-steem-api-lets-you-interact-with-steem-blockchain-and-make-a-request-get-output-and-start-implementing-new-apps-apis-have-default-parameters-set-to-get-you-started-and-see-how-request-works--api-list-is-compiled-from-steem-githubhttpsgithub-comsteemitsteem-1httpsgithub-comsteemitsteemtreemasterlibrariesappincludesteemitappapi-hpp-and-2httpsgithub-comsteemitsteemtreemasterlibrariesappincludesteemitappdatabase-api-hpp--if-you-want-to-contribute-documenting-detail-of-properties-and-output-contact-goodkarmahttpssteemit-chatdirectgoodkarma--you-can-also-check-full-list-here-steem-jshttpssteemjs-com
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