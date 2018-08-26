---
swagger: "2.0"
x-collection-name: ATTOM
x-complete: 0
info:
  title: Attom Data Solutions API Returns community information.
  description: This search returns community information for a specific geography.
  version: 1.0.0
host: search.onboard-apis.com
basePath: /communityapi/v2.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /area/full:
    get:
      summary: Returns community information.
      description: This search returns community information for a specific geography.
      operationId: getCommunityAPIAreaFull
      x-api-path-slug: areafull-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: ApiKey
        description: Application Key
      - in: query
        name: AreaId
        description: This is the Area ID to search
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Community
      - Information
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