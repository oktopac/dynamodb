# dynamodb

a simple dockerfile for running dynamodb locally

to run, run the following command

```
docker run -d -p 127.0.0.1:8000:8000 dynamodb
```

Then, connect to the local instance in your dynamodb client

```python
dbresource = boto3.resource('dynamodb', endpoint_url='http://localhost:8000')

# or

dbclient = boto3.client('dynamodb', endpoint_url='http://localhost:8000')
```
