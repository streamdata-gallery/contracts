swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite VWAP
  description: provides-delayed-and-historical-volumeweightedaverage-price-vwap-information-
  version: 1.0.0
host: www.xignite.com
basePath: xVWAP.json/XigniteVWAP
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ListFrontMonthContracts:
    get:
      summary: List Front Month Contracts
      description: List all commodity future Front Month Contracts.
      operationId: postListfrontmonthcontracts
      x-api-path-slug: listfrontmonthcontracts-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Front
      - Month
      - Contracts