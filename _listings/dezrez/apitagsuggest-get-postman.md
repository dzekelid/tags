{
  "info": {
    "name": "Dezrez Get tag suggestions for value",
    "_postman_id": "fffd9664-215e-463e-ab7c-305668dba23c",
    "description": "Get tag suggestions for value.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Enum",
      "item": [
        {
          "id": "01b79a79-bb78-4ec6-9a16-cd9153ae47de",
          "name": "Enum_SuggestBytypeNameBysystemName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/enum/suggest/:typeName/:systemName"
              ],
              "variable": [
                {
                  "id": "systemName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "typeName",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get enum suggestions for value."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6ce9e09-ffdd-42f1-9e73-fd8089d0ba11"
            }
          ]
        }
      ]
    },
    {
      "name": "Feature",
      "item": [
        {
          "id": "9071cd68-f80b-4d7e-9f19-ebb2082f52f5",
          "name": "Feature_SuggestByname",
          "request": {
            "url": "http://api.dezrez.com/api/feature/suggest?name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get feature suggestions for value."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07daa5bc-cb8c-4202-9959-d2b60887f42a"
            }
          ]
        }
      ]
    },
    {
      "name": "Tag",
      "item": [
        {
          "id": "de12de41-9460-4587-ae96-d0d1c89808b9",
          "name": "Tag_SuggestByname",
          "request": {
            "url": "http://api.dezrez.com/api/tag/suggest?name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get tag suggestions for value."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3445d5ee-c63b-4948-9e1f-d09094f34916"
            }
          ]
        }
      ]
    }
  ]
}