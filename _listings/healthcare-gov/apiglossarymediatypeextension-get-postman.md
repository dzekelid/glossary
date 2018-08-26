{
  "info": {
    "name": "HealthCare.gov Get Glossary",
    "_postman_id": "9de3ba1c-e40c-4126-b572-16e13f434d3f",
    "description": "Returns pages content.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Articles",
      "item": [
        {
          "id": "7fd78507-eb12-4796-b2e2-9253128f79d8",
          "name": "getApiArticlesMediatypeextension",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.healthcare.gov",
              "path": [
                "api/articles:mediaTypeExtension"
              ],
              "variable": [
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns pages content."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f85120ec-bdc0-44b1-976f-b923007a3bad"
            }
          ]
        }
      ]
    },
    {
      "name": "Blog",
      "item": [
        {
          "id": "54adb69f-5217-407e-8d7f-7ffa08ea704c",
          "name": "getApiBlogMediatypeextension",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.healthcare.gov",
              "path": [
                "api/blog:mediaTypeExtension"
              ],
              "variable": [
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns pages content."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a3d6fa9-7d03-4e23-b4db-7438dd622c35"
            }
          ]
        }
      ]
    },
    {
      "name": "Glossary",
      "item": [
        {
          "id": "0de09e95-4b28-42cd-bd6f-fdea386175ff",
          "name": "getApiGlossaryMediatypeextension",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.healthcare.gov",
              "path": [
                "api/glossary:mediaTypeExtension"
              ],
              "variable": [
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns pages content."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "198bca9e-fb66-4289-9535-e98460d37357"
            }
          ]
        }
      ]
    }
  ]
}