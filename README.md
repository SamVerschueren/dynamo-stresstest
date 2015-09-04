# dynamo-stresstest

Library for easy DynamoDB stresstesting

## Idea

The idea is to create an easy to use library that can be used to stresstest a DynamoDB database. How much reads and writes can be done per second on a table with a certain provisioned throughput.

It should be possible for the user to set the size per record that is being inserted in the table and to choose a type per field and how long the value of the field could be. The size is very important because the reads and writes are determined by the size, for instance a 2 KB record will use 2 RCU instead of a 1 KB record that will only use 1 RCU.
