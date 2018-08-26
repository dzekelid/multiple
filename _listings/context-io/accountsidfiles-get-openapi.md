---
swagger: "2.0"
x-collection-name: Context.IO
x-complete: 0
info:
  title: Context.IO Get Accounts Files
  description: 'Lists files found as email attachments. List filters: each of the
    email, to, from, cc and bcc parameters can be set to a comma-separated list of
    email addresses. These multiple addresses are treated as an OR combination. You
    can set more than one parameter when doing this call. Multiple parameters are
    treated as an AND combination.'
  version: 1.0.0
host: api.context.io
basePath: /2.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{id}/files:
    get:
      summary: Get Accounts Files
      description: 'Lists files found as email attachments. List filters: each of
        the email, to, from, cc and bcc parameters can be set to a comma-separated
        list of email addresses. These multiple addresses are treated as an OR combination.
        You can set more than one parameter when doing this call. Multiple parameters
        are treated as an AND combination.'
      operationId: listAccountFiles_
      x-api-path-slug: accountsidfiles-get
      parameters:
      - in: query
        name: bcc
        description: Email address of a contact BCCed on the messages
      - in: query
        name: cc
        description: Email address of a contact CCed on the messages
      - in: query
        name: date_after
        description: Only include files attached to messages sent after a given timestamp
      - in: query
        name: date_before
        description: Only include files attached to messages sent before a given timestamp
      - in: query
        name: email
        description: Email address of the contact for whom you want the latest files
          exchanged with
      - in: query
        name: file_name
        description: Search for files based on their name
      - in: query
        name: from
        description: Email address of a contact files have been received from
      - in: query
        name: group_by_revisions
        description: If set to 1, the list will do an intelligent grouping of files
          to reflect occurrences of the same document
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: indexed_after
        description: Only include files attached to messages indexed after a given
          timestamp
      - in: query
        name: indexed_before
        description: Only include files attached to messages indexed before a given
          timestamp
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: offset
        description: Start the list at this offset (zero-based)
      - in: query
        name: to
        description: Email address of a contact files have been sent to
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Files
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