# Purchasers (Customers)

## Get All Purchasers

```shell
curl "https://api.ordermentum.com/v1/purchasers?supplierId=a5cad00b-0c85-4d95-ab3f-9fb1933dbeed"
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
    "self": "https://app.ordermentum.com/v1/purchasers?supplierId=a5cad00b-0c85-4d95-ab3f-9fb1933dbeed&pageNo=3",
    "first": "https://app.ordermentum.com/v1/purchasers?supplierId=bd4b8236-1649-49a5-aa6e-2d0f0e9407ea&pageNo=1",
    "prev": "https://app.ordermentum.com/v1/purchasers?supplierId=44c2ae51-b2eb-4f86-b021-fc7d181f5b65&pageNo=2",
    "next": "https://app.ordermentum.com/v1/purchasers?supplierId=561b48a5-f292-4f5c-abfe-3d7ff70ee91b&pageNo=4",
    "last": "https://app.ordermentum.com/v1/purchasers?supplierId=5331fea9-52e3-427d-bae8-57f1b7c7edd8&pageNo=9"
  },
  "data": [
    {
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
    }
  ]
}
```

This endpoint retrieves all purchasers

### HTTP Request

`GET http://app.ordermentum.com/v1/purchasers`

### Query Parameters

| Parameter  | Default | Description                                 |
| ---------- | ------- | ------------------------------------------- |
| pageNo     | 1       | Page number                                 |
| pageSize   | 25      | Number of purchasers in the response        |
| supplierId | null    | The supplier to retreive the purchasers for |
| createdAt  | null    | when the order was created                  |
| updatedAt  | null    | when the order was last updated             |


## Get a Specific Purchaser

```shell
curl "http://app.ordermentum.com/v1/purchasers/69B34C71-3D61-4D40-92DE-BD7954D26BD2"
  -H "Authorization: Bearer UNIQUE_TOKEN"
```

> The above command returns JSON structured like this:

```json
{
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
}
```

### HTTP Request

`GET http://app.ordermentum.com/v1/purchasers/<ID>`

### URL Parameters

| Parameter | Description                         |
| --------- | ----------------------------------- |
| ID        | The ID of the purchaser to retrieve |
