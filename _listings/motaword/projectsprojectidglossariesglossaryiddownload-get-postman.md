{
  "info": {
    "name": "Mota Word Download a glossary",
    "_postman_id": "7e022fd9-3c83-4b3f-b809-83f834d9f985",
    "description": "Download a glossary.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Projects",
      "item": [
        {
          "id": "180cbc51-ac9c-45a6-a13b-22357aae54a9",
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
              "id": "dcb8a7c9-7c1f-4d4c-a5a6-f1edfa4696c9"
            }
          ]
        },
        {
          "id": "2f3b1eea-9a39-4117-8e24-008806e8c33a",
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
              "id": "d7f9c1f7-2eb9-492e-acf5-e0249af6aa71"
            }
          ]
        },
        {
          "id": "fce159dd-976e-4a1f-a824-005642aeb428",
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
              "id": "a52e0171-74a0-4335-89f9-06037528c0cb"
            }
          ]
        },
        {
          "id": "8826e127-ddc7-4875-8bbe-0857298dee9d",
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
              "id": "91f43a1f-c756-4966-ad44-3c1aa5dbfb4e"
            }
          ]
        },
        {
          "id": "627d91ff-3916-4a48-b73c-a1cc118e664e",
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
              "id": "67326b44-8510-445e-847e-0ed6c7faebcf"
            }
          ]
        },
        {
          "id": "e4f9634e-ff24-4526-a1b0-170715590c4f",
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
              "id": "d83314a5-86ab-487f-98dc-f5f95ed4202b"
            }
          ]
        },
        {
          "id": "be0860ba-bb41-4df5-8e4a-c457e66ff4fc",
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
              "id": "dfdc01ed-25f4-4b28-87c2-edc5ca54d765"
            }
          ]
        },
        {
          "id": "49811673-bd7e-4fb8-bc81-fbce3afe8654",
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
              "id": "85848297-ecde-4af8-9ef1-0942a5d125cb"
            }
          ]
        },
        {
          "id": "276f75c0-f0ff-4169-b729-94658fcdc583",
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
              "id": "5cf085af-55cd-4583-9bd4-5d02bcd95d92"
            }
          ]
        },
        {
          "id": "9b6303f9-f57b-4c1f-b379-b0829ba775c7",
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
              "id": "a31fb3f1-78e5-4dcf-b918-77e5cfdf5d58"
            }
          ]
        },
        {
          "id": "261029fb-ada9-43e6-976c-a167b13062ec",
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
              "id": "d8b53401-a796-4e89-aa76-d41ba40e505f"
            }
          ]
        },
        {
          "id": "1ceb7084-e72f-49a6-9e7c-b14a3e442339",
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
              "id": "cb57698e-05b8-4b2f-a3e8-388d5223a32a"
            }
          ]
        },
        {
          "id": "961d7c35-ca9c-44c0-aea9-2298be1df528",
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
              "id": "06f74806-5d51-4fc0-aecb-0eb9d004b243"
            }
          ]
        },
        {
          "id": "41515a1b-cc18-457b-bd04-13c7fd218bc2",
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
              "id": "d9a7af06-ba7a-4d7d-a750-99ce71479e6b"
            }
          ]
        },
        {
          "id": "92a4732b-77e4-4df6-92a9-8056d7d41e54",
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
              "id": "627a4e93-d58d-4897-ac26-3ac347b4bf1f"
            }
          ]
        },
        {
          "id": "2ebd7840-2a35-4d8e-be3c-6aea7c4948e7",
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
              "id": "9c95e78b-a4ae-4f22-9978-6bec5105a6de"
            }
          ]
        },
        {
          "id": "e01ca3f5-f499-497a-a6a5-7d707e9f7443",
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
              "id": "6a4a64dc-e34f-4ab8-8e65-25e415f844ed"
            }
          ]
        },
        {
          "id": "4debc730-0df6-48a8-a61a-711b74e65101",
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
              "id": "0f2ac511-d1bd-408a-a2c1-308f9cdfd00b"
            }
          ]
        },
        {
          "id": "ea63b97d-c9d5-4d34-8dc2-db1f82b191bd",
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
              "id": "e6e964c3-0bd7-4d2c-9c99-f7aee30f8274"
            }
          ]
        },
        {
          "id": "c0b144bc-12ff-4ca3-a661-21fc1512fe3b",
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
              "id": "c4624d35-c453-4ccd-9782-eda35fbd4f68"
            }
          ]
        },
        {
          "id": "ee6647b3-7053-473e-a5cc-7a3278898909",
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
              "id": "89180c9e-61fb-4def-829e-91327cb60e40"
            }
          ]
        },
        {
          "id": "09a0f89a-03f5-42ae-87ba-09926f1b768b",
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
              "id": "7f07098a-27d8-4a13-b1e5-96a8e141b80c"
            }
          ]
        },
        {
          "id": "9918ded3-8891-4061-8bf3-d7a7c345bb31",
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
              "id": "3e85ad10-e8ef-4205-996c-b373bfba387b"
            }
          ]
        },
        {
          "id": "69c861e9-44f7-4bb0-bc2f-abc1c8bc93c8",
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
              "id": "d48183ce-3151-4c59-b485-39b59c73f09f"
            }
          ]
        },
        {
          "id": "c8b62401-5ec5-49b7-b4c7-c66ff253c87b",
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
              "id": "e7386c36-9454-4908-87d3-747c9542cb35"
            }
          ]
        },
        {
          "id": "8935b66e-b9e7-4067-924c-3cf6b3a6edbe",
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
              "id": "0f0327ae-e8e1-4822-a20b-d315c85a2597"
            }
          ]
        },
        {
          "id": "34881fca-7cd4-4a23-85d3-b272db041ded",
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
              "id": "e9466fd0-f1a1-4ca7-bfc7-bdb829c4ff84"
            }
          ]
        },
        {
          "id": "a2c69658-8360-453b-8961-01295382c1d8",
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
              "id": "aa435cfb-ea79-4268-bc24-321f27656af2"
            }
          ]
        },
        {
          "id": "3f132234-4055-4670-9f4e-9c34a0036b7d",
          "name": "getGlossary",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get single glossary."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ec98fd0-06af-4785-b3f8-fecf7df31bd6"
            }
          ]
        },
        {
          "id": "1dda8c42-7deb-40c6-9962-c91277b772c9",
          "name": "updateGlossary",
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
            "method": "PUT",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "glossaries",
                  "value": "{}",
                  "disabled": false,
                  "description": "Single file data"
                }
              ]
            },
            "description": "Update the glossary. File name and contents will replaced with the new one."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70001a0c-1527-4a29-93a9-2be1af3a8cf2"
            }
          ]
        },
        {
          "id": "e9dcd4fe-16a7-4390-94ca-bc4d7d081f2b",
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
              "id": "32ac3faf-cf78-4450-92fc-64237133f770"
            }
          ]
        },
        {
          "id": "1ae15ee2-deb3-40f0-ac5c-166c6422cd6c",
          "name": "downloadGlossary",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/glossaries/:glossaryId/download"
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Download a glossary."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "541ded1b-a7a0-4b3d-a200-69c4dbf9a0a0"
            }
          ]
        }
      ]
    }
  ]
}