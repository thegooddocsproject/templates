# Endpoint name

Method | syntax
----- | ----------
<!-- POST |POST/lunch/meal/burgerMeal. -->

<!-- Delete this comment after you have replaced the method and syntax above. -->

## Description

<!-- post- used to get the command  meal order from the customer.in this case the Post for the POC will be the burger meal that needs to be documented. -->

<!-- Enter a short description. What is it for, and what can it do? -->

Parameters

Name | type | Req. | Description
---- | ----- | ----- | --------------------

<!--orderNum | string | Y |  this specifies the order number that customers regenerates everday -->
<!--timestamp | string  | N | this is a unique identification. that specifies the time and date the order is recieved -->
<!--item1 | int |this specifies the number of order in the whole meal -->
<!--itemOrdered |string | this specifies the item ordered , the type"buger meal" and cost 18.00 nis.-->
<!--item2 |this specifies the number of order in the whole meal-->
<!--itemOrdered |this specifies the item ordered, the type "soup" and cost 12.00 nis-->
<!--item3 |this specifies the number of  the oorder-->
<!--itemOrdered | this specifies the item ordered, the type" french fries" and cost 8.00 nis -->
<!--item4 |this specifies the number of the order -->
<!--itemOrdeded |this specifies the item ordered, the type" crispy onion rings" and the cost 10.00 -->
<!--item5 | this specifies the number of the order -->
<!--itemOrdered | this specifoes the item orderedm the type " coke" and the cost 8.00 nis -->

Parameter_one | string | Y |  Stores the customer name
Parameter_two | int  | N | Stores a postal code, like the U.S. ZIP code.

<!-- Replace the two example rows and include rows for all your parameters. -->
<!-- If one of the parameters has a set of sub-parameters, create a table or bulleted list for that, but proceed with caution. If the API is complex, there might be an easier way to do your reference section than writing markup by hand. -->

## Examples

### Request

```HTTP

curl -H "Content-Type: application/json" -X POST -d'{
   "mealType":"lunch",
   "mealCat":{
  	"main":"burgerMeal",
  	"burger":{
     	"pattyType":"”beef”",
     	"pattyQty":1,
     	"pattyWeightG":300,
     	"pattyCook":"MR",
     	"bunType":"whiteBread",
     	"condiment1":"ketchup",
     	"condiment2":"secretSauce",
      "condiment3":"mayonnaise",
     	"topping1":"lettuce",
      "topping2':"cucumber",
      "topping3":"tomato",
      "topping4":"pickledOnion",
     	"topping5":"cheddarCheese",


   },
  	"sides":{
     	"side1":{
        	"type":"soup",
        	"size":"small"
     	},
     	"side2":{
        	"type":"frenshFries",
        	"size":"small"
     	},
      side3":{
           "type":"crispyOnionRings",
           "size":"large"
  	},
  	"drink":{
     	"type":"Coke",
     	"size":"large",
     	"ice":"yes"
  	}
   }
}'
http://URL/


<!--  A copy-and-paste working request, if possible. Not one with values replaced by their names, such as "ID." -->

```

<!-- For the purpose of the POC, only the burger meal needs to be documented. The burger JSON object is included in the POST request which is sent to the kitchen. When an OK           response is received, the order is printed in the kitchen so the cook can start cooking. -->


<!-- Follow with comments to explain what each part of the request is doing -->

### Response

```HTTP

<!-- 200 OK -->

<!--  An actual response returned by this endpoint for the request above.  -->

```
 <!--  When a correct order is placed, the server replies to the app with an acknowledgement. This is not displayed to the user.    -->
