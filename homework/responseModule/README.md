# Write a Module for API Response Objects

Write a module for a set of common response objects to send to any requesting client.

Context:
We are writing an api. We need to send back common responses to all calling clients. We want to wrap our response information in a response object depending on the type of response. For example, the client sends in invalid parameters, we should make a message indicating that invalid parameters were sent in and then add that to the InvalidParamsErrorResponse data property.

The structure should be:

BaseResponse
* SuccessResponse
** ListResponse
** CreatedResponse
** DeletedResponse
* ErrorResponse
** InvalidParamsErrorResponse
** UnauthorizedErrorResponse

ResponseFactory
* should give you the appropriate Response Object


Each response has these common properties:
timestamp: {date} (a timestamp of when the response was made)
type: {string} (the type of response example: ListResponse)
data: {object|array of objects} (an object if not ListResponse or array if ListResponse)

You should demonstrate strong knowledge of 

* factory pattern
* Object Oriented Programming



