---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite Global News
  description: provide-stock-and-market-news-operations
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
  /GetHistoricalSecurityHeadlines:
    post:
      summary: Get Historical Security Headlines
      description: Returns all headlines that were published in a specified time frame
        for a given security.
      operationId: GetHistoricalSecurityHeadlines
      x-api-path-slug: gethistoricalsecurityheadlines-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Security
      - Headlines
  /GetTopMarketHeadlinesBySector:
    post:
      summary: Get Top Market Headlines By Sector
      description: Returns the most recent specified number of market headlines associated
        with a specified sector.
      operationId: GetTopMarketHeadlinesBySector
      x-api-path-slug: gettopmarketheadlinesbysector-post
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
      - Sector
  /GetTodaysMarketHeadlinesBySector:
    post:
      summary: Get Todays Market Headlines By Sector
      description: Returns all market headlines that were published today for a specified
        sector.
      operationId: GetTodaysMarketHeadlinesBySector
      x-api-path-slug: gettodaysmarketheadlinesbysector-post
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
      - Sector
  /GetTodaysSecurityHeadlines:
    post:
      summary: Get Todays Security Headlines
      description: Returns all headlines that were published today for a given security.
      operationId: GetTodaysSecurityHeadlines
      x-api-path-slug: gettodayssecurityheadlines-post
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
      - Security
      - Headlines
  /GetRecentTopSecurityHeadlines:
    post:
      summary: Get Recent Top Security Headlines
      description: Returns 14 days specified number of headlines for a given security.
      operationId: GetRecentTopSecurityHeadlines
      x-api-path-slug: getrecenttopsecurityheadlines-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Recent
      - Top
      - Security
      - Headlines
  /GetHistoricalMarketHeadlines:
    post:
      summary: Get Historical Market Headlines
      description: Returns all market headlines that were published in a specified
        time frame.
      operationId: GetHistoricalMarketHeadlines
      x-api-path-slug: gethistoricalmarketheadlines-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Market
      - Headlines
  /GetHistoricalMarketHeadlinesBySector:
    post:
      summary: Get Historical Market Headlines By Sector
      description: Returns all market headlines that were published in a specified
        time frame for a specified sector.
      operationId: GetHistoricalMarketHeadlinesBySector
      x-api-path-slug: gethistoricalmarketheadlinesbysector-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Market
      - Headlines
      - Sector
---