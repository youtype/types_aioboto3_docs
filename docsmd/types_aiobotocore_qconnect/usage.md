# Examples

> [Index](../README.md) > [QConnect](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [QConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect)
    type annotations stubs module [types-aiobotocore-qconnect](https://pypi.org/project/types-aiobotocore-qconnect/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[qconnect]` package installed.

Write your `QConnect` code as usual,
type checking and code completion should work out of the box.



```python
# QConnectClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("qconnect") as client:  # (1)
    result = await client.create_assistant()  # (2)
```

1. client: [QConnectClient](./client.md)
2. result: [:material-code-braces: CreateAssistantResponseTypeDef](./type_defs.md#createassistantresponsetypedef) 



```python
# ListAssistantAssociationsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("qconnect") as client:  # (1)
    paginator = client.get_paginator("list_assistant_associations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [ListAssistantAssociationsPaginator](./paginators.md#listassistantassociationspaginator)
3. item: [:material-code-braces: ListAssistantAssociationsResponseTypeDef](./type_defs.md#listassistantassociationsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[qconnect]`
or a standalone `types_aiobotocore_qconnect` package, you have to explicitly specify
`client: QConnectClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# QConnectClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_qconnect.client import QConnectClient
from types_aiobotocore_qconnect.type_defs import CreateAssistantResponseTypeDef
from types_aiobotocore_qconnect.type_defs import CreateAssistantRequestRequestTypeDef


session = Session()

client: QConnectClient
async with session.client("qconnect") as client:  # (1)
    kwargs: CreateAssistantRequestRequestTypeDef = {...}  # (2)
    result: CreateAssistantResponseTypeDef = await client.create_assistant(**kwargs)  # (3)
```

1. client: [QConnectClient](./client.md)
2. kwargs: [:material-code-braces: CreateAssistantRequestRequestTypeDef](./type_defs.md#createassistantrequestrequesttypedef) 
3. result: [:material-code-braces: CreateAssistantResponseTypeDef](./type_defs.md#createassistantresponsetypedef) 



```python
# ListAssistantAssociationsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_qconnect.client import QConnectClient
from types_aiobotocore_qconnect.paginator import ListAssistantAssociationsPaginator
from types_aiobotocore_qconnect.type_defs import ListAssistantAssociationsResponseTypeDef


session = Session()

client: QConnectClient
async with session.client("qconnect") as client:  # (1)
    paginator: ListAssistantAssociationsPaginator = client.get_paginator("list_assistant_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssistantAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [ListAssistantAssociationsPaginator](./paginators.md#listassistantassociationspaginator)
3. item: [:material-code-braces: ListAssistantAssociationsResponseTypeDef](./type_defs.md#listassistantassociationsresponsetypedef) 




