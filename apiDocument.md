//page 1
# list of category
>> http://localhost:9700/category

# list of items
>> http://localhost:9700/list

//page 2
# list of products
>> http://localhost:9700/product

# list of products wrt category
>> http://localhost:9700/product?category_id=1

# list of items wrt category
>> http://localhost:9700/list?category_id=3

# list of items wrt products
>> http://localhost:9700/list?product_Id=6

//page 3
# details of a particular item
>> http://localhost:9700/details/49

//page 4
# details of items selected
(POST)> localhost:9700/listItem
(body)> [21,22,23]

# place order
(POST)> localhost:9700/placeOrder
(body)> {
    "name": "Onion",
    "qty":1,
    "cost": 20
}

//page 5
#  view orders
>> localhost:9700/viewOrder

# delete order
>> localhost:9700/deleteOrders

# Update Order
(PUT)> localhost:9700/updateOrder/6256bafda3523cbf538d22bb
(body)> {
 "cost": 26,
 "qty": 2
}