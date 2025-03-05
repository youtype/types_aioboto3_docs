# Examples

> [Index](../README.md) > [KafkaConnect](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [KafkaConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#kafkaconnect)
    type annotations stubs module [types-aiobotocore-kafkaconnect](https://pypi.org/project/types-aiobotocore-kafkaconnect/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[kafkaconnect]` package installed.

Write your `KafkaConnect` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# KafkaConnectClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("kafkaconnect") as client:  # (1)
    result = await client.create_connector()  # (2)
```

1. client: [KafkaConnectClient](./client.md)
2. result: [:material-code-braces: CreateConnectorResponseTypeDef](./type_defs.md#createconnectorresponsetypedef)



#### Paginator usage example

```python
# ListConnectorOperationsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("kafkaconnect") as client:  # (1)
    paginator = client.get_paginator("list_connector_operations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [KafkaConnectClient](./client.md)
2. paginator: [ListConnectorOperationsPaginator](./paginators.md#listconnectoroperationspaginator)
3. item: [:material-code-braces: ListConnectorOperationsResponseTypeDef](./type_defs.md#listconnectoroperationsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[kafkaconnect]`
or a standalone `types_aiobotocore_kafkaconnect` package, you have to explicitly specify
`client: KafkaConnectClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# KafkaConnectClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_kafkaconnect.client import KafkaConnectClient
from types_aiobotocore_kafkaconnect.type_defs import CreateConnectorResponseTypeDef
from types_aiobotocore_kafkaconnect.type_defs import CreateConnectorRequestTypeDef


session = Session()

client: KafkaConnectClient
async with session.client("kafkaconnect") as client:  # (1)
    kwargs: CreateConnectorRequestTypeDef = {...}  # (2)
    result: CreateConnectorResponseTypeDef = await client.create_connector(**kwargs)  # (3)
```

1. client: [KafkaConnectClient](./client.md)
2. kwargs: [:material-code-braces: CreateConnectorRequestTypeDef](./type_defs.md#createconnectorrequesttypedef)
3. result: [:material-code-braces: CreateConnectorResponseTypeDef](./type_defs.md#createconnectorresponsetypedef)



#### Paginator usage example

```python
# ListConnectorOperationsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_kafkaconnect.client import KafkaConnectClient
from types_aiobotocore_kafkaconnect.paginator import ListConnectorOperationsPaginator
from types_aiobotocore_kafkaconnect.type_defs import ListConnectorOperationsResponseTypeDef


session = Session()

client: KafkaConnectClient
async with session.client("kafkaconnect") as client:  # (1)
    paginator: ListConnectorOperationsPaginator = client.get_paginator("list_connector_operations")  # (2)
    async for item in paginator.paginate(...):
        item: ListConnectorOperationsResponseTypeDef
        print(item)  # (3)
```

1. client: [KafkaConnectClient](./client.md)
2. paginator: [ListConnectorOperationsPaginator](./paginators.md#listconnectoroperationspaginator)
3. item: [:material-code-braces: ListConnectorOperationsResponseTypeDef](./type_defs.md#listconnectoroperationsresponsetypedef)




