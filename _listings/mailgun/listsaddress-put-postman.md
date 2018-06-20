{
  "info": {
    "name": "Mailgun API Update List",
    "_postman_id": "9a30f47a-923e-4089-90f6-bba0628d7303",
    "description": "Update mailing list properties, such as address, description or name",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bounces",
      "item": [
        {
          "id": "3b52665d-7fc5-4e6f-8541-48d1c968a064",
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
              "id": "4bbf955b-939b-49d0-9307-0366e324b404"
            }
          ]
        }
      ]
    },
    {
      "name": "Bounce",
      "item": [
        {
          "id": "d9ac5c03-cb22-4978-9ad0-475338c3b3db",
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
              "id": "920c38e5-c5de-4234-8b72-5804b561e67d"
            }
          ]
        },
        {
          "id": "32c8efc4-059f-472d-87a5-9b18b3ac26bf",
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
              "id": "bec9eee2-5504-4db9-be00-474d6c5e24a6"
            }
          ]
        },
        {
          "id": "2928109c-d080-4a1d-89c8-29ebd78fbb85",
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
              "id": "7809dd6b-282f-42ca-8f68-ec9f9c91f6c8"
            }
          ]
        }
      ]
    },
    {
      "name": "Complaints",
      "item": [
        {
          "id": "86d95948-6404-41e7-bbd7-7e8b3ec4d1b3",
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
              "id": "ec4bdbe7-56af-47ac-8182-497cc384ef3f"
            }
          ]
        }
      ]
    },
    {
      "name": "Complaint",
      "item": [
        {
          "id": "62cc8f2d-dc0d-4dbe-b04b-2611e8ebe789",
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
              "id": "dc73dbf4-7cfa-4c25-9c1b-1f0fce72b96e"
            }
          ]
        },
        {
          "id": "4a3318d5-a844-4ba1-8d88-ea1a292cbada",
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
              "id": "a624ad5b-cb45-4d59-96e5-6825624ccf08"
            }
          ]
        },
        {
          "id": "feaef50e-19d0-497a-9142-58fd8ece0f6c",
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
              "id": "bd7f6ca9-e2db-4d55-8430-6f47705e00e6"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "204599a0-5d5f-45a9-a4d1-84999cb81d4e",
          "name": "postLists",
          "request": {
            "url": "http://api.mailgun.net/v2/lists?access_level=%7B%7D&address=%7B%7D&description=%7B%7D&name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new mailing list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "112f3693-f9f2-44fb-9996-70f84ee2114e"
            }
          ]
        },
        {
          "id": "fe235b32-18d5-4a8e-add6-31af970257d9",
          "name": "getListsAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "lists/:address"
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
            "description": "Returns a single mailing list by a given address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d12a6d31-1b86-48f5-b316-7fca006ce7ec"
            }
          ]
        },
        {
          "id": "2a13a8ae-7779-4083-bf5b-1cf0957e6566",
          "name": "putListsAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "lists/:address"
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "address",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update mailing list properties, such as address, description or name"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d52284e-9b00-4d67-869e-baaea77c2712"
            }
          ]
        },
        {
          "id": "8c32215f-388a-4bbe-b76a-db7eb6e3eec4",
          "name": "deleteListsAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "lists/:address"
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
            "description": "Deletes a mailing list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93fac7b0-4b23-47db-bb66-84eb66ced0c3"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "a27f83d7-57b3-4aef-969b-146f6865748b",
          "name": "getLists",
          "request": {
            "url": "http://api.mailgun.net/v2/lists/?access_level=%7B%7D&address=%7B%7D&description=%7B%7D&limit=%7B%7D&namespace_id=%7B%7D&skip=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of mailing lists under your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0818e13-d08c-4862-943f-f26eb214700a"
            }
          ]
        }
      ]
    }
  ]
}