# Examples

> [Index](../README.md) > [DataZone](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DataZone](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#datazone)
    type annotations stubs module [types-aiobotocore-datazone](https://pypi.org/project/types-aiobotocore-datazone/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[datazone]` package installed.

Write your `DataZone` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# DataZoneClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("datazone") as client:  # (1)
    result = await client.accept_predictions()  # (2)
```

1. client: [DataZoneClient](./client.md)
2. result: [:material-code-braces: AcceptPredictionsOutputTypeDef](./type_defs.md#acceptpredictionsoutputtypedef)



#### Paginator usage example

```python
# ListAssetFiltersPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("datazone") as client:  # (1)
    paginator = client.get_paginator("list_asset_filters")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. paginator: [ListAssetFiltersPaginator](./paginators.md#listassetfilterspaginator)
3. item: [:material-code-braces: ListAssetFiltersOutputTypeDef](./type_defs.md#listassetfiltersoutputtypedef)




### Explicit type annotations

With `types-aioboto3-lite[datazone]`
or a standalone `types_aiobotocore_datazone` package, you have to explicitly specify
`client: DataZoneClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# DataZoneClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_datazone.client import DataZoneClient
from types_aiobotocore_datazone.type_defs import AcceptPredictionsOutputTypeDef
from types_aiobotocore_datazone.type_defs import AcceptPredictionsInputTypeDef


session = Session()

client: DataZoneClient
async with session.client("datazone") as client:  # (1)
    kwargs: AcceptPredictionsInputTypeDef = {...}  # (2)
    result: AcceptPredictionsOutputTypeDef = await client.accept_predictions(**kwargs)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. kwargs: [:material-code-braces: AcceptPredictionsInputTypeDef](./type_defs.md#acceptpredictionsinputtypedef)
3. result: [:material-code-braces: AcceptPredictionsOutputTypeDef](./type_defs.md#acceptpredictionsoutputtypedef)



#### Paginator usage example

```python
# ListAssetFiltersPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_datazone.client import DataZoneClient
from types_aiobotocore_datazone.paginator import ListAssetFiltersPaginator
from types_aiobotocore_datazone.type_defs import ListAssetFiltersOutputTypeDef


session = Session()

client: DataZoneClient
async with session.client("datazone") as client:  # (1)
    paginator: ListAssetFiltersPaginator = client.get_paginator("list_asset_filters")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssetFiltersOutputTypeDef
        print(item)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. paginator: [ListAssetFiltersPaginator](./paginators.md#listassetfilterspaginator)
3. item: [:material-code-braces: ListAssetFiltersOutputTypeDef](./type_defs.md#listassetfiltersoutputtypedef)




