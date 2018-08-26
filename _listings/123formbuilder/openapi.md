---
swagger: "2.0"
x-collection-name: 123FormBuilder
x-complete: 1
info:
  title: ""
  version: 1.0.0
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
---