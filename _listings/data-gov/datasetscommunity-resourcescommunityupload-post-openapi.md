---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Add Datasets Community Resources Community Upload
  description: Update the file related to a given community resource
  version: "3"
host: catalog.data.gov
basePath: /api/3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /datasets/community_resources/:
    get:
      summary: Get Datasets Community Resources
      description: List all community resources
      operationId: getDatasetsCommunityResources
      x-api-path-slug: datasetscommunity-resources-get
      parameters:
      - in: query
        name: dataset
        description: Filter activities for that particular dataset
      - in: query
        name: organization
        description: Filter activities for that particular organization
      - in: query
        name: owner
        description: Filter activities for that particular user
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      - in: query
        name: sort
        description: The sorting attribute
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Community
      - Resources
    post:
      summary: Add Datasets Community Resources
      description: Create a new community resource
      operationId: postDatasetsCommunityResources
      x-api-path-slug: datasetscommunity-resources-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Community
      - Resources
  /datasets/community_resources/{community}/:
    delete:
      summary: Delete Datasets Community Resources Community
      description: Delete a given community resource
      operationId: deleteDatasetsCommunityResourcesCommunity
      x-api-path-slug: datasetscommunity-resourcescommunity-delete
      parameters:
      - in: path
        name: community
        description: The community resource unique identifier
      - in: query
        name: dataset
        description: The dataset ID or slug
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Community
      - Resources
      - Community
    get:
      summary: Get Datasets Community Resources Community
      description: Retrieve a community resource given its identifier
      operationId: getDatasetsCommunityResourcesCommunity
      x-api-path-slug: datasetscommunity-resourcescommunity-get
      parameters:
      - in: path
        name: community
        description: The community resource unique identifier
      - in: query
        name: dataset
        description: The dataset ID or slug
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Community
      - Resources
      - Community
    put:
      summary: Put Datasets Community Resources Community
      description: Update a given community resource
      operationId: putDatasetsCommunityResourcesCommunity
      x-api-path-slug: datasetscommunity-resourcescommunity-put
      parameters:
      - in: path
        name: community
        description: The community resource unique identifier
      - in: query
        name: dataset
        description: The dataset ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Community
      - Resources
      - Community
  /datasets/community_resources/{community}/upload/:
    post:
      summary: Add Datasets Community Resources Community Upload
      description: Update the file related to a given community resource
      operationId: postDatasetsCommunityResourcesCommunityUpload
      x-api-path-slug: datasetscommunity-resourcescommunityupload-post
      parameters:
      - in: path
        name: community
        description: The community resource unique identifier
      - in: query
        name: dataset
        description: The dataset ID or slug
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Community
      - Resources
      - Community
      - Upload
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