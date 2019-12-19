# Filtering

Most endpoints allow you to filter the results by dates.

All timestamps are all in ISO 8601 format.

```shell
curl "http://app.ordermentum.com/v1/orders?createdAt[gte]=2019-11-15T01:16:15.139Z"
  -X GET
  -H "Authorization: UNIQUE_TOKEN"
```

### Fields

| Parameter | Description                 |
| --------- | --------------------------- |
| createdAt | When the record was created |
| updatedAt | When the record was updated |


### Parameters

| Parameter | Description              |
| --------- | ------------------------ |
| gte       | Greater than or equal to |
| lte       | Less than or equal to    |
| lt        | Less than                |
| gt        | Greater than             |

