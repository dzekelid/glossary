{
  "info": {
    "name": "Big Oven Get food glossary article",
    "_postman_id": "8b7c6b33-4103-459f-8a97-ba9ac6463922",
    "description": "Get food glossary article.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Recipes",
      "item": [
        {
          "id": "8e889675-1c37-406d-be19-47393f3e155f",
          "name": "Collection_GetCollection",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api2.bigoven.com",
              "path": [
                "collection/:id"
              ],
              "query": [
                {
                  "key": "pg",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "rpp",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sessionForLogging",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "test",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a recipe collection. a recipe collection is a curated set of recipes.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58404e2b-bb5b-4392-9789-0590c22dbc63"
            }
          ]
        },
        {
          "id": "fb9e1f2d-20d3-4f84-a620-499774cff26d",
          "name": "Collection_GetCollectionMeta",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api2.bigoven.com",
              "path": [
                "collection/:id/meta"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a recipe collection metadata. a recipe collection is a curated set of recipes.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67916537-6857-4d07-98a4-e90ebb0dc720"
            }
          ]
        },
        {
          "id": "cee4dc86-9e6c-4340-b292-f8e434d5820b",
          "name": "Collection_Collections",
          "request": {
            "url": "http://api2.bigoven.com/collections?test=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the list of current, seasonal recipe collections. from here, you can use the /collection/{id} endpoint to retrieve the recipes in those collections.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7ef3f9e3-1495-4466-a765-276f16e17ca0"
            }
          ]
        },
        {
          "id": "bbaf03dd-1848-4dfe-bdb4-1d47f32a8f13",
          "name": "Glossary_ByTerm",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api2.bigoven.com",
              "path": [
                "glossary/byterm/:term"
              ],
              "variable": [
                {
                  "id": "term",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get food glossary article by term (e.g., asparagus). this editorial is (c) bigoven and must carry attribution and a link back to the glossary entry on bigoven.com.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd1e3264-8b68-49a5-863a-146f7578339a"
            }
          ]
        },
        {
          "id": "84b149a3-bbcd-408c-b48b-45eb27d49bde",
          "name": "Glossary_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api2.bigoven.com",
              "path": [
                "glossary/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get food glossary article."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1b8cf51f-8743-4ec8-87d3-db6c8380a6d8"
            }
          ]
        }
      ]
    }
  ]
}