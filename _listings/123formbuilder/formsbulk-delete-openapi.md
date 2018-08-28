---
swagger: "2.0"
x-collection-name: 123FormBuilder
x-complete: 0
info:
  title: 123FormBuilder Delete multiple forms
  version: 1.0.0
  description: Delete multiple forms
host: api.123contactform.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /forms/bulk:
    delete:
      summary: Delete multiple forms
      description: Delete multiple forms
      operationId: delete-multiple-forms
      x-api-path-slug: formsbulk-delete
      parameters:
      - in: formData
        name: form_ids
        description: The IDs of the forms separated by comma
      - in: formData
        name: JWT
        description: JWT authentication token
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Forms
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