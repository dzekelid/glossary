---
swagger: "2.0"
x-collection-name: BigOven
x-complete: 0
info:
  title: Big Oven Get food glossary article by term (e.g., asparagus). This editorial
    is (c) BigOven and MUST carry attribution and a link back to the glossary entry
    on BigOven.com.
  description: Get food glossary article by term (e.g., asparagus). this editorial
    is (c) bigoven and must carry attribution and a link back to the glossary entry
    on bigoven.com..
  termsOfService: Please see our [terms of service](http://api2.bigoven.com/web/documentation/termsofuse
  version: partner
host: api2.bigoven.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /glossary/byterm/{term}:
    get:
      summary: Get food glossary article by term (e.g., asparagus). This editorial
        is (c) BigOven and MUST carry attribution and a link back to the glossary
        entry on BigOven.com.
      description: Get food glossary article by term (e.g., asparagus). this editorial
        is (c) bigoven and must carry attribution and a link back to the glossary
        entry on bigoven.com..
      operationId: Glossary_ByTerm
      x-api-path-slug: glossarybytermterm-get
      parameters:
      - in: path
        name: term
        description: Keyword used to look up article, e
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Glossary
      - Byterm
      - Term
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