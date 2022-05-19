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