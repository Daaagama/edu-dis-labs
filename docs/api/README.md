---
title: RESTfull service API v0.1
language_tabs:
  - http: HTTP
language_clients:
  - http: ""
toc_footers:
  - <a
    href="https://boldak.github.io/dis-edu/swagger/12.api.html#openapi-swagger">See
    also Educational Materials</a>
includes: []
search: true
highlight_theme: darkula
headingLevel: 2

---

<!-- Generator: Widdershins v4.0.1 -->

<h1 id="restfull-service-api">RESTfull service API v0.1</h1>

> Scroll down for code samples, example requests and responses. Select a language for code samples from the tabs above or the mobile navigation menu.

API for my project `Developing RESTful services on Node` 

Base URLs:

* <a href="http://localhost:8000">http://localhost:8000</a>

Email: <a href="mailto:abilokorenko@gmail.com">Artem Bilokorenko</a> Web: <a href="https://gvbilokorenko.github.io/edu-dis-labs/">Artem Bilokorenko</a> 
License: <a href="https://gvbilokorenko.github.io/edu-dis-labs/license.html">ECL 2.0</a>

<h1 id="restfull-service-api-crud">CRUD</h1>

## get__catalog

> Code samples

```http
GET http://localhost:8000/catalog HTTP/1.1
Host: localhost:8000
Accept: application/json

```

`GET /catalog`

*Get all catalog*

Returns data from catalog in JSON

> Example responses

> 200 Response

```json
[
  {
    "id": 1,
    "name": "First",
    "description": "Very cool!",
    "price": 11700
  },
  {
    "id": 2,
    "name": "Second",
    "description": "Very cool!",
    "price": 11700
  }
]
```

<h3 id="get__catalog-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Successful response|Inline|

<h3 id="get__catalog-responseschema">Response Schema</h3>

<aside class="success">
This operation does not require authentication
</aside>

## get__catalog_{id}

> Code samples

```http
GET http://localhost:8000/catalog/{id} HTTP/1.1
Host: localhost:8000
Accept: application/json

```

`GET /catalog/{id}`

*Get item with id*

Returns data aabout specif item with id from catalog in JSON

<h3 id="get__catalog_{id}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer|true|Numeric ID of the item in the catalog|

> Example responses

> 200 Response

```json
{
  "id": 1,
  "name": "First",
  "description": "Very cool!",
  "price": 11700
}
```

<h3 id="get__catalog_{id}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Successful response|Inline|

<h3 id="get__catalog_{id}-responseschema">Response Schema</h3>

<aside class="success">
This operation does not require authentication
</aside>

## post__catalog_post

> Code samples

```http
POST http://localhost:8000/catalog/post HTTP/1.1
Host: localhost:8000
Content-Type: application/json
Accept: text/plain; charset=utf-8

```

`POST /catalog/post`

*Get all catalog*

Returns string

> Body parameter

```json
{}
```

<h3 id="post__catalog_post-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|object|true|Optional description in *Markdown*|

> Example responses

> 200 Response

```
"Successfuly sended data"
```

<h3 id="post__catalog_post-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Successful response|string|

<aside class="success">
This operation does not require authentication
</aside>

