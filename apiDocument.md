//page 1
# list of category
>> http://localhost:9700/category
>> https://myapi-heroku.herokuapp.com/category

# list of items
>> http://localhost:9700/list
>> https://myapi-heroku.herokuapp.com/list

//page 2
# list of products
>> http://localhost:9700/product
>> https://myapi-heroku.herokuapp.com/product

# list of products wrt category
>> http://localhost:9700/product?category_id=1
>> https://myapi-heroku.herokuapp.com/product?category_id=1

# list of items wrt category
>> http://localhost:9700/list?category_id=3
>> https://myapi-heroku.herokuapp.com/list?category_id=3

# list of items wrt products
>> http://localhost:9700/list?product_Id=6
>> https://myapi-heroku.herokuapp.com/list?product_Id=6

//page 3
# details of a particular item
>> http://localhost:9700/details/49
>> https://myapi-heroku.herokuapp.com/details/49

//page 4
# details of items selected
(POST)> localhost:9700/listItem
(body)> [21,22,23]

# place order
(POST)> localhost:9700/placeOrder
(body)> {
   {
   "name": "Emma",
   "email": "emma@gmail.com",
   "phone": 5474784832,
   "cost": 450,
   "listitem":[47,34,85,67]
}

//page 5
#  view orders
>> localhost:9700/viewOrder

# Get Order on basis of emailId
>> localhost:9700/viewOrder?email=shamika@gmail.com

# delete order
>> localhost:9700/deleteOrders

# Update Order
(PUT)> localhost:9700/updateOrder/6258285a46b9ae51328b8459
(body)> {
    "cost": 390,
    "phone": 9826457679
}