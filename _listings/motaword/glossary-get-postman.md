{
  "info": {
    "name": "Mota Word Download the global glossary.",
    "_postman_id": "df366258-04d5-4a08-895c-a0e6f15d3526",
    "description": "Download your corporate account's global glossary. This endpoint is available only for corporate account customers.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Folder",
      "item": [
        {
          "id": "ece14829-1fb2-4d75-991d-7f7673157086",
          "name": "getEndpoints",
          "request": {
            "url": "http://api.motaword.com/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The root endpoint will provide you a JSON Swagger definition."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "11e74e2e-4929-4270-8595-452d00f5e5dc"
            }
          ]
        }
      ]
    },
    {
      "name": "Formats",
      "item": [
        {
          "id": "a2a389ea-b42b-497b-8c65-47e0ea3a6c60",
          "name": "getFormats",
          "request": {
            "url": "http://api.motaword.com/formats",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of supported formats for documents, style guides and extensions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23579125-38e0-4a63-a1fa-8d2f0abe0898"
            }
          ]
        }
      ]
    },
    {
      "name": "Glossary",
      "item": [
        {
          "id": "5f57aeca-0b95-4fbe-9544-3df89b5118fd",
          "name": "downloadGlobalGlossary",
          "request": {
            "url": "http://api.motaword.com/glossary",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Download your corporate account's global glossary. This endpoint is available only for corporate account customers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "73977149-e36f-4879-88ca-5d2085d167d9"
            }
          ]
        }
      ]
    }
  ]
}