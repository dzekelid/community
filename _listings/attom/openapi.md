swagger: "2.0"
x-collection-name: ATTOM
x-complete: 1
info:
  title: Attom Data Solutions API
  description: attom-empowers-customers-with-better-property-data--we-warehouse-property-data-nationwide-with-myriad-data-points-on-each-parcel-including-ownership-information-latlong-square-footage-loan-types-sales-history-sales-comps-crime-schools-and-more-
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