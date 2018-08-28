---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Futures Get Last Industry Headlines
  description: Return the last press releases since a certain time for an industry.
  version: 1.0.0
host: www.xignite.com
basePath: xFutures.json/XigniteFutures
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetTopIndustryHeadlines:
    post:
      summary: Get Top Industry Headlines
      description: Return the top press releases for an industry.
      operationId: postGettopindustryheadlines
      x-api-path-slug: gettopindustryheadlines-post
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
      - Industry
      - Headlines
  /GetTodaysIndustryHeadlines:
    post:
      summary: Get Todays Industry Headlines
      description: Return press releases for today for an industry.
      operationId: postGettodaysindustryheadlines
      x-api-path-slug: gettodaysindustryheadlines-post
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
      - Industry
      - Headlines
  /GetLastIndustryHeadlines:
    post:
      summary: Get Last Industry Headlines
      description: Return the last press releases since a certain time for an industry.
      operationId: postGetlastindustryheadlines
      x-api-path-slug: getlastindustryheadlines-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Last
      - Industry
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