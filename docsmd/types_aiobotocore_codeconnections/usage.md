# Examples

> [Index](../README.md) > [CodeConnections](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CodeConnections](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections.html#codeconnections)
    type annotations stubs module [types-aiobotocore-codeconnections](https://pypi.org/project/types-aiobotocore-codeconnections/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[codeconnections]` package installed.

Write your `CodeConnections` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# CodeConnectionsClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("codeconnections") as client:  # (1)
    result = await client.create_connection()  # (2)
```

1. client: [CodeConnectionsClient](./client.md)
2. result: [:material-code-braces: CreateConnectionOutputTypeDef](./type_defs.md#createconnectionoutputtypedef)






### Explicit type annotations

With `types-aioboto3-lite[codeconnections]`
or a standalone `types_aiobotocore_codeconnections` package, you have to explicitly specify
`client: CodeConnectionsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# CodeConnectionsClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_codeconnections.client import CodeConnectionsClient
from types_aiobotocore_codeconnections.type_defs import CreateConnectionOutputTypeDef
from types_aiobotocore_codeconnections.type_defs import CreateConnectionInputTypeDef


session = Session()

client: CodeConnectionsClient
async with session.client("codeconnections") as client:  # (1)
    kwargs: CreateConnectionInputTypeDef = {...}  # (2)
    result: CreateConnectionOutputTypeDef = await client.create_connection(**kwargs)  # (3)
```

1. client: [CodeConnectionsClient](./client.md)
2. kwargs: [:material-code-braces: CreateConnectionInputTypeDef](./type_defs.md#createconnectioninputtypedef)
3. result: [:material-code-braces: CreateConnectionOutputTypeDef](./type_defs.md#createconnectionoutputtypedef)






