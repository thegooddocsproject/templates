# API reference overview

{Before using this template, read [the accompanying guide](api-reference-guide.md) to this template}.

## Introduction

The {product name} APIs are REST APIs that provides {xx features}.

## Base URL

The APIs referenced in this documentation use the following base URL:

```
https://api.example.com
```


## Authorization

All requests to the API must be authenticated and authorized before they can access or manage resources on the {environment or platform}.

The {product name} API uses the **{auth_type}** authorization type.

You can authenticate your requests by {using authentication type and method}.

For example:

```
<EXAMPLE>
```


API requests without valid authentication will fail with a status of {error code}.


## Versioning

{This section is optional.}

The {product name} APIs provide {x} versions of API endpoints...

## Pagination

{This section is optional.}

You can use {xx} to paginate the results returned by the {product name} APIs. If not specified, the default values are ...

## Rate limiting and throttling

{This section is optional.}

The {product name} APIs use a {xx} rate limiting strategy. The maximum number of requests allowed to access a {resource/endpoint/..} is {xx} requests per {time period}.

If the number of requests exceeds that limit, an HTTP `429 Too Many Request` error is returned.

## Status code

The {product name} APIs use standard HTTP response codes.

| Status code | Message           | Description   |
|-------------|-------------------|---------------|
| 200 `OK`    | Request succeeds. | {description} |
|             |                   |               |
|             |                   |               |

# {Resource name}

The {resource name} is used to {xxx}.

## Data model

| Attribute | Type | Required/Optional | Description | Notes |
|-----------|------|-------------------|-------------|-------|
|           |      |                   |             |       |
|           |      |                   |             |       |
|           |      |                   |             |       |

## Example

```
<EXAMPLE>
```

## Endpoints

Use the following endpoints to interact with the {resource name} entities.

| Method | Endpoint name                           | Description           |
|--------|-----------------------------------------|-----------------------|
| POST   | {[Endpoint name A](link_to_endpoint_a)} | Creates a {resource}. |
| GET    | {[Endpoint name B](link_to_endpoint_b)} | Returns a {resource}. |
|        |                                         |                       |


# {Endpoint name}

{Provide a one-line description of what the API does. Starts with a verb.}

## Endpoint

```bash
{METHOD} /{request_url}/{{path_parameter}}
```

## Description

This endpoint ...

{This paragraph is optional.} This endpoint has been deprecated. Use {the recommended endpoint} instead. For more information about how to migrate to {the recommended endpoint}, see [{the migration guide}](link).

{This paragraph is optional.} The maximum number of calls to this API endpoint is {xx} per minute. For more information about API rate limiting/throttling, see [{the topic}](example).


## Authorization

The {authorization method} is required for each API request.

(Optional) Calling this endpoint also requires the {xx} permission.


## Request schema

### Path parameters

{This section is optional.}

| Path parameter | Type   | Required/Optional | Description              | Notes |
|----------------|--------|-------------------|--------------------------|-----|
| {Id}           | string | Required          | Unique identifier of {}. |     |
| {name}         | string | Optional          | Name of {}.              |     |
|                |        |                   |                          |     |

### Query parameters

{This section is optional.} 

| Query parameter | Type | Required/Optional | Description | Notes |
|-----------------|------|-------------------|-------------|-------|
|                 |      |                   |             |       |


### Header parameters

{This section is optional.} 

| Header parameter | Type | Required/Optional | Description | Notes |
|------------------|------|-------------------|-------------|-------|
|                  |      |                   |             |       |

### Request body

{This section is optional.} 

| Field | Type | Required/Optional | Description | Notes |
|-------|------|-------------------|-------------|-------|
|       |      |                   |             |       |


## Request example

```
<EXAMPLE>

```

## Response schema

If the request succeeds, this endpoint returns {one of the following options:
* a {data} in the response body in the {content type} format.
* a 200 status code with no response body.
}

Otherwise, this endpoint returns {[xx errors](link_to_error_list)}.

## Response example

```
<EXAMPLE>
```
