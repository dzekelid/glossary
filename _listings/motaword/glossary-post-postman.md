{
  "info": {
    "name": "Mota Word Create or update the global glossary.",
    "_postman_id": "770d7cbb-bfd6-436d-b25a-9c3d441c7d57",
    "description": "Update your corporate account's global glossary. This endpoint is available only for corporate account customers.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Folder",
      "item": [
        {
          "id": "eeb78170-a92b-4426-9240-37c083694bb1",
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
              "id": "a71896e5-f610-4f4e-bcca-ceeffb72acd5"
            }
          ]
        }
      ]
    },
    {
      "name": "Formats",
      "item": [
        {
          "id": "396b5d39-1eb4-4947-9b07-b39a1d047e04",
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
              "id": "13f0c69e-344f-442e-9ab8-f276b0073c62"
            }
          ]
        }
      ]
    },
    {
      "name": "Glossary",
      "item": [
        {
          "id": "2e88af93-46da-4054-904c-e82413eb6f84",
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
              "id": "a5b5f205-1ed7-44dc-b90d-6c943447b937"
            }
          ]
        },
        {
          "id": "7e9a99c9-408b-4c52-bc53-d505a41fe7d0",
          "name": "updateGlobalGlossary",
          "request": {
            "url": "http://api.motaword.com/glossary",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "glossary",
                  "value": "{}",
                  "disabled": false,
                  "description": "Glossary file"
                }
              ]
            },
            "description": "Update your corporate account's global glossary. This endpoint is available only for corporate account customers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "650a29a6-8fee-4ae3-b5ce-5291468736c5"
            }
          ]
        }
      ]
    }
  ]
}