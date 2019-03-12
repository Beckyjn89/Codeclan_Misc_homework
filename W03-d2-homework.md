Your task this evening is to read over the completed end\_code for tomorrow's lesson, understand it as much as possible, and answer the following questions.

1) What is the relationship between customers and pizza\_orders?
a one-to-many relationship between customers and pizza\_orders - customer id links the two tables


2) At what point is the id of a `PizzaOrder` created?
when it is saved into the database (line 27 of pizza_order.rb)

3) At what point do we assign a value to the `@id` instance variables of our objects?
when sqlrunner is run in the function save (line 31 of pizza_order.rb)


4) Name 2 things that the `Customer`'s `@id` property is used for.
used in the pizza order to identify the customer, can be used by pizza_order.customer to show the customer details of a specific order

5) Why might it be important to check if `options['id']` is `nil` in our `initialize` method before assigning `@id` the value of `options[‘id’].to_i?`
because nil can't be turned into an integer and it would throw up an error

6) What are the responsibilities of `SqlRunner`?
SqlRunner does the preparing, executing and closing of the sql bit

7) How does `SqlRunner` improve the quality of our code?
It makes the code neater and more DRY. 
