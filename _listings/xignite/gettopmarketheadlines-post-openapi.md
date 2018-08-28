---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Global News Get Top Market Headlines
  description: Returns the most recent specified number of market headlines.
  version: 1.0.0
host: globalnews.xignite.com
basePath: xGlobalNews.json/XigniteGlobalNews
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetTodaysMarketHeadlines:
    post:
      summary: Get Todays Market Headlines
      description: Returns all market headlines that were published today.
      operationId: GetTodaysMarketHeadlines
      x-api-path-slug: gettodaysmarketheadlines-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Todays
      - Market
      - Headlines
  /GetTopSecurityHeadlines:
    post:
      summary: Get Top Security Headlines
      description: Returns the most recent specified number of headlines for a given
        security.
      operationId: GetTopSecurityHeadlines
      x-api-path-slug: gettopsecurityheadlines-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Top
      - Security
      - Headlines
  /GetTopMarketHeadlines:
    post:
      summary: Get Top Market Headlines
      description: Returns the most recent specified number of market headlines.
      operationId: GetTopMarketHeadlines
      x-api-path-slug: gettopmarketheadlines-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Top
      - Market
      - Headlines
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