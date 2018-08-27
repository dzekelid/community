{
  "info": {
    "name": "Data.gov API Get Datasets Community Resources Community",
    "_postman_id": "6b9b44a2-a509-41b5-9899-0ad167acde01",
    "description": "Retrieve a community resource given its identifier",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "datasets",
      "item": [
        {
          "id": "fa195d0c-1734-439e-9b2f-839cbfe1818e",
          "name": "getDatasetsCommunityResourcesCommunity",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "datasets/community_resources/:community/"
              ],
              "query": [
                {
                  "key": "dataset",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "community",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve a community resource given its identifier"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad0960c0-120e-4011-9b9f-f3c5e808993c"
            }
          ]
        }
      ]
    }
  ]
}