{
  "info": {
    "name": "Mailgun API Add Bounce",
    "_postman_id": "484ed9e9-b124-476c-a6cf-458c3bbdc924",
    "description": "Adds a permanent bounce to the bounces table. Updates the existing record if already here.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bounces",
      "item": [
        {
          "id": "c391acb8-89db-46c9-a2eb-7c2700657822",
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
              "id": "23ad6029-0357-4df3-a178-b2afb857b584"
            }
          ]
        }
      ]
    },
    {
      "name": "Bounce",
      "item": [
        {
          "id": "dc8f0693-ad4c-48c9-87c7-dd81af4c9882",
          "name": "postBounces",
          "request": {
            "url": "http://api.mailgun.net/v2/bounces/?address=%7B%7D&code=%7B%7D&error=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a permanent bounce to the bounces table. Updates the existing record if already here."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c41c9297-0f91-4e34-91ab-22eb4214ec6a"
            }
          ]
        }
      ]
    }
  ]
}