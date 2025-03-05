# Examples

> [Index](../README.md) > [OpenSearchService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [OpenSearchService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#opensearchservice)
    type annotations stubs module [types-aiobotocore-opensearch](https://pypi.org/project/types-aiobotocore-opensearch/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[opensearch]` package installed.

Write your `OpenSearchService` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# OpenSearchServiceClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("opensearch") as client:  # (1)
    result = await client.accept_inbound_connection()  # (2)
```

1. client: [OpenSearchServiceClient](./client.md)
2. result: [:material-code-braces: AcceptInboundConnectionResponseTypeDef](./type_defs.md#acceptinboundconnectionresponsetypedef)



#### Paginator usage example

```python
# ListApplicationsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("opensearch") as client:  # (1)
    paginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [OpenSearchServiceClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[opensearch]`
or a standalone `types_aiobotocore_opensearch` package, you have to explicitly specify
`client: OpenSearchServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# OpenSearchServiceClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_opensearch.client import OpenSearchServiceClient
from types_aiobotocore_opensearch.type_defs import AcceptInboundConnectionResponseTypeDef
from types_aiobotocore_opensearch.type_defs import AcceptInboundConnectionRequestTypeDef


session = Session()

client: OpenSearchServiceClient
async with session.client("opensearch") as client:  # (1)
    kwargs: AcceptInboundConnectionRequestTypeDef = {...}  # (2)
    result: AcceptInboundConnectionResponseTypeDef = await client.accept_inbound_connection(**kwargs)  # (3)
```

1. client: [OpenSearchServiceClient](./client.md)
2. kwargs: [:material-code-braces: AcceptInboundConnectionRequestTypeDef](./type_defs.md#acceptinboundconnectionrequesttypedef)
3. result: [:material-code-braces: AcceptInboundConnectionResponseTypeDef](./type_defs.md#acceptinboundconnectionresponsetypedef)



#### Paginator usage example

```python
# ListApplicationsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_opensearch.client import OpenSearchServiceClient
from types_aiobotocore_opensearch.paginator import ListApplicationsPaginator
from types_aiobotocore_opensearch.type_defs import ListApplicationsResponseTypeDef


session = Session()

client: OpenSearchServiceClient
async with session.client("opensearch") as client:  # (1)
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationsResponseTypeDef
        print(item)  # (3)
```

1. client: [OpenSearchServiceClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef)




