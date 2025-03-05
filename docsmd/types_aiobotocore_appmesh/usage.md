# Examples

> [Index](../README.md) > [AppMesh](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AppMesh](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#appmesh)
    type annotations stubs module [types-aiobotocore-appmesh](https://pypi.org/project/types-aiobotocore-appmesh/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[appmesh]` package installed.

Write your `AppMesh` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# AppMeshClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("appmesh") as client:  # (1)
    result = await client.create_gateway_route()  # (2)
```

1. client: [AppMeshClient](./client.md)
2. result: [:material-code-braces: CreateGatewayRouteOutputTypeDef](./type_defs.md#creategatewayrouteoutputtypedef)



#### Paginator usage example

```python
# ListGatewayRoutesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("appmesh") as client:  # (1)
    paginator = client.get_paginator("list_gateway_routes")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AppMeshClient](./client.md)
2. paginator: [ListGatewayRoutesPaginator](./paginators.md#listgatewayroutespaginator)
3. item: [:material-code-braces: ListGatewayRoutesOutputTypeDef](./type_defs.md#listgatewayroutesoutputtypedef)




### Explicit type annotations

With `types-aioboto3-lite[appmesh]`
or a standalone `types_aiobotocore_appmesh` package, you have to explicitly specify
`client: AppMeshClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# AppMeshClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_appmesh.client import AppMeshClient
from types_aiobotocore_appmesh.type_defs import CreateGatewayRouteOutputTypeDef
from types_aiobotocore_appmesh.type_defs import CreateGatewayRouteInputTypeDef


session = Session()

client: AppMeshClient
async with session.client("appmesh") as client:  # (1)
    kwargs: CreateGatewayRouteInputTypeDef = {...}  # (2)
    result: CreateGatewayRouteOutputTypeDef = await client.create_gateway_route(**kwargs)  # (3)
```

1. client: [AppMeshClient](./client.md)
2. kwargs: [:material-code-braces: CreateGatewayRouteInputTypeDef](./type_defs.md#creategatewayrouteinputtypedef)
3. result: [:material-code-braces: CreateGatewayRouteOutputTypeDef](./type_defs.md#creategatewayrouteoutputtypedef)



#### Paginator usage example

```python
# ListGatewayRoutesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_appmesh.client import AppMeshClient
from types_aiobotocore_appmesh.paginator import ListGatewayRoutesPaginator
from types_aiobotocore_appmesh.type_defs import ListGatewayRoutesOutputTypeDef


session = Session()

client: AppMeshClient
async with session.client("appmesh") as client:  # (1)
    paginator: ListGatewayRoutesPaginator = client.get_paginator("list_gateway_routes")  # (2)
    async for item in paginator.paginate(...):
        item: ListGatewayRoutesOutputTypeDef
        print(item)  # (3)
```

1. client: [AppMeshClient](./client.md)
2. paginator: [ListGatewayRoutesPaginator](./paginators.md#listgatewayroutespaginator)
3. item: [:material-code-braces: ListGatewayRoutesOutputTypeDef](./type_defs.md#listgatewayroutesoutputtypedef)




