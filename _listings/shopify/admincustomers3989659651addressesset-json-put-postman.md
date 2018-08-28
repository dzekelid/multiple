{
  "info": {
    "name": "Shopify destroying multiple customer addresses",
    "_postman_id": "efe03183-8e3b-41ff-be7d-0d9a91a1e99e",
    "description": "Destroying multiple customer addresses.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Commerce",
      "item": [
        {
          "id": "bca8a0ab-ee26-4646-a219-95f56950b75c",
          "name": "getAdminCustomers3989659651Addresses.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/customers/3989659651/addresses.json",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get all of a customer's addresses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f01d4bb-02af-44c2-be01-c69dd428fc8f"
            }
          ]
        },
        {
          "id": "a815f3b5-6a68-415d-87c1-127f6494935e",
          "name": "putAdminCustomers3989659651AddressesSet.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/customers/3989659651/addresses/set.json?address_ids=%5B%7B%7D%5D&operation=%7B%7D",
            "method": "PUT",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Destroying multiple customer addresses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90c64cc0-8506-4492-9eed-8c3381d11818"
            }
          ]
        }
      ]
    }
  ]
}