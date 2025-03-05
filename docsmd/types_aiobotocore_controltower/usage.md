# Examples

> [Index](../README.md) > [ControlTower](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ControlTower](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#controltower)
    type annotations stubs module [types-aiobotocore-controltower](https://pypi.org/project/types-aiobotocore-controltower/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[controltower]` package installed.

Write your `ControlTower` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ControlTowerClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("controltower") as client:  # (1)
    result = await client.create_landing_zone()  # (2)
```

1. client: [ControlTowerClient](./client.md)
2. result: [:material-code-braces: CreateLandingZoneOutputTypeDef](./type_defs.md#createlandingzoneoutputtypedef)



#### Paginator usage example

```python
# ListBaselinesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("controltower") as client:  # (1)
    paginator = client.get_paginator("list_baselines")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ControlTowerClient](./client.md)
2. paginator: [ListBaselinesPaginator](./paginators.md#listbaselinespaginator)
3. item: [:material-code-braces: ListBaselinesOutputTypeDef](./type_defs.md#listbaselinesoutputtypedef)




### Explicit type annotations

With `types-aioboto3-lite[controltower]`
or a standalone `types_aiobotocore_controltower` package, you have to explicitly specify
`client: ControlTowerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ControlTowerClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_controltower.client import ControlTowerClient
from types_aiobotocore_controltower.type_defs import CreateLandingZoneOutputTypeDef
from types_aiobotocore_controltower.type_defs import CreateLandingZoneInputTypeDef


session = Session()

client: ControlTowerClient
async with session.client("controltower") as client:  # (1)
    kwargs: CreateLandingZoneInputTypeDef = {...}  # (2)
    result: CreateLandingZoneOutputTypeDef = await client.create_landing_zone(**kwargs)  # (3)
```

1. client: [ControlTowerClient](./client.md)
2. kwargs: [:material-code-braces: CreateLandingZoneInputTypeDef](./type_defs.md#createlandingzoneinputtypedef)
3. result: [:material-code-braces: CreateLandingZoneOutputTypeDef](./type_defs.md#createlandingzoneoutputtypedef)



#### Paginator usage example

```python
# ListBaselinesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_controltower.client import ControlTowerClient
from types_aiobotocore_controltower.paginator import ListBaselinesPaginator
from types_aiobotocore_controltower.type_defs import ListBaselinesOutputTypeDef


session = Session()

client: ControlTowerClient
async with session.client("controltower") as client:  # (1)
    paginator: ListBaselinesPaginator = client.get_paginator("list_baselines")  # (2)
    async for item in paginator.paginate(...):
        item: ListBaselinesOutputTypeDef
        print(item)  # (3)
```

1. client: [ControlTowerClient](./client.md)
2. paginator: [ListBaselinesPaginator](./paginators.md#listbaselinespaginator)
3. item: [:material-code-braces: ListBaselinesOutputTypeDef](./type_defs.md#listbaselinesoutputtypedef)




