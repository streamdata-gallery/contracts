---
swagger: "2.0"
info:
  title: Akamai API List Usage per Contract
  description: List Usage per Contract
  version: 1.0.0
host: developer.akamai.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /billing-center-api/v2/contracts/{contractId}/products/{productId}/measures:
    get:
      summary: List Usage per Contract
      description: List Usage per Contract
      operationId: billingcenterapiv2contractscontractidproductsproductidmeasuresyearmonthfromyearfrommonthtoyeartomont
      parameters:
      - in: query
        name: billingDayOnly
        description: Aggregates cumulative data as of the end of the billing period,
          typically the end of the month, otherwise the day the contract&#8217;s term
          expires
        type: string
      - in: query
        name: contractId
        description: Identifies the contract under which data is aggregated
        type: string
      - in: query
        name: fromMonth
        description: The month starting the range of aggregated data
        type: string
      - in: query
        name: fromYear
        description: The year starting the range of aggregated data
        type: string
      - in: query
        name: month
        description: The month for which data is aggregated
        type: string
      - in: query
        name: productId
        description: Identifies the product under which data is aggregated
        type: string
      - in: query
        name: statisticName
        description: Reports on a specific statistic, otherwise reports all statistics
          by default
        type: string
      - in: query
        name: toMonth
        description: The month ending the range of aggregated data
        type: string
      - in: query
        name: toYear
        description: The year ending the range of aggregated data
        type: string
      - in: query
        name: year
        description: The year for which data is aggregated
        type: string
      responses:
        200:
          description: OK
      tags:
      - billing
      - center
      - contracts
      - contract
      - products
      - product
      - measures
      - year
      - month
      - fromyear
      - frommonth
      - toyear
      - tomonth
      - statisticname
      - billingdayonly
definitions: []
x-collection-name: Akamai
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