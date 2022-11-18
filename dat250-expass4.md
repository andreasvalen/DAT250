# Excercise 

### Report

## Experiment 1

Everything went smooth with postman

## Experiment 2

It was a bit hard to see where the unit tests failed so i did one test at the time.
I encountered a with the "testNonExistingTodo" where it would try to read the entire response instead of the body.
I ended up just returning the "Todo with...found!" string instead of the spark response, and it worked.

https://github.com/andreasvalen/expass4/tree/master/dat250-sparkjava-counter/todos/src/main/java/no/hvl/dat250/rest/todos
