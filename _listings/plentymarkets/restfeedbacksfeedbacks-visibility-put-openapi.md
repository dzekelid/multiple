---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Update the visibility of multiple feedbacks
  description: Updates the visibility of multiple feedbacks. A list with IDs of feedbacks
    must be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/feedbacks/delete_feedbacks/{feedbackIds}:
    delete:
      summary: Delete multiple feedbacks
      description: Deletes multiple feedbacks. A list with IDs of feedbacks must be
        specified.
      operationId: deleteRestFeedbacksDeleteFeedbacksFeedbacks
      x-api-path-slug: restfeedbacksdelete-feedbacksfeedbackids-delete
      parameters:
      - in: path
        name: feedbackIds
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Feedbacks
  /rest/feedbacks/feedbacks_visibility:
    put:
      summary: Update the visibility of multiple feedbacks
      description: Updates the visibility of multiple feedbacks. A list with IDs of
        feedbacks must be specified.
      operationId: putRestFeedbacksFeedbacksVisibility
      x-api-path-slug: restfeedbacksfeedbacks-visibility-put
      parameters:
      - in: query
        name: feedbackIds
        description: The list of feedback IDs, separated by commas
      - in: query
        name: isVisible
        description: The visibility value
      responses:
        200:
          description: OK
      tags:
      - Visibility
      - Of
      - Multiple
      - Feedbacks
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---