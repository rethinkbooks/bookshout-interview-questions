# bookshout-interview-questions

## 1. BookShout API Request / Parse
Using Ruby, create a program that from the command line takes 2 arguments, book id and a tax rate. And return the total price of the book with tax.

(For API access I would suggest looking at the RestClient library here: https://github.com/rest-client/rest-client . Although there are other options, feel free to use what you think is best.)

Example:
ruby bookshout_price_fetcher.rb 44990 .0825
Would return:
Deception - $7.57

You can use our API here:
https://www.bookshout.com/api/books/44990.json
Where 44990 is the book id.

Here are some example book ids: 44990, 44991,44992, etc.

## 2. CSV Parse
Using Ruby and given a CSV file with 2 columns and n rows and NO HEADER rows, where the first column is a book title, and the second column is a price. Write a program that takes the path to the csv and return the following information:

Most expensive book,
Least expensive book,
Average book price

Example data
Book A, 1.00
Book B, 2.00
Book C, 3,00

ruby csv_price_parser.rb ../path_to_file.csv
would return:
Most Expensive: Book C
Least Expensive: Book A
Average Book Price: 2.00

I would suggest using this documentation: http://ruby-doc.org/stdlib-1.9.2/libdoc/csv/rdoc/CSV.html

## 3. Stack Implementation
Using Java create a stack data structure using an array implementation. This video should help you, https://www.youtube.com/watch?v=sFVxsglODoo
The structure should follow standard stack ADT operations: push, pop, top, isEmpty. 

Bonus points if you can make the stack dynamically sized. Set the initial size of the stack to 2, and add 10 elements and test to confirm your dynamic resizing is working.

I expect that using your code I can do the following:
init_size = 2
stack = new Stack(init_size)
stack.push(5) -> void return
stack.push(3) -> void return
stack.push(2) -> void return
stack.top() -> returns 2
stack.pop() -> returns 2
stack.top -> returns 3
stack.pop() -> returns 3
stack.top() -> returns 5
stack.isEmpty() -> returns true
