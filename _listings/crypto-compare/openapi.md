swagger: "2.0"
x-collection-name: Crypto Compare
x-complete: 1
info:
  title: Cryptocompare
  description: todo-add-description
  version: 1.0.0
host: min-api.cryptocompare.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /data/pricemulti:
    get:
      summary: Get Multiple Prices
      description: Get multiple prices.
      operationId: DataPricemultiGet
      x-api-path-slug: datapricemulti-get
      parameters:
      - in: query
        name: fsyms
      - in: query
        name: tsyms
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Multiple
      - Prices