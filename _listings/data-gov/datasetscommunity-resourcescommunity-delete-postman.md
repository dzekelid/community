{
  "info": {
    "name": "Data.gov API Delete Datasets Community Resources Community",
    "_postman_id": "754e713e-cbd9-45a1-b2d5-c0e203177429",
    "description": "Delete a given community resource",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "datasets",
      "item": [
        {
          "id": "34395b45-dc87-4705-a9a2-46d4da300ddd",
          "name": "deleteDatasetsCommunityResourcesCommunity",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a given community resource"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0c0c7d9-987c-4169-97e2-d128c3c3d6c2"
            }
          ]
        }
      ]
    }
  ]
}