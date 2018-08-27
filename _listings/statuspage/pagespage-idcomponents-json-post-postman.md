{
  "info": {
    "name": "StatusPage.io Create a component",
    "_postman_id": "c72d1062-f158-4fff-9f0f-600f6103364e",
    "description": "Create a component",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Components",
      "item": [
        {
          "id": "d83500bf-fae1-4258-9401-6ce31b4d9912",
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
              "id": "cb05539e-dd95-43a2-ac56-680ac344c4f1"
            }
          ]
        },
        {
          "id": "d596c584-9de8-4672-a4c3-51806bde2b53",
          "name": "create-a-component",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/components.json?component[description]=component%5Bdescription%5D&component[group_id]=component%5Bgroup_id%5D&component[name]=component%5Bname%5D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a component"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0afb49c8-c5ea-47ac-91b1-8569f62198ac"
            }
          ]
        }
      ]
    }
  ]
}