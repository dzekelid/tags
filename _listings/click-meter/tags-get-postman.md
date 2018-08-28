{
  "info": {
    "name": "Click Meter List of all the groups associated to the user filtered by this tag.",
    "_postman_id": "b82fa5af-d6f0-4f4a-9eac-888d5b228e9e",
    "description": "List of all the groups associated to the user filtered by this tag..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tags",
      "item": [
        {
          "id": "11d26bf3-063a-449e-9029-f8c6fe9f48e2",
          "name": "getTags",
          "request": {
            "url": "http://apiv2.clickmeter.com:80/tags?datapoints=%7B%7D&groups=%7B%7D&limit=%7B%7D&name=%7B%7D&offset=%7B%7D&type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of all the groups associated to the user filtered by this tag.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1b932edd-12b0-4979-8b07-c7d7f27f0a47"
            }
          ]
        }
      ]
    }
  ]
}