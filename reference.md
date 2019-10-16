**This template is still a work in progress.**

# Reference Section

## About the Reference Section

The reference section is the main event for you API documentation. New users will start with other documents to help them get going, but experienced users will refer more frequently to the reference section for the detailed information they need to make use of the API.
The reference section should contain a full listing of endpoints, methods, and parameters

## The General Contents

The reference section is generally a collection of short entries, arranged in alphabetical order.

### Reference Entries

Each reference listing should contain:
* The HTTP method, if applicable
* An example of the syntax
* A description of the endpoint in question (What is it for, and what can it do?)
* All the parameters for each endpoint (at a minimum: name, data type, description, comments)
* An example request
* An example response
* Response schema

### Special Reference Topics

* Authentication
* Error-handling. Make sure users can find an explanation for any error code they might receive.
* Throttling

## Best Practices for Reference Docs

Each detailed reference entry should contain all the information a user might need to know when using a parameter.

Include these:

Description of what the parameter does and when to use it
   * Data type
   * All the acceptable values, if there is a limited set of options
   * whether the parameter is required or optional

If more than one endpoint or parameter can get the job done, explain which one pertains to what situation. (Each probably exists for a specific reason, but the user needs to know.)

Each reference entry should include both a syntax and a working example. The example code should be followed by extensive comments that explain how it works.

## Examples

examples:
https://developers.google.com/gmail/api/v1/reference
