{
  "info": {
    "name": "Data.gov API Add Datasets Community Resources Community Upload",
    "_postman_id": "cb6fe40c-51c1-4bf2-af24-92872da9a395",
    "description": "Update the file related to a given community resource",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "datasets",
      "item": [
        {
          "id": "56d616d9-6931-4df5-a034-9f02fc29a373",
          "name": "postDatasetsCommunityResourcesCommunityUpload",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "datasets/community_resources/:community/upload/"
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Update the file related to a given community resource"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aafc3d43-592f-46d6-8954-0c70b11641be"
            }
          ]
        }
      ]
    }
  ]
}