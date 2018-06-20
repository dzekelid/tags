{
  "info": {
    "name": "AWS CloudSearch Add Tags",
    "_postman_id": "11115b6f-b6dc-47b5-88bd-002a3bf8df5b",
    "description": "Attaches resource tags to an\n Amazon CloudSearch domain.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tags",
      "item": [
        {
          "id": "be03c10a-e3bf-4090-baee-bad211d62e1f",
          "name": "AddTags",
          "request": {
            "url": "http://example.com/api/?Action=AddTags?Base=Base&InternalException=InternalException&LimitExceededException=LimitExceededException&ValidationException=ValidationException",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches resource tags to an\n Amazon CloudSearch domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ca85bf1-1513-492d-ad45-843180af94bd"
            }
          ]
        }
      ]
    }
  ]
}