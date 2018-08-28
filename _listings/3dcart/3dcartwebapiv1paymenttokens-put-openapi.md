---
swagger: "2.0"
x-collection-name: 3dcart
x-complete: 0
info:
  title: 3dcart This method is used to update multiple paymenttokens in the database.
    No URL parameters should be included.
  version: 1.0.0
  description: This method is used to update multiple paymenttokens in the database.
    no url parameters should be included..
host: apirest.3dcart.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /3dCartWebAPI/v1/Categories:
    put:
      summary: This method is used to update multiple category records in the database.
        No {categoryid} parameters should be included.
      description: This method is used to update multiple category records in the
        database. no {categoryid} parameters should be included..
      operationId: Category_Update
      x-api-path-slug: 3dcartwebapiv1categories-put
      parameters:
      - in: body
        name: categories
        description: A Json or XML object containing the new categories
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Category
      - Records
      - In
      - Database
      - ""
      - "No"
      - Categoryid
      - Parameters
      - Should
      - Be
      - Included
  /3dCartWebAPI/v1/Customers:
    put:
      summary: This method is used to update multiple customers in the system. No
        URL parameters should be included.
      description: This method is used to update multiple customers in the system.
        no url parameters should be included..
      operationId: Customers_Update
      x-api-path-slug: 3dcartwebapiv1customers-put
      parameters:
      - in: body
        name: customers
        description: A Json or XML object containing the new customer
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Customers
      - In
      - System
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
  /3dCartWebAPI/v1/Distributors:
    put:
      summary: This method is used to update multiple distributor records in the database.
        No {distributorid} parameters should be included.
      description: This method is used to update multiple distributor records in the
        database. no {distributorid} parameters should be included..
      operationId: Distributors_Update
      x-api-path-slug: 3dcartwebapiv1distributors-put
      parameters:
      - in: body
        name: distributors
        description: A Json or XML object containing the new distributors
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Distributor
      - Records
      - In
      - Database
      - ""
      - "No"
      - Distributorid
      - Parameters
      - Should
      - Be
      - Included
  /3dCartWebAPI/v1/Manufacturers:
    put:
      summary: This method is used to update multiple manufacturers in the database.
        No URL parameters should be included.
      description: This method is used to update multiple manufacturers in the database.
        no url parameters should be included..
      operationId: Manufacturer_Update
      x-api-path-slug: 3dcartwebapiv1manufacturers-put
      parameters:
      - in: body
        name: manufacturers
        description: A Json or XML object containing the new manufacturers
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Manufacturers
      - In
      - Database
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
  /3dCartWebAPI/v1/Orders:
    put:
      summary: This method is used to update multiple orders in the database. No URL
        parameters should be included.
      description: This method is used to update multiple orders in the database.
        no url parameters should be included..
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1orders-put
      parameters:
      - in: body
        name: orders
        description: A Json or XML object containing the orders
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Orders
      - In
      - Database
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
  /3dCartWebAPI/v1/PaymentTokens:
    put:
      summary: This method is used to update multiple paymenttokens in the database.
        No URL parameters should be included.
      description: This method is used to update multiple paymenttokens in the database.
        no url parameters should be included..
      operationId: PaymentToken_Update
      x-api-path-slug: 3dcartwebapiv1paymenttokens-put
      parameters:
      - in: body
        name: paymenttokens
        description: A Json or XML object containing the new PaymentTokens
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Paymenttokens
      - In
      - Database
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
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