# DynamoDB

NoSQL database.

Where documents (objects) are organised as follows:
Tables = Collections of objects
Items = Row = Object

## Streams

Releases a "data stream" of events that can be listened to.

## Transaction

Guaranteed CUD operations across multiple tables. i.e. keep duplicated data in sync.

## DAX

DynamoDB accelerator via a seamless cache.

5 min TTL default.

## Global Tables

i.e. Cross region replication

## Costing

### Manual 

Read Capacity Units (RCUs) and Write Capacity Units (WCUs) used for costing.

### Automatic

OnDemand Capacity can be specified to scales as needed.
