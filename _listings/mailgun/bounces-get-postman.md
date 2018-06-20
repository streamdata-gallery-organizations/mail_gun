{
  "info": {
    "name": "Mailgun API Bounces",
    "_postman_id": "6e618192-4290-4c06-9120-bf82b7dbd159",
    "description": "Fetches the list of bounces.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bounces",
      "item": [
        {
          "id": "3e8a9e7b-c1d5-4f11-9d95-35067d9ec830",
          "name": "getBounces",
          "request": {
            "url": "http://api.mailgun.net/v2/bounces/?limit=%7B%7D&skip=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches the list of bounces."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9767662-1677-4903-9c3f-26992ba157f9"
            }
          ]
        }
      ]
    }
  ]
}