{
  "info": {
    "name": "StatusPage.io Delete a component",
    "_postman_id": "61b0105c-d691-4d59-88a3-9a1c066e99f7",
    "description": "Delete a component",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Components",
      "item": [
        {
          "id": "2cd5f6b3-aab9-43d8-9693-c0a38aa62571",
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
              "id": "263c26de-dd91-477f-afa2-10094b90500f"
            }
          ]
        },
        {
          "id": "4d9bb35e-cdc2-4ba7-bbf6-a8d2eeb138c1",
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
              "id": "925d2b4d-dc36-44ec-b9d7-83148abe39d6"
            }
          ]
        },
        {
          "id": "5e47e163-c14a-42ea-b1c4-d2893d5c3881",
          "name": "delete-a-component",
          "request": {
            "url": "http://example.com/api/pages/[page_id]/components/[component_id].json",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a component"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8facb5ee-e854-4ba0-af3d-28a8c33cfa59"
            }
          ]
        }
      ]
    }
  ]
}