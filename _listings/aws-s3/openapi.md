---
swagger: "2.0"
x-collection-name: AWS S3
x-complete: 1
info:
  title: No Title
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?delete:
    post:
      summary: Delete Multiple Objects
      description: The Multi-Object Delete operation enables you to delete multiple
        objects from a bucketusing a single HTTP request
      operationId: delete-multiple-objects
      x-api-path-slug: delete-post
      parameters:
      - in: header
        name: Content-Length
        description: Length of the body according to RFC 2616
      - in: header
        name: Content-MD5
        description: The base64-encoded 128-bit MD5 digest of the data
      - in: header
        name: x-amz-mfa
        description: The value is the concatenation of the authentication devices
          serial number, a space,tttttttttand the value that is displayed on your
          authenticationtttttttttdevice
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Objects
---