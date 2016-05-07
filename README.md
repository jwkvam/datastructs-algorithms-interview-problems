# Query Batching

At Verdigris, we have database that stores data about our customers' electrical
circuits.

## Problem

Included in the repository is a Python API for querying the data stored on our
database. Currently, the client is written to perform each query individually.
Since this data query must be made over a network, the amount of time to
establish a connection and perform the query is the bottleneck.

Write a batched version of the client such that we can minimize the network
overhead.

To query for data, run:

```bash
python batched_queries.py
```
