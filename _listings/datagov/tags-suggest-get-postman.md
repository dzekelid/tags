{
  "info": {
    "name": "Data.gov API Get Tags Suggest",
    "_postman_id": "1f8ae17e-dc2f-4680-8fa2-f01f2914a624",
    "description": "Suggest tags",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "tags",
      "item": [
        {
          "id": "3d331bbf-6abe-47a3-99cf-d5a509b75363",
          "name": "getTagsSuggest",
          "request": {
            "url": "http://catalog.data.gov/api/3/tags/suggest/?q=%7B%7D&size=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Suggest tags"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "afda6c7a-8bb9-46ad-be36-51d6e0e491eb"
            }
          ]
        }
      ]
    }
  ]
}