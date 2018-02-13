
# Webhooks

## Get All Webhooks

```shell
curl "https://api.ordermentum.com/v1/webhooks"
  -H "Authorization: Bearer UNIQUE_TOKEN"
```

> The above command returns JSON structured like this:

```json
{
  "meta": {
    "totalResults": 10,
    "totalPages": 1,
    "pageSize": 25,
    "pageNo": 1
  },
  "links": {
    "self": "https://app.ordermentum.com/v1/products?supplierId=a5cad00b-0c85-4d95-ab3f-9fb1933dbeed&pageNo=3",
    "first": "https://app.ordermentum.com/v1/products?supplierId=bd4b8236-1649-49a5-aa6e-2d0f0e9407ea&pageNo=1",
    "prev": "https://app.ordermentum.com/v1/products?supplierId=44c2ae51-b2eb-4f86-b021-fc7d181f5b65&pageNo=2",
    "next": "https://app.ordermentum.com/v1/products?supplierId=561b48a5-f292-4f5c-abfe-3d7ff70ee91b&pageNo=4",
    "last": "https://app.ordermentum.com/v1/products?supplierId=5331fea9-52e3-427d-bae8-57f1b7c7edd8&pageNo=9"
  },
  "data": [
    {
      "id": "b1da7ace-824e-4e69-8463-f0c70d7fac0b",
      "name": "Order - #OM155",
      "purchaserId": {},
      "supplierId": "503be8e5-15cb-4aa1-bf9b-15c28dff0fb4",
      "retailerId": "7492729e-980d-49e0-a1f5-6812bef9bfdf",
      "retailerName": "Caroline's Cafe",
      "retailerAlias": "Caroline's Cafe and Carafes",
      "orderNumber": "OM155",
      "number": "OM155",
      "retailer": {
        "id": "a17ff909-81a3-4850-a4c4-923bcfac6b30",
        "createdAt": "2016-12-01T05:44:59.223Z",
        "updatedAt": "2016-12-01T05:44:59.223Z",
        "name": "Eric's Excellent Eats Pty Ltd",
        "legalName": "Eric's Excellent Eats Pty Ltd",
        "tradingName": "Everyone Eat Eric",
        "email": "accounts@example.com",
        "phone": "+61438888888",
        "liquorLicense": "FIXME",
        "abn": "51600457412",
        "suppliers": [
          {}
        ]
      },
      "purchaser": {
        "id": "863fcb9d-29a4-4968-88a9-b149579b98c4",
        "createdAt": "2016-12-01T05:44:59.223Z",
        "updatedAt": "2016-12-01T05:44:59.223Z",
        "deletedAt": {},
        "activatedAt": {},
        "reference": "FIXME",
        "name": "Pete's Pun Parlour",
        "retailerAlias": "Punny Pete",
        "retailerLegalName": "Pun Purveyors Pty",
        "retailerTradingName": "Papa Pete's Patented Puns",
        "retailerPhone": "0488888888",
        "retailerEmail": "accounts@example.com",
        "retailerAddressLine": "123 Fake St, FakeTown, NSW, 2086",
        "retailerId": "aa4b813d-0a8f-4b05-9f9a-4241246d9082",
        "supplierId": "985f5798-c792-428e-8287-243099d7e26c",
        "paymentMethodType": "card",
        "invoiceSetting": "on_delivery",
        "invoiceFrequency": "on_place",
        "paymentTerms": "Statement 14 days",
        "paymentDelay": 7,
        "paymentMethodId": {},
        "paymentSchedule": "immediate",
        "freightGroupId": {},
        "visibilityGroupId": {},
        "priceGroupId": {},
        "stopCredit": false,
        "minimumOrderValue": "100.34",
        "disabled": false,
        "deliveryInstructions": {},
        "notes": {},
        "schedules": [
          {}
        ],
        "externalCustomerId": {}
      },
      "paymentMethodType": "card",
      "paymentDelay": 7,
      "directProcessing": false,
      "paidToSupplier": "2016-12-01T05:44:59.223Z",
      "invoiceNumber": "OM127",
      "invoice": {
        "id": {},
        "dueAt": {},
        "paidAt": {},
        "updatedAt": {},
        "cancelledAt": {},
        "submittedAt": {},
        "updatedBy": {},
        "processing": {},
        "paidSupplierAt": {}
      },
      "invoiceId": {},
      "dueAt": "2016-12-01T05:44:59.223Z",
      "status": "Paid",
      "type": "auto",
      "freight": 10.23,
      "totalFreight": 10,
      "totalCost": 140.2,
      "subtotal": 135.2,
      "totalGst": 5,
      "total": 150.2,
      "paidAt": "2016-12-01T05:44:59.223Z",
      "paidBy": "bd7bd2fe-0588-46c7-acd7-1fbca468ec77",
      "isOutstanding": false,
      "products": [
        {
          "id": "5846b780-c4fa-40a3-b662-be5aa15c415c",
          "createdAt": "2016-12-01T05:44:59.223Z",
          "updatedAt": "2016-12-01T05:44:59.223Z",
          "deletedAt": "2016-12-01T05:44:59.223Z",
          "updatedById": "64a01c74-1dc7-4fa5-b20d-afe9da81b83b",
          "deletedById": "2202dc91-5aed-4825-86a8-a1bacd98e5bf",
          "externalId": {},
          "universalId": "96264694-0f2c-4ab0-86f1-911283ca2218",
          "supplierId": "8990a258-06b1-4eea-a00d-181e96545158",
          "categoryId": "8943e5ca-bb7e-4d9a-84a4-e13f71da6ad1",
          "description": {},
          "name": "1kg Sourdough",
          "SKU": "SRBR1243",
          "salesCode": "SRBR0001",
          "basePrice": "25.2727",
          "activatedAt": "2016-12-01T05:44:59.223Z",
          "sortOrder": 5,
          "image": {
            "secure_url": "https://res.cloudinary.com/ordermentum/image/upload/fake_file_name_goes_here.jpg"
          },
          "unit": "Loaves",
          "uom": "Cans",
          "weight": {}
        }
      ],
      "lineItems": [
        {
          "id": "4bd11a0e-86b3-46b8-a610-9ece5e4d3131",
          "createdAt": "2016-12-01T05:44:59.223Z",
          "updatedAt": "2016-12-01T05:44:59.223Z",
          "name": "1kg Sourdough",
          "SKU": "SRBR1243",
          "orderId": "5f6794ee-41f2-40fe-b6f3-ede4ebec49c3",
          "productId": "93335816-80c1-4d55-8da9-82e06b629ac3",
          "price": "60.00",
          "quantity": 1,
          "subtotal": "60.00",
          "taxable": true,
          "totalWeight": "20.23"
        }
      ],
      "lineCount": 14,
      "productCount": 43,
      "comment": {},
      "reference": "BREAD1234",
      "editable": false,
      "chargable": false,
      "chargedAt": "2016-12-01T05:44:59.223Z",
      "chargedBy": "904e2886-68dc-44ca-b68c-c7dae789528a",
      "cancelledAt": {},
      "cancelledBy": "646f0e60-9b70-41c1-9b61-8df49e8be450",
      "canMarkAsPaid": false,
      "createdAt": "2016-12-01T05:44:59.223Z",
      "placedOn": "2016-12-01T05:44:59.223Z",
      "createdBy": "cb8898d9-6072-4e2a-be8a-44409606322c",
      "chargedByUser": "Freddy Muggins",
      "deliveryDate": "2016-12-01T05:44:59.223Z",
      "updatedAt": "2016-12-01T05:44:59.223Z",
      "deletedAt": "2016-12-01T05:44:59.223Z",
      "updatedBy": "2e5bdba0-a650-4bb5-a2c1-5eb7a20d1f5d"
    }
  ]
}
```

