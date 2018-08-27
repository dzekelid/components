{
  "info": {
    "name": "StatusPage.io Get a list of all components",
    "_postman_id": "09ed5322-4bba-48fb-89b7-fc7299bda609",
    "description": "Get a list of all components",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Components",
      "item": [
        {
          "id": "e26b4043-6323-4e8f-a928-ea5bfb486f28",
          "name": "get-a-list-of-all-components",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/components.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of all components"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bae951fa-68fa-408a-b8c4-5d203d44a383"
            }
          ]
        }
      ]
    }
  ]
}