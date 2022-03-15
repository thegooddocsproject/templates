
# GET Reference type

Method | syntax
----- | ----------
GET | base_url/endpoint/etc.

<!-- Delete this comment after you have replaced the method and syntax above. -->

## Description

<!-- Enter a short description. What is it for, and what can it do? -->

Parameters

Name | type | Req. | Description
---- | ----- | ----- | --------------------
Parameter_one | string | Y |  Meal Type. Either says "burgerMeal" or "salad"
Parameter_two | int float  | N | Timestamp for order 
Parameter_three | int  | Y | Cost 

<!-- Replace the two example rows and include rows for all your parameters. -->
<!-- If one of the parameters has a set of sub-parameters, create a table or bulleted list for that, but proceed with caution. If the API is complex, there might be an easier way to do your reference section than writing markup by hand. -->

## Examples
curl -X GET "http://URL/tableNo?id=99"
# Response
{
   "orderNum":123,
   
   "timestamp":
   "2020-01-21T07:44:45-05:00",
   "Item1":{
      
      "ItemOrdered":{
         "type":"burgerMeal",
         "Cost":10.99
      }
   },
   "Item2":{
   
     "ItemOrdered":{
        "type":"salad",
         "Cost":9.50
      }
   }
}


### Request

```HTTP
<!--  A copy-and-paste working request, if possible. Not one with values replaced by their names, such as "ID." -->

```

<!-- Follow with comments to explain what each part of the request is doing -->

### Response

```HTTP
<!--  An actual response returned by this endpoint for the request above.  -->

```

<!-- Write a comment explaining the response, if it would be helpful. For a response with a complicated schema, create a table like the one used above for the request.  -->
