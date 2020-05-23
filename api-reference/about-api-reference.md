# The API reference entry

## About the reference section

The reference section is generally a collection of short entries, arranged in alphabetical order. This template addresses the individual reference entry that you create for a single endpoint. 

The reference section is important for API documentation. New users will start with other documents to help them get going, but experienced users will refer more frequently to the reference section for the detailed information they need to make use of the API.

The reference section should contain a full listing of endpoints, methods, and parameters

## The general contents

### Reference entries

Each reference listing should ideally contain:

* A general description of the endpoint in question (What is it for, and what can it do?)
* The HTTP method, if applicable
* An example of the syntax
* All the parameters for the endpoint (And for each parameter, see the requirements below)
* An example request
* An example response
* Response schema

## Best practices for reference docs

Each detailed reference entry should contain all the information a user might need to know when using the feature.

For parameters, include these:

   * name (the actual parameter that users will pass)
   * Description of what the parameter does and when to use it
   * Data type
   * All the acceptable values, if there is a limited set of options
   * whether the parameter is required or optional

Differentiate the endpoint you are documenting from other similar endpoints. If more than one endpoint or parameter can get the job done, explain which one pertains to what situation. (Each probably exists for a specific reason, but the user needs to know.)

Each reference entry should include both a syntax and a working example. The example code should be followed by extensive comments that explain how it works.

## Examples

examples:
[API reference of various resource types](https://developers.google.com/gmail/api/v1/reference)
