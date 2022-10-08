# Excercise 3

### Report

- Installation went smooth

Verified binary:
![db screenshot](https://github.com/andreasvalen/DAT250/blob/main/resources/imgs/VerifiedBinary.PNG?raw=true)

## Experiment 1

Create:
![db screenshot](https://github.com/andreasvalen/DAT250/blob/main/resources/imgs/MongoDBCreate.PNG?raw=true)

Read:
![db screenshot](https://github.com/andreasvalen/DAT250/blob/main/resources/imgs/MongoDBRead.PNG?raw=true)

Update:
![db screenshot](https://github.com/andreasvalen/DAT250/blob/main/resources/imgs/MongoDBUpdate.PNG?raw=true)

Delete:
![db screenshot](https://github.com/andreasvalen/DAT250/blob/main/resources/imgs/MapReduceNotWorking.PNG?raw=true)

## Experminet 2

I could not find a workaround for map-reduce being deprecated.
I tried to downgrade to an older version, but I was unable to get it to work:
![db screenshot](https://github.com/andreasvalen/DAT250/blob/main/resources/imgs/MapReduceNotWorking.PNG?raw=true)

I ended up doing the aggregation excercise instead.
The "additional operation" is also done with aggreagation and merge (had to go back again to the newer version to get merge to work).
The operation makes a new collection of the best customers. The new documents have a "biggest_order" field and a "big_orders" field which
stores the number of times the customer has made an order for more than 50 price units.

Best customers:
![db screenshot](https://github.com/andreasvalen/DAT250/blob/main/resources/imgs/AdditionalOperation.PNG?raw=true)

- Getting map-reduce to run remains unsolved
