{
  "info": {
    "name": "Data.gov API Add Datasets Dataset Upload Community",
    "_postman_id": "af467a9b-9bd8-4b84-8542-e41c85715b62",
    "description": "Upload a new community resource",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "datasets",
      "item": [
        {
          "id": "fb634493-80c6-4be0-9d6c-2248ad522ca6",
          "name": "postDatasetsDatasetUploadCommunity",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "datasets/:dataset/upload/community/"
              ],
              "variable": [
                {
                  "id": "dataset",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "file",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Upload a new community resource"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "005c504b-103c-4f00-94b0-bdb37e6b64c4"
            }
          ]
        }
      ]
    }
  ]
}