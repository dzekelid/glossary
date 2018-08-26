---
swagger: "2.0"
x-collection-name: Healthcare.gov
x-complete: 0
info:
  title: HealthCare.gov Get Glossary
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