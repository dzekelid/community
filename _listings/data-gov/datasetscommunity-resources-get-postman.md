{
  "info": {
    "name": "Data.gov API Get Datasets Community Resources",
    "_postman_id": "50c8f211-6c06-4297-9198-14fdb4402046",
    "description": "List all community resources",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "datasets",
      "item": [
        {
          "id": "d2d548f9-d8e0-4d32-be56-c76cea64e637",
          "name": "getDatasetsCommunityResources",
          "request": {
            "url": "http://catalog.data.gov/api/3/datasets/community_resources/?dataset=%7B%7D&organization=%7B%7D&owner=%7B%7D&page=%7B%7D&page_size=%7B%7D&sort=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all community resources"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "082a8442-3020-461c-9b0a-985c39e95ce4"
            }
          ]
        }
      ]
    }
  ]
}