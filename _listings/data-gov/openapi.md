swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 1
info:
  title: Data.gov API
  description: the-data-gov-catalog-is-powered-by-ckan-a-powerful-open-source-data-platform-that-includes-a-robust-api--please-be-aware-that-data-gov-and-the-data-gov-ckan-api-only-contain-metadata-about-datasets--this-metadata-includes-urls-and-descriptions-of-datasets-but-it-does-not-include-the-actual-data-within-each-dataset-
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
  /datasets/{dataset}/upload/community/:
    post:
      summary: Add Datasets Dataset Upload Community
      description: Upload a new community resource
      operationId: postDatasetsDatasetUploadCommunity
      x-api-path-slug: datasetsdatasetuploadcommunity-post
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      - in: formData
        name: file
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Upload
      - Community
  /me/org_community_resources/:
    get:
      summary: Get Me Org Community Resources
      description: List all community resources related to me and my organizations
      operationId: getMeOrgCommunityResources
      x-api-path-slug: meorg-community-resources-get
      parameters:
      - in: query
        name: q
        description: The string to filter items
      responses:
        200:
          description: OK
      tags:
      - Me
      - Org
      - Community
      - Resources