This endpoint retrieves all webhooks.

### HTTP Request

`GET http://app.ordermentum.com/v1/webhooks`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
pageNo | 1 | Page number
pageSize | 25 | Number of webhooks in the response
retailerId | null | The retailer to retreive the webhooks for
supplierId | null | The supplier to retreive the webhooks for

## Get a Specific Order

```shell
curl "http://app.ordermentum.com/v1/webhooks/69B34C71-3D61-4D40-92DE-BD7954D26BD2"
  -H "Authorization: Bearer UNIQUE_TOKEN"
```

> The above command returns JSON structured like this:

```json
{
  "id": "b1da7ace-824e-4e69-8463-f0c70d7fac0b",
  "name": "Order - #OM155",
  "purchaserId": {},
  "supplierId": "503be8e5-15cb-4aa1-bf9b-15c28dff0fb4",
  "retailerId": "7492729e-980d-49e0-a1f5-6812bef9bfdf",
  "retailerName": "Caroline's Cafe",
  "retailerAlias": "Caroline's Cafe and Carafes",
  "orderNumber": "OM155",
  "number": "OM155",
  "retailer": {
    "id": "a17ff909-81a3-4850-a4c4-923bcfac6b30",
    "createdAt": "2016-12-01T05:44:59.223Z",
    "updatedAt": "2016-12-01T05:44:59.223Z",
    "name": "Eric's Excellent Eats Pty Ltd",
    "legalName": "Eric's Excellent Eats Pty Ltd",
    "tradingName": "Everyone Eat Eric",
    "email": "accounts@example.com",
    "phone": "+61438888888",
    "liquorLicense": "FIXME",
    "abn": "51600457412",
    "suppliers": [
      {}
    ]
  },
  "purchaser": {
    "id": "863fcb9d-29a4-4968-88a9-b149579b98c4",
    "createdAt": "2016-12-01T05:44:59.223Z",
    "updatedAt": "2016-12-01T05:44:59.223Z",
    "deletedAt": {},
    "activatedAt": {},
    "reference": "FIXME",
    "name": "Pete's Pun Parlour",
    "retailerAlias": "Punny Pete",
    "retailerLegalName": "Pun Purveyors Pty",
    "retailerTradingName": "Papa Pete's Patented Puns",
    "retailerPhone": "0488888888",
    "retailerEmail": "accounts@example.com",
    "retailerAddressLine": "123 Fake St, FakeTown, NSW, 2086",
    "retailerId": "aa4b813d-0a8f-4b05-9f9a-4241246d9082",
    "supplierId": "985f5798-c792-428e-8287-243099d7e26c",
    "paymentMethodType": "card",
    "invoiceSetting": "on_delivery",
    "invoiceFrequency": "on_place",
    "paymentTerms": "Statement 14 days",
    "paymentDelay": 7,
    "paymentMethodId": {},
    "paymentSchedule": "immediate",
    "freightGroupId": {},
    "visibilityGroupId": {},
    "priceGroupId": {},
    "stopCredit": false,
    "minimumOrderValue": "100.34",
    "disabled": false,
    "deliveryInstructions": {},
    "notes": {},
    "schedules": [
      {}
    ],
    "externalCustomerId": {}
  },
  "paymentMethodType": "card",
  "paymentDelay": 7,
  "directProcessing": false,
  "paidToSupplier": "2016-12-01T05:44:59.223Z",
  "invoiceNumber": "OM127",
  "invoice": {
    "id": {},
    "dueAt": {},
    "paidAt": {},
    "updatedAt": {},
    "cancelledAt": {},
    "submittedAt": {},
    "updatedBy": {},
    "processing": {},
    "paidSupplierAt": {}
  },
  "invoiceId": {},
  "dueAt": "2016-12-01T05:44:59.223Z",
  "status": "Paid",
  "type": "auto",
  "freight": 10.23,
  "totalFreight": 10,
  "totalCost": 140.2,
  "subtotal": 135.2,
  "totalGst": 5,
  "total": 150.2,
  "paidAt": "2016-12-01T05:44:59.223Z",
  "paidBy": "bd7bd2fe-0588-46c7-acd7-1fbca468ec77",
  "isOutstanding": false,
  "products": [
    {
      "id": "5846b780-c4fa-40a3-b662-be5aa15c415c",
      "createdAt": "2016-12-01T05:44:59.223Z",
      "updatedAt": "2016-12-01T05:44:59.223Z",
      "deletedAt": "2016-12-01T05:44:59.223Z",
      "updatedById": "64a01c74-1dc7-4fa5-b20d-afe9da81b83b",
      "deletedById": "2202dc91-5aed-4825-86a8-a1bacd98e5bf",
      "externalId": {},
      "universalId": "96264694-0f2c-4ab0-86f1-911283ca2218",
      "supplierId": "8990a258-06b1-4eea-a00d-181e96545158",
      "categoryId": "8943e5ca-bb7e-4d9a-84a4-e13f71da6ad1",
      "description": {},
      "name": "1kg Sourdough",
      "SKU": "SRBR1243",
      "salesCode": "SRBR0001",
      "basePrice": "25.2727",
      "activatedAt": "2016-12-01T05:44:59.223Z",
      "sortOrder": 5,
      "image": {
        "secure_url": "https://res.cloudinary.com/ordermentum/image/upload/fake_file_name_goes_here.jpg"
      },
      "unit": "Loaves",
      "uom": "Cans",
      "weight": {}
    }
  ],
  "lineItems": [
    {
      "id": "4bd11a0e-86b3-46b8-a610-9ece5e4d3131",
      "createdAt": "2016-12-01T05:44:59.223Z",
      "updatedAt": "2016-12-01T05:44:59.223Z",
      "name": "1kg Sourdough",
      "SKU": "SRBR1243",
      "orderId": "5f6794ee-41f2-40fe-b6f3-ede4ebec49c3",
      "productId": "93335816-80c1-4d55-8da9-82e06b629ac3",
      "price": "60.00",
      "quantity": 1,
      "subtotal": "60.00",
      "taxable": true,
      "totalWeight": "20.23"
    }
  ],
  "lineCount": 14,
  "productCount": 43,
  "comment": {},
  "reference": "BREAD1234",
  "editable": false,
  "chargable": false,
  "chargedAt": "2016-12-01T05:44:59.223Z",
  "chargedBy": "904e2886-68dc-44ca-b68c-c7dae789528a",
  "cancelledAt": {},
  "cancelledBy": "646f0e60-9b70-41c1-9b61-8df49e8be450",
  "canMarkAsPaid": false,
  "createdAt": "2016-12-01T05:44:59.223Z",
  "placedOn": "2016-12-01T05:44:59.223Z",
  "createdBy": "cb8898d9-6072-4e2a-be8a-44409606322c",
  "chargedByUser": "Freddy Muggins",
  "deliveryDate": "2016-12-01T05:44:59.223Z",
  "updatedAt": "2016-12-01T05:44:59.223Z",
  "deletedAt": "2016-12-01T05:44:59.223Z",
  "updatedBy": "2e5bdba0-a650-4bb5-a2c1-5eb7a20d1f5d"
}
```

This endpoint retrieves a specific webhook.

### HTTP Request

`GET http://app.ordermentum.com/v1/webhooks/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the webhook to retrieve

## Update a specific webhook

```shell
curl "http://app.ordermentum.com/v1/webhooks/9AD783F1-4E1E-4396-A317-D528C99E177D"
  -X PUT
  -D '{"name": "Test Webhook" }'
  -H "Authorization: UNIQUE_TOKEN"
```

> The above command returns JSON structured the same a GET request

This endpoint updates a specific webhook

### HTTP Request

`PUT http://app.ordermentum.com/webhooks/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the webhook to update

## Delete a specific webhook

```shell
curl "http://app.ordermentum.com/v1/webhooks/9AD783F1-4E1E-4396-A317-D528C99E177D"
  -X DELETE
  -H "Authorization: UNIQUE_TOKEN"
```

> The above command returns JSON structured the same a GET request

This endpoint deletes a specific webhook

### HTTP Request

`DELETE http://app.ordermentum.com/v1/webhooks/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the webhook to delete
