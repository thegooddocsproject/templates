# Endpoint name

property | description
-------- | -----------
tableNo  | this specifies that it is table number x that ordered the meal

curl -X GET "http://URL/tableNo?id=99"



## Description

 GET - used to get commands from the server. In this case the GET for the POC will be to GET the bill. this specifies that table number 99 ordered 5 items, the main meal, sides and drink.  This is the call which is sent when the server wants to get the bill the GET request includes the table number.  The order number is included in the response. Take out orders are table 99. When this is printed, the customer can pay the bill. 


Parameters

Name | type | Req. | Description
---- | ----- | ----- | --------------------
orderNum | string | Y |  this specifies the order number that customers regenerates everday 
timestamp | string  | N | this is a unique identification. that specifies the time and date the order is recieved 
item1 | int |this specifies the number of order in the whole meal 
itemOrdered |string | this specifies the item ordered , the type"buger meal" and cost 18.00 nis
item2 |   |this specifies the number of order in the whole meal
itemOrdered |   |this specifies the item ordered, the type "soup" and cost 12.00 nis
item3 |   |this specifies the number of  the oorder
itemOrdered |   | this specifies the item ordered, the type" french fries" and cost 8.00 nis 
item4 |   |this specifies the number of the order 
itemOrdeded |   |this specifies the item ordered, the type" crispy onion rings" and the cost 10.00 
item5 |   | this specifies the number of the order 
itemOrdered |   | this specifoes the item orderedm the type " coke" and the cost 8.00 nis 


## Examples

### Request

```HTTP
 curl -X GET "http://URL/tableNo?id=99  



curl -X GET "http://URL/tableNo?id=99"
# response
{
   "orderNum":123,
   "timestamp":"2020-01-21T07:44:45-05:00",
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



<!-- This is the call which is sent when the server wants to get the bill the GET request includes the table number.  The order number is included in the response. Take out orders are table 99. When this is printed, the customer can pay the bill.  -->

### Response

```

