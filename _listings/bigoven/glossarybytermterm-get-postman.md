{
  "info": {
    "name": "Big Oven Get food glossary article by term (e.g., asparagus). This editorial is (c) BigOven and MUST carry attribution and a link back to the glossary entry on BigOven.com.",
    "_postman_id": "4b2af0b2-4fc3-4a66-aae4-ea83e3fbbf32",
    "description": "Get food glossary article by term (e.g., asparagus). this editorial is (c) bigoven and must carry attribution and a link back to the glossary entry on bigoven.com..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Recipes",
      "item": [
        {
          "id": "2950977e-8c25-417e-ba56-2795f013d25f",
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
              "id": "d354297e-6c79-42d4-8f5c-758ae12249c1"
            }
          ]
        },
        {
          "id": "32f19971-6659-4de9-a3d6-346a80af891e",
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
              "id": "c0563839-3132-40cb-9f76-f5d6072b7bc8"
            }
          ]
        },
        {
          "id": "0c218c82-65a4-4084-a5c4-6e6b1d3accfa",
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
              "id": "9e5b291f-6f3d-4c7d-801b-073803734218"
            }
          ]
        },
        {
          "id": "29c25d13-1a59-4845-a3ea-4ee8f102d9fe",
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
              "id": "31f91f22-56a9-46d1-94b3-9840f2ebb526"
            }
          ]
        }
      ]
    }
  ]
}