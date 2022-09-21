# API Reference

{Before using this template, read [the accompanying guide](api-reference-guide.md) to this template}.


## Overview

This reference describes the Application Program Interfaces (APIs) that help you {access | customize | program} {product}'s {features | functionality}.

### Base URL

The APIs referenced in this documentation use the following base URL:

```
https://api.example.com
```


### Authorization

All requests to the API must be authenticated and authorized before they can access or manage resources on the {environment | platform}.

The {product} API uses the `{auth_type}` authorization type.

You can authenticate your requests by using {authentication type and method}.

For example:

```
{EXAMPLE}
```


API requests without valid authentication will fail with a status of `{error_code}`.


### Versioning

{This section is optional.}

The {product} APIs provide multiple versions of API endpoints.

{Commentary about the versions supported.}

### Pagination

{This section is optional.}

Due to the potential very large result sets from API calls, responses {are | can be} returned as shorter pages.

Pagination can be customized using {pagination settings}. If not specified, the default values are {values}.

### Rate limiting and throttling

{This section is optional.}

The {product} APIs use a {strategy_name} rate limiting strategy. The maximum number of requests allowed to access a {resource | endpoint |..} is {number} requests per {time period}.

If the number of requests exceeds that limit, an HTTP `429 Too Many Request` error is returned.

### HTTP status code

The {product} APIs use the following standard HTTP response codes:

| Status code | Message           | Description   |
|-------------|-------------------|---------------|
| `200 OK`    | Request succeeds. | {description} |
|             |                   |               |
|             |                   |               |

### Errors

{This section is optional.}

The {product} APIs use the following error types:

| Error                                   | Description      |
|-----------------------------------------|------------------|
| [{ExampleErrorType}](#exampleerrortype) | {Failure in ...} |
|                                         |                  |
|                                         |                  |

#### ExampleErrorType

| Field          | Type     | Description                                      |
|----------------|----------|--------------------------------------------------|
| {errorType}    | {enum}   | {Predefined error codes. Possible enum values are x, y, ..., and z.} |
| {errorMessage} | {string} | {Additional information about why the error occurs.} |


## {Resource name}

The {resource name} is used to {functionality}.

### Data model

| Attribute | Type   | Required? | Description                  |
|-----------|--------|-----------|------------------------------|
| {id}      | string | Required  | {Unique identifier of user.} |
| {name}    | string | Optional  | {Name of user}.              |
|           |        |           |                              |


### Example

```
{EXAMPLE}
```

### Endpoints

Use the following endpoints to interact with the {resource name} entities.

| Method | Endpoint name                            | Description             |
|--------|------------------------------------------|-------------------------|
| POST   | {[Endpoint name A](#link_to_endpoint_a)} | Creates a {resource}.   |
| GET    | {[Endpoint name B](#link_to_endpoint_b)} | Retrieves a {resource}. |
|        |                                          |                         |


## {Endpoint name}

{Provide a one-line description of what the API does. Starts with a verb. For example, "retrieves a user".}

### Endpoint

```bash
{METHOD} /{request-url}/{{path-parameter}}
```

### Description

This endpoint ...

{This paragraph is optional.} This endpoint has been deprecated. Use {the recommended endpoint} instead. For more information about how to migrate to {the recommended endpoint}, see [{the migration guide}](#link).

{This paragraph is optional.} The maximum number of calls to this API endpoint is {number} per minute. For more information about API rate limiting/throttling, see [{the topic}](#example).


### Authorization

The [{authorization method}](#authorization) is required for each API request.

{This paragraph is optional.} Calling this endpoint also requires the {permission_name} permission.


### Request schema

#### Path parameters

{This section is optional.}

| Path parameter | Type   | Required? | Description                  |
|----------------|--------|-----------|------------------------------|
| {id}           | string | Required  | {Unique identifier of user.} |
|                |        |           |                              |

#### Query parameters

{This section is optional.}

| Query parameter | Type | Required? | Description                             |
|-----------------|------|-----------|-----------------------------------------|
| {pageSize}      | int  | Optional  | {The number of items to be returned in a single request. The default value is 20.} |
|                 |      |           |                                         |

#### Header parameters

{This section is optional.}

| Header parameter | Type   | Required? | Description                          |
|------------------|--------|-----------|--------------------------------------|
| {Content-Type}   | string | Required  | {Media type of the resource. Must be object}. |
|                  |        |           |                                      |

#### Request body

{This section is optional.}

| Field  | Type   | Required? | Description                      |
|--------|--------|-----------|----------------------------------|
| {id}   | string | Required  | {Unique identifier of the user.} |
| {name} | string | Optional  | {Name of the user.}              |

### Request example

```
{EXAMPLE}

```

### Response schema

| Status code | Schema                                              | Description |
|-------------|-----------------------------------------------------|----------|
| `2xx`         | [{ExampleDataType}](#data-model)   | {Describe the result where the request succeeds.} |
| `4xx`         | [{ExampleErrorType}](#exampleerrortype) | {Describe the result where the request fails with the specified error code.} |

### Response example

```
{EXAMPLE}

```
