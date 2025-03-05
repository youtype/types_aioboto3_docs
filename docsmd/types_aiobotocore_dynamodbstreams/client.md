# DynamoDBStreamsClient

> [Index](../README.md) > [DynamoDBStreams](./README.md) > DynamoDBStreamsClient

!!! note ""

    Auto-generated documentation for [DynamoDBStreams](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#dynamodbstreams)
    type annotations stubs module [types-aiobotocore-dynamodbstreams](https://pypi.org/project/types-aiobotocore-dynamodbstreams/).

## DynamoDBStreamsClient

Type annotations and code completion for `#!python session.client("dynamodbstreams")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams.Client)

```python
# DynamoDBStreamsClient usage example

from aioboto3.session import Session
from types_aiobotocore_dynamodbstreams.client import DynamoDBStreamsClient

session = Session()
async with session.client("dynamodbstreams") as client:
    client: DynamoDBStreamsClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("dynamodbstreams").exceptions` structure.

```python
# DynamoDBStreamsClient.exceptions usage example

async with session.client("dynamodbstreams") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.ExpiredIteratorException,
        client.exceptions.InternalServerError,
        client.exceptions.LimitExceededException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.TrimmedDataAccessException,
    ) as e:
        print(e)
```

```python
# DynamoDBStreamsClient.exceptions type checking example

from types_aiobotocore_dynamodbstreams.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("dynamodbstreams").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("dynamodbstreams").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams.Client)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### describe\_stream

Returns information about a stream, including the current status of the stream,
its Amazon Resource Name (ARN), the composition of its shards, and its
corresponding DynamoDB table.

Type annotations and code completion for `#!python session.client("dynamodbstreams").describe_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams.Client)

```python
# describe_stream method definition

await def describe_stream(
    self,
    *,
    StreamArn: str,
    Limit: int = ...,
    ExclusiveStartShardId: str = ...,
) -> DescribeStreamOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeStreamOutputTypeDef](./type_defs.md#describestreamoutputtypedef)


```python
# describe_stream method usage example with argument unpacking

kwargs: DescribeStreamInputTypeDef = {  # (1)
    "StreamArn": ...,
}

parent.describe_stream(**kwargs)
```

1. See [:material-code-braces: DescribeStreamInputTypeDef](./type_defs.md#describestreaminputtypedef)

### get\_records

Retrieves the stream records from a given shard.

Type annotations and code completion for `#!python session.client("dynamodbstreams").get_records` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams.Client)

```python
# get_records method definition

await def get_records(
    self,
    *,
    ShardIterator: str,
    Limit: int = ...,
) -> GetRecordsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRecordsOutputTypeDef](./type_defs.md#getrecordsoutputtypedef)


```python
# get_records method usage example with argument unpacking

kwargs: GetRecordsInputTypeDef = {  # (1)
    "ShardIterator": ...,
}

parent.get_records(**kwargs)
```

1. See [:material-code-braces: GetRecordsInputTypeDef](./type_defs.md#getrecordsinputtypedef)

### get\_shard\_iterator

Returns a shard iterator.

Type annotations and code completion for `#!python session.client("dynamodbstreams").get_shard_iterator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams.Client)

```python
# get_shard_iterator method definition

await def get_shard_iterator(
    self,
    *,
    StreamArn: str,
    ShardId: str,
    ShardIteratorType: ShardIteratorTypeType,  # (1)
    SequenceNumber: str = ...,
) -> GetShardIteratorOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ShardIteratorTypeType](./literals.md#sharditeratortypetype)
2. See [:material-code-braces: GetShardIteratorOutputTypeDef](./type_defs.md#getsharditeratoroutputtypedef)


```python
# get_shard_iterator method usage example with argument unpacking

kwargs: GetShardIteratorInputTypeDef = {  # (1)
    "StreamArn": ...,
    "ShardId": ...,
    "ShardIteratorType": ...,
}

parent.get_shard_iterator(**kwargs)
```

1. See [:material-code-braces: GetShardIteratorInputTypeDef](./type_defs.md#getsharditeratorinputtypedef)

### list\_streams

Returns an array of stream ARNs associated with the current account and
endpoint.

Type annotations and code completion for `#!python session.client("dynamodbstreams").list_streams` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams.Client)

```python
# list_streams method definition

await def list_streams(
    self,
    *,
    TableName: str = ...,
    Limit: int = ...,
    ExclusiveStartStreamArn: str = ...,
) -> ListStreamsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStreamsOutputTypeDef](./type_defs.md#liststreamsoutputtypedef)


```python
# list_streams method usage example with argument unpacking

kwargs: ListStreamsInputTypeDef = {  # (1)
    "TableName": ...,
}

parent.list_streams(**kwargs)
```

1. See [:material-code-braces: ListStreamsInputTypeDef](./type_defs.md#liststreamsinputtypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("dynamodbstreams").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("dynamodbstreams").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Type[BaseException] | None,
    exc_val: BaseException | None,
    exc_tb: types.TracebackType | None,
) -> None:
    ...
```





