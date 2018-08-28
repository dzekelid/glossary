swagger: "2.0"
x-collection-name: Healthcare.gov
x-complete: 1
info:
  title: Healthcare
  version: 1.0.0
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
      summary: Get Glossary Pagename
      description: Returns pages content.
      operationId: getGlossaryPagenameMediatypeextension
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
      - Glossary
      - Pagename