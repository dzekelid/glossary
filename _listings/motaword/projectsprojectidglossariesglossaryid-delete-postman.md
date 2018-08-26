{
  "info": {
    "name": "Mota Word Delete the glossary",
    "_postman_id": "0b948167-03ca-427c-87d1-a53125eb199a",
    "description": "Delete the glossary.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Projects",
      "item": [
        {
          "id": "ad977539-978d-4a61-8f73-9cce6a26da96",
          "name": "getProjects",
          "request": {
            "url": "http://api.motaword.com/projects?page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of your projects."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c34b4c2-bc61-449d-a853-24a02205f4d7"
            }
          ]
        },
        {
          "id": "c6670cec-245a-4bbc-be2b-8d89db78b4c9",
          "name": "createProject",
          "request": {
            "url": "http://api.motaword.com/projects",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "callback_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "Optional"
                },
                {
                  "key": "custom",
                  "value": "{}",
                  "disabled": false,
                  "description": "Optional"
                },
                {
                  "key": "documents",
                  "value": "[{}]",
                  "disabled": false,
                  "description": "Optional"
                },
                {
                  "key": "glossaries",
                  "value": "[{}]",
                  "disabled": false,
                  "description": "Optional"
                },
                {
                  "key": "source_language",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "styleguides",
                  "value": "[{}]",
                  "disabled": false,
                  "description": "Optional"
                },
                {
                  "key": "target_languages",
                  "value": "[{}]",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Create a new project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9b922c0-e5e0-48ce-80f6-2157702d34a3"
            }
          ]
        },
        {
          "id": "11683984-be5b-493a-b249-b2929549444f",
          "name": "getProject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id"
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
            "description": "Get single project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "13e2873f-dd02-4a24-b7c6-b23996c8208b"
            }
          ]
        },
        {
          "id": "d43c25ad-2ffe-4304-94e0-9ce2ea20482d",
          "name": "updateProject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "callback_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "Optional"
                },
                {
                  "key": "custom",
                  "value": "{}",
                  "disabled": false,
                  "description": "Optional"
                },
                {
                  "key": "source_language",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "target_languages",
                  "value": "[{}]",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Update project language pairs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f93422e-ad50-4326-9adf-b3a3103d028b"
            }
          ]
        },
        {
          "id": "c4f4a028-4479-4d22-8086-66b386f12246",
          "name": "deleteProject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete(cancel) a project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f73ae617-e065-4ceb-93a3-1b4ff2632173"
            }
          ]
        },
        {
          "id": "6ce3842b-4610-4eef-9eed-9d647a7d19f0",
          "name": "triggerCallback",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id/callback/:actionType"
              ],
              "variable": [
                {
                  "id": "actionType",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Trigger a call to your callback url related to this project.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b67bf8d-0761-4f8d-9b08-2073e6223b55"
            }
          ]
        },
        {
          "id": "0a51d46a-418e-492b-802e-a29af1722e64",
          "name": "cancelProject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id/cancel"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "reason",
                  "value": "{}",
                  "disabled": false,
                  "description": "Cancellation reason"
                }
              ]
            },
            "description": "Cancel your translation project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1fede5e6-6b3b-479d-85dd-8a6320ebce12"
            }
          ]
        },
        {
          "id": "53aac3bd-16ef-4cbb-aa5d-21ac786fff53",
          "name": "download",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id/download"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Download the latest translation package. You must have given a /package call beforehand and wait until the packaging status is 'completed'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31485546-6c1e-4617-bb9f-154b1ac74ee7"
            }
          ]
        },
        {
          "id": "8f585e4d-7025-4023-b66e-22a6049aca80",
          "name": "downloadLanguage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id/download/:language"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "language",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Download only the translation package of this language. You must have given a /package call beforehand and wait until the packaging status is 'completed'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38e4a32c-6984-4fd0-85c9-607b936278b2"
            }
          ]
        },
        {
          "id": "5fedf668-71ba-45ed-98d1-ee22c173fa3f",
          "name": "launchProject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id/launch"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "budget_code",
                  "value": "{}",
                  "disabled": false,
                  "description": "Optional with corporate accounts"
                },
                {
                  "key": "payment_code",
                  "value": "{}",
                  "disabled": false,
                  "description": "Optional"
                },
                {
                  "key": "payment_method",
                  "value": "{}",
                  "disabled": false,
                  "description": "Optional"
                }
              ]
            },
            "description": "Launch your translation project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f4eb5e44-4a60-47a8-8b2c-d65c16c85140"
            }
          ]
        },
        {
          "id": "cf7ce8cd-9193-4b95-8f5f-a9cb66d3f05b",
          "name": "package",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id/package"
              ],
              "query": [
                {
                  "key": "async",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Package the translation project, make it ready to be downloaded."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34144110-89b0-4cbe-b541-4cdd66f3837e"
            }
          ]
        },
        {
          "id": "545439d7-bdcd-4105-94cc-4fea3050f6a1",
          "name": "trackPackage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id/package/check"
              ],
              "query": [
                {
                  "key": "key",
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
            "description": "This request will tell you the current progress of the translation packaging. You will use the 'key' provided by the /package call."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3dc0897e-166c-4ac8-ab98-149df82cdf34"
            }
          ]
        },
        {
          "id": "3265ef62-9d86-42d4-a68e-787d6ca9dd0c",
          "name": "packageLanguage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id/package/:language"
              ],
              "query": [
                {
                  "key": "async",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "language",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Package the translation of a specific target language to be downloaded.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ed2ec1e-9647-41ce-b1ea-f0fde0e1eabd"
            }
          ]
        },
        {
          "id": "b4da4eaf-e2ce-4aea-96f0-06f3dd6edac4",
          "name": "getProgress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id/progress"
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
            "description": "Get the progress of an already launched project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23be69fa-a079-46ab-ac4f-98378d3ff831"
            }
          ]
        },
        {
          "id": "1c97c469-a437-4c23-931f-6be51ab59efd",
          "name": "submitProjectReports",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id/reports"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "activity_type",
                  "value": "{}",
                  "disabled": false,
                  "description": "Activity Type"
                },
                {
                  "key": "message",
                  "value": "{}",
                  "disabled": false,
                  "description": "Report Message"
                }
              ]
            },
            "description": "Submit reports for a project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "41e21c6b-9aef-4590-9a6f-a120e60a9182"
            }
          ]
        },
        {
          "id": "f92261db-2486-4359-a793-ca636838aa86",
          "name": "getActivities",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/activities"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "per_page",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of realtime activities on the project, such as translation suggestion and translation approval."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0365df3e-b126-4717-bab4-be517fa82a9f"
            }
          ]
        },
        {
          "id": "62f81e6e-5655-4c43-b32b-641f402b9c9c",
          "name": "getActivity",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/activities/:activityId"
              ],
              "variable": [
                {
                  "id": "activityId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a single realtime activity.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "17962ffd-fa56-48f3-87d2-35a6a9874d4e"
            }
          ]
        },
        {
          "id": "f49b8699-9344-4136-a9f2-f23affc49c23",
          "name": "submitComment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/activities/:activityId"
              ],
              "variable": [
                {
                  "id": "activityId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "comment",
                  "value": "{}",
                  "disabled": false,
                  "description": "Comment text"
                }
              ]
            },
            "description": "Submit a comment to an activity.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b78fde5f-b8e0-4d03-8e91-649411b6b965"
            }
          ]
        },
        {
          "id": "d316e3f8-a11b-4ee8-826d-8a244c728766",
          "name": "getActivityComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/activities/:activityId/comments"
              ],
              "variable": [
                {
                  "id": "activityId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of comments belonging to this activity.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a274f958-9435-4ae0-b772-8743ab58ee55"
            }
          ]
        },
        {
          "id": "9121770e-da1a-4d1e-8115-150b8d6ee02c",
          "name": "getComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/comments"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "per_page",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of activity comments throughout the whole project.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "678a18d7-657a-411f-ae5b-21478b7b583e"
            }
          ]
        },
        {
          "id": "a3d677ae-7886-46b5-8812-e73b39c74b45",
          "name": "getDocuments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/documents"
              ],
              "variable": [
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of documents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c1eb2cb-4da5-4250-bca5-394bbd647bf4"
            }
          ]
        },
        {
          "id": "e536319c-8047-4f43-917a-4701fa39b436",
          "name": "createDocument",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/documents"
              ],
              "variable": [
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "documents",
                  "value": "[{}]",
                  "disabled": false,
                  "description": "You can add as many files as you want in documents[] parameter"
                },
                {
                  "key": "schemes",
                  "value": "[{}]",
                  "disabled": false,
                  "description": "JSON string"
                }
              ]
            },
            "description": "Upload a new document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bea4d0c6-f1ac-45a0-9aac-e9c96552be32"
            }
          ]
        },
        {
          "id": "29f05ddf-b78b-4e40-9ac5-0793026f2197",
          "name": "getDocument",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/documents/:documentId"
              ],
              "variable": [
                {
                  "id": "documentId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get single document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca31baa6-c49e-4860-9615-dcea4bcf3edc"
            }
          ]
        },
        {
          "id": "f3db1c19-bc78-4a46-a870-cd3de48753a0",
          "name": "updateDocument",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/documents/:documentId"
              ],
              "variable": [
                {
                  "id": "documentId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "documents",
                  "value": "{}",
                  "disabled": false,
                  "description": "Single file data"
                },
                {
                  "key": "schemes",
                  "value": "{}",
                  "disabled": false,
                  "description": "JSON string"
                }
              ]
            },
            "description": "Update the document. File name and contents will replaced with the new one."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36821a2c-2802-4234-8ebb-a908ef01a3c5"
            }
          ]
        },
        {
          "id": "088e41f2-5bc8-41b2-a565-d0ede50f2409",
          "name": "deleteDocument",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/documents/:documentId"
              ],
              "variable": [
                {
                  "id": "documentId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete the document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a6033bd2-ae82-43a2-86dd-f23a67f454c2"
            }
          ]
        },
        {
          "id": "36ba18d1-9863-4b08-8cea-dedab60493e2",
          "name": "downloadDocument",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/documents/:documentId/download"
              ],
              "variable": [
                {
                  "id": "documentId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Download a document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce27778f-d658-4ffe-8561-b9f09e5861d1"
            }
          ]
        },
        {
          "id": "c8daeff4-93c8-4187-a3d9-9819ba619e1e",
          "name": "getGlossaries",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/glossaries"
              ],
              "variable": [
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of glossaries."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a062bfef-7a47-41df-b9f6-14d4a2e1b2e4"
            }
          ]
        },
        {
          "id": "644f78e5-b4a7-40ec-9e41-e10d88026fbd",
          "name": "createGlossary",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/glossaries"
              ],
              "variable": [
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "glossaries",
                  "value": "{}",
                  "disabled": false,
                  "description": "You can only add one glossary, even though the name suggests multiple glossaries"
                }
              ]
            },
            "description": "Upload a new glossary."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ab03513-d236-47cb-8123-9fa3192d329d"
            }
          ]
        },
        {
          "id": "e2bd2647-026e-437d-9562-883b8b9a816a",
          "name": "deleteGlossary",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/glossaries/:glossaryId"
              ],
              "variable": [
                {
                  "id": "glossaryId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete the glossary."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0d2e4f43-1a8b-4597-9df9-76a5cf55322e"
            }
          ]
        }
      ]
    }
  ]
}