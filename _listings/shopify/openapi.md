swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/customers/3989659651/addresses/set.json:
    put:
      summary: destroying multiple customer addresses
      description: Destroying multiple customer addresses.
      operationId: putAdminCustomers3989659651AddressesSet.json
      x-api-path-slug: admincustomers3989659651addressesset-json-put
      parameters:
      - in: query
        name: address_ids[]
      - in: header
        name: Content-Type
      - in: query
        name: operation
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Destroying
      - Multiple
      - Customer
      - Addresses
  /admin/products.json:
    post:
      summary: Create a new product with multiple product variants
      description: Create a new product with multiple product variants.
      operationId: postAdminProducts.json
      x-api-path-slug: adminproducts-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Product
      - Multiple
      - Product
      - Variants