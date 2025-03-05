# Examples

> [Index](../README.md) > [TelcoNetworkBuilder](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [TelcoNetworkBuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#telconetworkbuilder)
    type annotations stubs module [types-aiobotocore-tnb](https://pypi.org/project/types-aiobotocore-tnb/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[tnb]` package installed.

Write your `TelcoNetworkBuilder` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# TelcoNetworkBuilderClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("tnb") as client:  # (1)
    result = await client.cancel_sol_network_operation()  # (2)
```

1. client: [TelcoNetworkBuilderClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# ListSolFunctionInstancesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("tnb") as client:  # (1)
    paginator = client.get_paginator("list_sol_function_instances")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [TelcoNetworkBuilderClient](./client.md)
2. paginator: [ListSolFunctionInstancesPaginator](./paginators.md#listsolfunctioninstancespaginator)
3. item: [:material-code-braces: ListSolFunctionInstancesOutputTypeDef](./type_defs.md#listsolfunctioninstancesoutputtypedef)




### Explicit type annotations

With `types-aioboto3-lite[tnb]`
or a standalone `types_aiobotocore_tnb` package, you have to explicitly specify
`client: TelcoNetworkBuilderClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# TelcoNetworkBuilderClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_tnb.client import TelcoNetworkBuilderClient
from types_aiobotocore_tnb.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_tnb.type_defs import CancelSolNetworkOperationInputTypeDef


session = Session()

client: TelcoNetworkBuilderClient
async with session.client("tnb") as client:  # (1)
    kwargs: CancelSolNetworkOperationInputTypeDef = {...}  # (2)
    result: EmptyResponseMetadataTypeDef = await client.cancel_sol_network_operation(**kwargs)  # (3)
```

1. client: [TelcoNetworkBuilderClient](./client.md)
2. kwargs: [:material-code-braces: CancelSolNetworkOperationInputTypeDef](./type_defs.md#cancelsolnetworkoperationinputtypedef)
3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# ListSolFunctionInstancesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_tnb.client import TelcoNetworkBuilderClient
from types_aiobotocore_tnb.paginator import ListSolFunctionInstancesPaginator
from types_aiobotocore_tnb.type_defs import ListSolFunctionInstancesOutputTypeDef


session = Session()

client: TelcoNetworkBuilderClient
async with session.client("tnb") as client:  # (1)
    paginator: ListSolFunctionInstancesPaginator = client.get_paginator("list_sol_function_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListSolFunctionInstancesOutputTypeDef
        print(item)  # (3)
```

1. client: [TelcoNetworkBuilderClient](./client.md)
2. paginator: [ListSolFunctionInstancesPaginator](./paginators.md#listsolfunctioninstancespaginator)
3. item: [:material-code-braces: ListSolFunctionInstancesOutputTypeDef](./type_defs.md#listsolfunctioninstancesoutputtypedef)




