{
  "info": {
    "name": "Steem get_discussions_by_author_before_date",
    "_postman_id": "26478282-7eb7-431d-8616-fdd742819124",
    "description": "get_discussions_by_author_before_date",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Get",
      "item": [
        {
          "id": "2586c689-4555-4067-9832-539b9625aa38",
          "name": "get-discussions-by-author-before-date",
          "request": {
            "url": "http://api.steemjs.com/get_discussions_by_author_before_date?author=%7B%7D&beforeDate=%7B%7D&limit=%7B%7D&startPermlink=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "get_discussions_by_author_before_date"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "755c8a08-6027-4467-ae1d-beea2f7654e1"
            }
          ]
        }
      ]
    }
  ]
}