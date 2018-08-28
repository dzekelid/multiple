---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify destroying multiple customer addresses
  description: Destroying multiple customer addresses.
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