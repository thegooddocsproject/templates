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
