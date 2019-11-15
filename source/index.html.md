---
title: API Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - shell

toc_footers:
  - <a href='https://app.ordermentum.com/'>Login to Ordermentum</a>
  - <a href='https://github.com/lord/slate'>Powered by Slate</a>

includes:
  - orders
  - purchasers
  - invoices
  - products
  - webhooks
  - errors
  - filtering

search: true
---

# Introduction

Welcome to the Ordermentum API! You can use our API to access Ordermentum API endpoints.

You can view code examples in the dark area to the right.

# Getting Started


In this section, we will provide a quick guide to getting started with the Ordermentum API. We will walk through the process of obtaining an authorisation token, using it to authorise a request, and getting a list of orders.

The examples use the curl application to allow them to be run from the command-line wherever curl is installed.

# Sending Requests

If you are writing your own client or sending requests via the command line, you should always ensure that an appropriate User-Agent header is sent. For example, for a client called OrdermentumClient version 1.0, you might use a user agent of OrdermentumClient/1.0 as in the example snippet.

```shell
curl "https://api.ordermentum.com/v1/orders" \
  -H "Accept: application/json"
  -H "User-Agent: OrdermentumClient/1.0"
```

You must also send the Accept header to indicate what content type is desired. This should be application/json or a wildcard such as \*/\*.

# Authentication

> To authorize, use this code:

```shell
# With shell, you can just pass the correct header with each request
curl "https://app.ordermentum.com/v1/profile"
  -H "Authorization: Bearer UNIQUE_TOKEN"
```

> Make sure to replace `UNIQUE_TOKEN` with your personal API token

Ordermentum uses API tokens to allow access to the API.

Ordermentum expects for the API token to be included in all API requests to the server in a header that looks like the following:

`Authorization: Bearer UNIQUE_TOKEN`

<aside class="notice">
You must replace <code>UNIQUE_TOKEN</code> with your personal API token
</aside>


# Token

Ordermentum uses API tokens to allow access to the API. To get a token you need to successfully authenticate with the API.

```shell
curl -X POST "https://app.ordermentum.com/v1/auth" \
     -H "Content-Type: application/json" \
     --data '{"username":"user@example.com","password":"hunter2"}'
```
> The above requests returns

```json
{
  "userId": "d495042a-27cd-4ae9-9ec5-ffc91985d1f6",
  "token": "aaaaaaaaaa.bbbbbbbbbbb.cccccccccccc",
  "expiry": "2016-12-01T05:44:59.223Z"
}
```
