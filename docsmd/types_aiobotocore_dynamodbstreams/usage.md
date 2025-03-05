# Examples

> [Index](../README.md) > [DynamoDBStreams](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DynamoDBStreams](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#dynamodbstreams)
    type annotations stubs module [types-aiobotocore-dynamodbstreams](https://pypi.org/project/types-aiobotocore-dynamodbstreams/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[dynamodbstreams]` package installed.

Write your `DynamoDBStreams` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# DynamoDBStreamsClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("dynamodbstreams") as client:  # (1)
    result = await client.describe_stream()  # (2)
```

1. client: [DynamoDBStreamsClient](./client.md)
2. result: [:material-code-braces: DescribeStreamOutputTypeDef](./type_defs.md#describestreamoutputtypedef)






### Explicit type annotations

With `types-aioboto3-lite[dynamodbstreams]`
or a standalone `types_aiobotocore_dynamodbstreams` package, you have to explicitly specify
`client: DynamoDBStreamsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# DynamoDBStreamsClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_dynamodbstreams.client import DynamoDBStreamsClient
from types_aiobotocore_dynamodbstreams.type_defs import DescribeStreamOutputTypeDef
from types_aiobotocore_dynamodbstreams.type_defs import DescribeStreamInputTypeDef


session = Session()

client: DynamoDBStreamsClient
async with session.client("dynamodbstreams") as client:  # (1)
    kwargs: DescribeStreamInputTypeDef = {...}  # (2)
    result: DescribeStreamOutputTypeDef = await client.describe_stream(**kwargs)  # (3)
```

1. client: [DynamoDBStreamsClient](./client.md)
2. kwargs: [:material-code-braces: DescribeStreamInputTypeDef](./type_defs.md#describestreaminputtypedef)
3. result: [:material-code-braces: DescribeStreamOutputTypeDef](./type_defs.md#describestreamoutputtypedef)






