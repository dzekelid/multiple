{
  "info": {
    "name": "Plentymarkets Create multiple correlations",
    "_postman_id": "39400080-2db1-4807-99d5-3545725ecce4",
    "description": "Creates multiple correlations. The type, market settings ID and the correlation ID for each param combination must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Multiple",
      "item": [
        {
          "id": "c02574ba-a108-4485-8642-47ec8b9237cc",
          "name": "deleteRestFeedbacksDeleteFeedbacksFeedbacks",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/feedbacks/delete_feedbacks/:feedbackIds"
              ],
              "variable": [
                {
                  "id": "feedbackIds",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
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
            "description": "Deletes multiple feedbacks. A list with IDs of feedbacks must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a60368f6-72d2-46b4-b5cd-187c5019a60f"
            }
          ]
        },
        {
          "id": "65d673c0-213d-46f9-a4df-edb9fa69b9d0",
          "name": "postRestMarketsSettingsCorrelationsBulk",
          "request": {
            "url": "http://example.com/rest/markets/settings/correlations/bulk",
            "method": "POST",
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
            "description": "Creates multiple correlations. The type, market settings ID and the correlation ID for each param combination must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6ebbb3a-afe8-4a4d-8733-58b928168b98"
            }
          ]
        }
      ]
    },
    {
      "name": "Visibility",
      "item": [
        {
          "id": "97f00cc4-3434-4e79-9310-214d417ef083",
          "name": "putRestFeedbacksFeedbacksVisibility",
          "request": {
            "url": "http://example.com/rest/feedbacks/feedbacks_visibility?feedbackIds=%7B%7D&isVisible=%7B%7D",
            "method": "PUT",
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
            "description": "Updates the visibility of multiple feedbacks. A list with IDs of feedbacks must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dded194f-46f7-4f02-a773-866bb589a1cf"
            }
          ]
        }
      ]
    }
  ]
}