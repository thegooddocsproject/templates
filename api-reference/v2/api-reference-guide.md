# API References Guide

Read this document before you start working on the API references template.

- _Document version_: 0.0.1
- _Last updated_: May 19, 2022

## Overview

Assuming that your API documentation set includes references of many API endpoints that are organized into groups, this template includes three parts:

- The [API reference overview section](#about-the-api-reference-overview-section) provides reference information for the whole API documentation set. It describes product-wise API specifications, such as protocol, authorization method, versioning, status code, etc.
- The [API resource reference section](#about-the-api-resource-reference-section) provides reference information for a subset of API endpoints that are grouped around a resource type. It describes resource-wise API specifications, such as the data model of the resource.
- The [API endpoint reference section](#about-the-api-endpoint-reference-section)
 provides reference information for a specific API endpoint. It describes the specifications of an API endpoint, such as the method, URL, request, and response schema.

## Before writing the API references

- Familiarize yourself with the API protocol. If possible, try making some API calls in a testing environment.
- Interact with your API developers to learn about the APIs that you are documenting. Understand the data models and the logical connections between the API endpoints.
- Discuss the logic of grouping the API endpoints. Although grouping the endpoints by resource type is a common practice, as used in this template, it is also possible to group them by use case or other characteristics that better suit the user's needs.
- Conduct some user research about how the audience of your documentation would use the APIs. Identify the programming languages that your audience would most likely adopt to interact with your APIs.
- Explore the possibility of auto-generating the API references.

## About the API reference overview section

### About the "Introduction" section

Use this section to provide a high-level overview of your API set, including the main features, communication protocol, content types, organization, etc.

### About the "Base URL" section

Base URL is a common segment to which the API endpoint paths are appended. Defining the base URL in this section reduces the effort to duplicate the segment in each endpoint reference.

The base URL may differ for different groups of users or in different environments. If multiple base URLs are available, list them in this section and clearly describe the conditions of using each of them.


### About the "Authorization" section

Use this section to specify the authentication and authorization requirements of using the APIs, including the authorization type, request schema, possible error codes, and examples.

Tips:

- This section should only describe the technical specifications of the API authorization, such as parameters and token expiration. Details of how to authenticate should be documented in a separate how-to guide and be referred to as a link here.
- Provide an example of the authorization request or command. You can use random strings to replace the actual secrets.
- If there is more than one authorization type applicable to your APIs, describe and specify the use case of each. If one of the options is preferred, highlight it.
- If different permission levels apply to different API endpoints, document the requirements in the reference for that endpoint.


### About the "Versioning" section

This section is optional. If applicable, use this section to describe the versioning, compatibility, and lifecycle policies of your API set. If migration guides are available, provide the links here.


### About the "Pagination" section

This section is optional. If applicable, use this section to describe the options and default values for dividing long API responses into pages.


### About the "Rate limiting and throttling" section

This section is optional. If applicable, use this section to describe the global rate limiting settings and quota of your APIs. If different quota applies to different endpoints, also add this section in the reference for endpoints.


### About the "Status code" section

Tips:

- For REST APIs, HTTP status codes are used. If you are writing references for other protocols, adjust the table columns.
- In the `Description` column, describe the causes of that error, and provide related information or links about how to deal with the error.

### Additional sections

If other specifications are applicable to the whole API set, such as data conventions, request retry logic, logging, monitoring, and so on, define your own sections at the end of this document.


## About the API resource reference section

The template assumes that the API endpoints are grouped by the resource type that they are interacting with.

**Title**

Substitute the document title `{Resource Name}` with the actual name.

**Short description**

Provide a one-line definition of the resource in the opening section and explain how and when your users should use it.

### About the "Data model" section

Use this section to describe each attribute of the resource entity in the table. Use the `Notes` column to provide additional information such as whether the attribute has default values, validation restrictions, and whether it is a non-editable field that cannot be updated with POST requests. If a cell is empty, fill in “N/A” or “/”.

### About the "Example" section

Provide a concrete example of the data entity with valid values. Fill in as many optional attributes as possible.

Use fenced code blocks (a pair of three backticks ` ``` `) to make your code distinctive from other text blocks.

Many Markdown processors also support syntax highlighting, which adds color to keywords. Indicate the language mode of your example after the opening backticks to take advantage of this feature. For example: ` ```json `. The displayed color schema depends on your processor and the rendering configurations.

### About the "Endpoints" section

List the endpoints that can interact with this resource type in the table:

- Capitalize the method names.
- Adopt a consistent naming convention for the APIs. In most cases, the naming convention used in the documentation is consistent with the one in the source code.
- Add a link to each of the endpoint names that directs users to the corresponding endpoint reference.
- For endpoints that are deprecated but still in use, add a note in the “Description” column. Consider using the strikethrough format (a pair of two tildes ~~) to indicate the deprecation status.


## About the API endpoint reference section

**Title**

Substitute the document title `{Endpoint Name}` with the actual name.

Tips:

- Typically the name of an API endpoint consists of the operation type and the resource type. For example, an API endpoint that creates a User resource can be named as `Create user`.
- As in the API resource reference, the naming convention should be consistent throughout your API documentation.
- Use the singular form of the resource name unless the endpoint is designed exclusively for a bulk operation, such as `List users`.

**Short description**

Provide a one-line description of what the API does. Starts with a verb. For example:

- For "get" operations: `Returns a {resource}.`
- For "list" operations: `Returns a list of {resources}.`
- For "create" operations: `Creates a {resource}.` or `Inserts a {resource}.`
- For "update" operations: `Updates a {resource}.`
- For "delete" operations: `Removes a {resource}.` 

Ensure that the description here is consistent with that listed in the resource reference.

### About the "Endpoint" section

Use this section to define the API endpoint.

Tips:

- Use fenced code blocks (a pair of three backticks ` ``` `) to make your code distinctive from other text blocks. 
- Replace {METHOD} with the actual request method and capitalize all letters. For example, `POST`.
- In the {request_url} segment, start with a slash character `/` and only provide the URL path (the segment after the hostname). The base URL can be omitted if you already document it in the API overview. For example, `/v2/users`.
- If the {request_url} contains path variables, use a placeholder to indicate the variable name. The format of placeholders should be consistent throughout the documentation set and conform to your organization’s guidelines. As an option, you can use snake case characters in curly brace `{}`, delimited by underscores. For example, `{user_id}`.
- Optionally use a different color to make the path parameters easily identifiable.
- Do not add slash characters `/` at the end.

### About the "Description" section

Use this section to provide more information on what the endpoint does, the purpose, and use cases of this API endpoint.

Optionally add notes about the API versioning information, API limit, deprecation status, and whether a replacement is available. If they are not applicable, remove the paragraphs.

### About the "Authorization" section

Provide a link to the common `Authorization` section in the API reference overview.

If calling the endpoint requires additional user roles or permissions, document them in this section.

### About the "Request schema" section

Use this section to define the specifications of the endpoint.

Each of the sub-sections is optional and should be adopted according to the actual endpoint definition:

- **Path parameters**: parameters defined within the path of the endpoint, denoted by placeholders.
- **Query parameters**: appended to the end of the request URL, after a question mark `?`. Parameters and their assigned values are connected by an equal sign `=`. Multiple query parameters are delimited by an and sign `&`.
- **Header parameters**: often the same across endpoints in an API set. Include this section only when specific header parameters are required for this endpoint.
- **Request body**: only applicable for requests using methods that permit a payload, such as POST, PUT, and PATCH. Include a link to the description of the resource type if applicable.

If no parameters or request body can be sent in the request, specify "None" in this section.

Tips:

- In each of the tables, keep the parameter name the same as what is presented in the endpoint section above.
- In the `Required/Optional` column, specify "Required" or "Optional" to avoid ambiguity.
- In the `Type` column, if the data type has detailed definitions in another place, provide the link. 
- In the `Description` column, start the description with a noun and omit the articles (the/a/an). No need to write "defines/specifies".
- Use the `Notes` column to provide additional information such as default values, minimum/maximum values, usage restrictions, and valid enum values.
- Do not leave cells empty in the table. If there is no content, fill in with “N/A” or “/”.


### About the "Request example" section

Use this section to provide an example that is complete and correct. The request should include the base URL, endpoint, headers, parameters, and request body. It should show as many parameter configurations as possible. Preferable, the example could be copy-pasted directly into your user's environment and return the expected result.

Tips:

- If you have several parameters for different use cases, especially when then parameters can not be used together, consider providing multiple request examples.
- The recommended format for your example is `cURL` request. Depending on the business needs, you can add request samples in multiple programming languages, which can be generated by external tools. Do user research in advance to determine what languages should be adopted. Meanwhile, you should also consider the additional maintenance effort when you add more examples.
- Match the sample request and parameters to the exact response the user would receive with those same parameters.
- Use fenced code blocks (a pair of three backticks ` ``` `) to make your code distinctive from other text blocks.

### About the "Response schema" section

Use this section to describe the content type and data model that are returned in the response, in both successful and failed cases:

- For successful requests, provide the content format.
- For failed requests, provide the possible error code and the link to the error description.

### About the "Response example" section

Use this section to provide an example of the response body if any, or clearly state that “the response body is empty”.
