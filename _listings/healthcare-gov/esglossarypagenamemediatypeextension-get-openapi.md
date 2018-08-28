---
swagger: "2.0"
x-collection-name: Healthcare.gov
x-complete: 0
info:
  title: HealthCare.gov Get Es Glossary Pagename
  version: 1.0.0
  description: Returns pages content.
host: www.healthcare.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/glossary{mediaTypeExtension}:
    get:
      summary: Get Glossary
      description: Returns pages content.
      operationId: getApiGlossaryMediatypeextension
      x-api-path-slug: apiglossarymediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
        description: Omiting the param causes html to be returned
      responses:
        200:
          description: OK
      tags:
      - Glossary
  /es/glossary/{pageName}{mediaTypeExtension}:
    get:
      summary: Get Es Glossary Pagename
      description: Returns pages content.
      operationId: getEsGlossaryPagenameMediatypeextension
      x-api-path-slug: esglossarypagenamemediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
        description: Omiting the param causes html to be returned
      - in: path
        name: pageName
      responses:
        200:
          description: OK
      tags:
      - Es
      - Glossary
      - Pagename
  /glossary/{pageName}{mediaTypeExtension}:
    get:
      summary: Get Glossary Page Name Media Type Extension
      description: Returns pages content.
      operationId: returns-pages-content
      x-api-path-slug: glossarypagenamemediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
        description: Omiting the param causes html to be returned
      - in: path
        name: pageName
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Glossary
      - Page
      - Name
      - Media
      - Type
      - Extension
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---