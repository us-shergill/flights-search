# flights-search

We can use a json schema modeller to capture the attributes for the data from the flight search.
I used the online json schema tool to create a data model for the flight search . We can use 
avro schema format for the json . 

The json that is captured during the flight search can be saved as is to a no sql store like 
dynamo db in AWS . Since the flight search is write heavy and millions of customers
searching for flights at the same time a database that scales well for writes is ideal
for performance . For json validations there are multiple open source libraries like
pydantic that can be use .

We should not just collect the data. Dig deep and monitor the dynamic behavior of customers 
customers. Identify behavioral outliers, patterns, and associated contexts. Sending 
emails based on customer behavior etc .