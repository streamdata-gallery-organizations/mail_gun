{
  "info": {
    "name": "Mailgun API Complaint",
    "_postman_id": "191cffcf-46e1-45f2-a1f7-5861d3bec60e",
    "description": "Fetches a single spam complaint by a given email address. This is useful to check if a particular user has complained.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bounces",
      "item": [
        {
          "id": "5ece5b81-5762-468e-814a-ed4390046442",
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
              "id": "aec82bc3-ff88-465c-92b5-a9a3a8eaf80e"
            }
          ]
        }
      ]
    },
    {
      "name": "Bounce",
      "item": [
        {
          "id": "1829737d-bddb-4bbd-94a3-251236f74bfb",
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
              "id": "0148241c-159c-42be-b1bf-4a9e7589e0c8"
            }
          ]
        },
        {
          "id": "7b5723b2-f62f-4e42-9336-2c00f9ebf4c3",
          "name": "getBouncesAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "bounces/:address"
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches a single bounce event by a given email address. This is useful to check if a given email address has bounced before."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f225b7f4-233e-47fd-9542-492d79f22dc9"
            }
          ]
        },
        {
          "id": "efa0b355-90fc-412d-8fee-103ae1507160",
          "name": "deleteBouncesAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "bounces/:address"
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "address",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Clears a bounce event."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ec0fd84-1941-45cc-a437-772a140c480a"
            }
          ]
        }
      ]
    },
    {
      "name": "Complaints",
      "item": [
        {
          "id": "3b489ce4-45d8-418f-b383-c8bfd8010e28",
          "name": "getComplaints",
          "request": {
            "url": "http://api.mailgun.net/v2/complaints/?limit=%7B%7D&skip=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches the list of complaints."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f94bfc7d-9d23-46c0-a8aa-f99277dd15bd"
            }
          ]
        }
      ]
    },
    {
      "name": "Complaint",
      "item": [
        {
          "id": "47a51d9b-5213-44b7-a67d-9c5d35deebfd",
          "name": "postComplaints",
          "request": {
            "url": "http://api.mailgun.net/v2/complaints/?address=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds an address to the complaints table."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d94f3e9-96a6-4447-badf-228077bc639c"
            }
          ]
        },
        {
          "id": "cfede6c8-0b96-4a9c-bfb0-771179032db2",
          "name": "getComplaintsAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "complaints/:address"
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches a single spam complaint by a given email address. This is useful to check if a particular user has complained."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84700242-a68e-461c-a35c-fa518d6eb6ab"
            }
          ]
        },
        {
          "id": "bce5cfe6-dc21-4bf0-a0f2-1f435c48fb86",
          "name": "deleteComplaintsAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "complaints/:address"
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a given spam complaint."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "304feba5-9460-4e5e-a418-1207f9c7fae7"
            }
          ]
        }
      ]
    }
  ]
}