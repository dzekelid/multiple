---
swagger: "2.0"
x-collection-name: Context.IO
x-complete: 1
info:
  title: Context.IO
  description: context-io-is-the-missing-email-api-that-makes-it-easy-and-fast-to-integrate-your-users-email-data-in-your-application-
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
  /accounts/{id}/messages:
    get:
      summary: Get Accounts Messages
      description: 'Lists email messages for an account. List filters: each of the
        email, to, from, cc and bcc parameters can be set to a comma-separated list
        of email addresses. These multiple addresses are treated as an OR combination.
        You can set more than one parameter when doing this call. Multiple parameters
        are treated as an AND combination.'
      operationId: listAccountMessages_
      x-api-path-slug: accountsidmessages-get
      parameters:
      - in: query
        name: bcc
        description: Email address of a contact BCCed on the messages
      - in: query
        name: body_type
        description: Used when include_body is set to get only body parts of a given
          MIME-type (i
      - in: query
        name: cc
        description: Email address of a contact CCed on the messages
      - in: query
        name: date_after
        description: Only include messages after a given timestamp
      - in: query
        name: date_before
        description: Only include messages before a given timestamp
      - in: query
        name: email
        description: Email address of the contact for whom you want the latest messages
          exchanged with
      - in: query
        name: folder
        description: Filter messages by the folder (or Gmail label)
      - in: query
        name: from
        description: Email address of a contact messages have been received from
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: include_body
        description: Set to 1 to include message bodies in the result
      - in: query
        name: include_flags
        description: Set to 1 to include IMAP flags for this message in the result
      - in: query
        name: include_headers
        description: Can be set to 0 (default), 1 or raw
      - in: query
        name: indexed_after
        description: Only include messages indexed after a given timestamp
      - in: query
        name: indexed_before
        description: Only include messages indexed before a given timestamp
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: offset
        description: Start the list at this offset (zero-based)
      - in: query
        name: subject
        description: Get messages whose subject matches this search string
      - in: query
        name: to
        description: Email address of a contact messages have been sent to
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Messages
---