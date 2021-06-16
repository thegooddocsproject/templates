# Get/TableNO 

property | description
-------- | -----------
tableNo  | this specifies that it is table number x that ordered the meal. in this case the GET for the POC will be to Get the bill

curl -X GET "http://URL/tableNo?id=99"



## Description

 GET - used to get commands from the server. In this case the GET for the POC will be to GET the bill. this specifies that table number 99 ordered 5 items, the main meal, sides and drink.  This is the call which is sent when the server wants to get the bill the GET request includes the table number.  The order number is included in the response. Take out orders are table 99. When this is printed, the customer can pay the bill. 


Parameters

propert name | data type    | choices               | default      | mandatory    |definition
------------ | ------------ | --------------------- | ------------ |------------ | ------------ 
pattytype    | string       | beef                  |  beef        |  yes        | the type of patty the customer can get on their burger
                              checken 
                              veggie
                            
pattyQty     | 1             |  1 or 2               |  1          | yes         | this specifies the quantity of patty the customer can get on thier  burger meal 
pattyWeightG | 300           |   300,350             |  300        |  yes        | this specifies the weight of the patty the customer want to get 
pattyCook    |    mr         |           |           |             | 
bunType      | string        | white bread           | white bread | yes         | this specifies  the type of the bun the customer  can get on their burger
                           
condiment1   | string        | ketchup               | ketchup     | yes         | this epecifies the   type of condiment the customer can get on their  burger
                               secretSauce 
                               mayonnise
topping1   | string       | lettuce,tomato,cucumber, | tomato      |  no         |  this specifies  the type of topping the customer can get on their burger
                            cucumber, pickled onion
                             cheddar cheese


sides     | string           | soup  |               |    no       |  no         | this specifies the type of sides the customer can get on their burger

type      |    string         |          |           |             |                     
size      |   string         | small    |            |  no         |              |  this spesifies  the size of burger the customer can get on their burger
drink     |  string          |         |             |             |    |                
type      |    string          | coke   |            |   no        |  no          |  this spesifies the type of drink the customer  can get 
size      |    string        | large  |              |    no       |   yes        |  this spesifies the  size of drink the customer can get 
ice       |    string        |  yes   |              |    no       |   no         |                

property | Data type | Req. | Description
---- | ----- | ----- | --------------------
orderNum | string | Y |  this specifies the order number that customers regenerates everday 
timestamp | string  | N | this is a unique identification. that specifies the time and date the order is recieved 
item1 | int |   | this specifies the number of order in the whole meal 
itemOrdered |string |   | this specifies the item ordered , the type"buger meal" and cost 18.00 nis
item2 |   |   |  this specifies the number of order in the whole meal
itemOrdered |   |   | this specifies the item ordered, the type "soup" and cost 12.00 nis
item3 |   |   | this specifies the number of  the oorder
itemOrdered |   |   |  this specifies the item ordered, the type" french fries" and cost 8.00 nis 
item4 |   |   |  this specifies the number of the order 
itemOrdeded |   |    |this specifies the item ordered, the type" crispy onion rings" and the cost 10.00 
item5 |   |    | this specifies the number of the order 
itemOrdered |   |    | this specifoes the item orderedm the type " coke" and the cost 8.00 nis 


## Examples

### Request

```HTTP


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

