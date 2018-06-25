{
  "info": {
    "name": "Pay Run.IO Get all pay schedule tags",
    "_postman_id": "85cfd448-d3cb-4f69-bb17-6924af59e0da",
    "description": "Gets all the tags from the pay schedule",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Employee",
      "item": [
        {
          "id": "c329ea19-921b-468f-8ad7-8817ccc4deb9",
          "name": "GetTagsFromEmployee",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/Employee/:EmployeeId/Tags"
              ],
              "variable": [
                {
                  "id": "EmployeeId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the tags from the employee"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff12e4fb-1267-410a-80f9-53f8b4efc183"
            }
          ]
        },
        {
          "id": "a6217797-87f5-4b28-8b57-3a33ff55f53d",
          "name": "GetTagsFromEmployeeRevision",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/Employee/:EmployeeId/Tags/:EffectiveDate"
              ],
              "variable": [
                {
                  "id": "EffectiveDate",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "EmployeeId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the tags from the employee revision"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "17dcc0b2-0712-40b1-b96d-de446c3e52e8"
            }
          ]
        },
        {
          "id": "3d099019-909f-4307-8630-7e41c5851981",
          "name": "GetAllEmployeeTags",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/Employees/Tags"
              ],
              "variable": [
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the employee tags"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f4d11adb-19ec-4ff8-b67f-abd820879752"
            }
          ]
        }
      ]
    },
    {
      "name": "Pay",
      "item": [
        {
          "id": "e6ea1789-fc7e-4036-8e49-a7227b47b4ab",
          "name": "GetTagsFromPayCode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/PayCode/:PayCodeId/Tags"
              ],
              "variable": [
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "PayCodeId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the tags from the pay code"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2553b11d-5223-4a99-905c-b7b991d9b292"
            }
          ]
        },
        {
          "id": "8f705088-809d-4d63-846c-f9b94b1eccbe",
          "name": "GetAllPayCodeTags",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/PayCodes/Tags"
              ],
              "variable": [
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the pay code tags"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "55ac6f1a-fd7a-4b4a-aad7-a3571632c4c6"
            }
          ]
        },
        {
          "id": "ccf0e94d-f851-4d11-b954-c1cda83dc3ab",
          "name": "GetTagsFromPayRun",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/PaySchedule/:PayScheduleId/PayRun/:PayRunId/Tags"
              ],
              "variable": [
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "PayRunId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "PayScheduleId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the tags from the pay run"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7907725c-7f7e-4ba0-ba68-7a6753b7fc04"
            }
          ]
        },
        {
          "id": "5abe8c00-d445-480f-bdb3-89222eb2403f",
          "name": "GetAllPayRunTags",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/PaySchedule/:PayScheduleId/PayRuns/Tags"
              ],
              "variable": [
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "PayScheduleId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the pay run tags"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a702683-59fe-48d7-b624-802c9c1921f2"
            }
          ]
        },
        {
          "id": "86272092-b9c7-457c-bbf6-139e4fb1d26e",
          "name": "GetTagsFromPaySchedule",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/PaySchedule/:PayScheduleId/Tags"
              ],
              "variable": [
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "PayScheduleId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the tags from the pay schedule"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f22c74b7-4633-4950-b00e-5a3567f4fb92"
            }
          ]
        }
      ]
    }
  ]
}