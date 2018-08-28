{
  "info": {
    "name": "Sustainable Facilities Tool API Tags",
    "_postman_id": "89b38978-d71c-4064-b752-6669fde6b0d5",
    "description": "Returns all search tags.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "tags",
      "item": [
        {
          "id": "2f674d23-cb6a-4d9a-85e6-64e451b9e37b",
          "name": "getTags",
          "request": {
            "url": "http://api.data.gov/sftool/v1/tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all search tags"
          },
          "response": [
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "[\r\n  {\r\n    \"id\": \"id\",\r\n    \"name\": \"name\"\r\n  }\r\n]",
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "c51dbc32-8cbd-47f5-86d6-2cfe1496c2a5"
            }
          ]
        }
      ]
    }
  ]
}