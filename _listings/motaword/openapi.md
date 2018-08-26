---
swagger: "2.0"
x-collection-name: MotaWord
x-complete: 1
info:
  title: Mota Word
  description: use-motaword-api-to-post-and-track-your-translation-projects-
  version: alpha-0.1.0
host: api.motaword.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /glossary:
    get:
      summary: Download the global glossary.
      description: Download your corporate account's global glossary. This endpoint
        is available only for corporate account customers.
      operationId: downloadGlobalGlossary
      x-api-path-slug: glossary-get
      responses:
        200:
          description: OK
      tags:
      - Glossary
    post:
      summary: Create or update the global glossary.
      description: Update your corporate account's global glossary. This endpoint
        is available only for corporate account customers.
      operationId: updateGlobalGlossary
      x-api-path-slug: glossary-post
      parameters:
      - in: formData
        name: glossary
        description: Glossary file
      responses:
        200:
          description: OK
      tags:
      - Glossary
  /projects/{projectId}/glossaries:
    get:
      summary: Get a list of glossaries
      description: Get a list of glossaries.
      operationId: getGlossaries
      x-api-path-slug: projectsprojectidglossaries-get
      parameters:
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Glossaries
    post:
      summary: Upload a new glossary
      description: Upload a new glossary.
      operationId: createGlossary
      x-api-path-slug: projectsprojectidglossaries-post
      parameters:
      - in: formData
        name: glossaries
        description: You can only add one glossary, even though the name suggests
          multiple glossaries
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Glossaries
  /projects/{projectId}/glossaries/{glossaryId}:
    delete:
      summary: Delete the glossary
      description: Delete the glossary.
      operationId: deleteGlossary
      x-api-path-slug: projectsprojectidglossariesglossaryid-delete
      parameters:
      - in: path
        name: glossaryId
        description: Glossary ID
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Glossaries
      - GlossaryId
    get:
      summary: Get single glossary
      description: Get single glossary.
      operationId: getGlossary
      x-api-path-slug: projectsprojectidglossariesglossaryid-get
      parameters:
      - in: path
        name: glossaryId
        description: Glossary ID
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Glossaries
      - GlossaryId
    put:
      summary: Update the glossary.
      description: Update the glossary. File name and contents will replaced with
        the new one.
      operationId: updateGlossary
      x-api-path-slug: projectsprojectidglossariesglossaryid-put
      parameters:
      - in: formData
        name: glossaries
        description: Single file data
      - in: path
        name: glossaryId
        description: Glossary ID
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Glossaries
      - GlossaryId
  /projects/{projectId}/glossaries/{glossaryId}/download:
    get:
      summary: Download a glossary
      description: Download a glossary.
      operationId: downloadGlossary
      x-api-path-slug: projectsprojectidglossariesglossaryiddownload-get
      parameters:
      - in: path
        name: glossaryId
        description: Glossary ID
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Glossaries
      - GlossaryId
      - Download
---