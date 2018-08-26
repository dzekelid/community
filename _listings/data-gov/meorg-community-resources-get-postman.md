{
  "info": {
    "name": "Data.gov API Get Me Org Community Resources",
    "_postman_id": "7fbeffd2-b58c-4630-b1db-19abc093ad32",
    "description": "List all community resources related to me and my organizations",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "me",
      "item": [
        {
          "id": "cbd413df-7981-434c-b8e5-e381e001bbf8",
          "name": "getMeOrgCommunityResources",
          "request": {
            "url": "http://catalog.data.gov/api/3/me/org_community_resources/?q=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all community resources related to me and my organizations"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5807daec-b8b1-401b-b908-d83c84e66c49"
            }
          ]
        }
      ]
    }
  ]
}