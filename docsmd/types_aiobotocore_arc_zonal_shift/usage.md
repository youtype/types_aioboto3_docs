# Examples

> [Index](../README.md) > [ARCZonalShift](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ARCZonalShift](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#arczonalshift)
    type annotations stubs module [types-aiobotocore-arc-zonal-shift](https://pypi.org/project/types-aiobotocore-arc-zonal-shift/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[arc-zonal-shift]` package installed.

Write your `ARCZonalShift` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ARCZonalShiftClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("arc-zonal-shift") as client:  # (1)
    result = await client.cancel_zonal_shift()  # (2)
```

1. client: [ARCZonalShiftClient](./client.md)
2. result: [:material-code-braces: ZonalShiftTypeDef](./type_defs.md#zonalshifttypedef)



#### Paginator usage example

```python
# ListAutoshiftsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("arc-zonal-shift") as client:  # (1)
    paginator = client.get_paginator("list_autoshifts")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ARCZonalShiftClient](./client.md)
2. paginator: [ListAutoshiftsPaginator](./paginators.md#listautoshiftspaginator)
3. item: [:material-code-braces: ListAutoshiftsResponseTypeDef](./type_defs.md#listautoshiftsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[arc-zonal-shift]`
or a standalone `types_aiobotocore_arc_zonal_shift` package, you have to explicitly specify
`client: ARCZonalShiftClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ARCZonalShiftClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_arc_zonal_shift.client import ARCZonalShiftClient
from types_aiobotocore_arc_zonal_shift.type_defs import ZonalShiftTypeDef
from types_aiobotocore_arc_zonal_shift.type_defs import CancelZonalShiftRequestTypeDef


session = Session()

client: ARCZonalShiftClient
async with session.client("arc-zonal-shift") as client:  # (1)
    kwargs: CancelZonalShiftRequestTypeDef = {...}  # (2)
    result: ZonalShiftTypeDef = await client.cancel_zonal_shift(**kwargs)  # (3)
```

1. client: [ARCZonalShiftClient](./client.md)
2. kwargs: [:material-code-braces: CancelZonalShiftRequestTypeDef](./type_defs.md#cancelzonalshiftrequesttypedef)
3. result: [:material-code-braces: ZonalShiftTypeDef](./type_defs.md#zonalshifttypedef)



#### Paginator usage example

```python
# ListAutoshiftsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_arc_zonal_shift.client import ARCZonalShiftClient
from types_aiobotocore_arc_zonal_shift.paginator import ListAutoshiftsPaginator
from types_aiobotocore_arc_zonal_shift.type_defs import ListAutoshiftsResponseTypeDef


session = Session()

client: ARCZonalShiftClient
async with session.client("arc-zonal-shift") as client:  # (1)
    paginator: ListAutoshiftsPaginator = client.get_paginator("list_autoshifts")  # (2)
    async for item in paginator.paginate(...):
        item: ListAutoshiftsResponseTypeDef
        print(item)  # (3)
```

1. client: [ARCZonalShiftClient](./client.md)
2. paginator: [ListAutoshiftsPaginator](./paginators.md#listautoshiftspaginator)
3. item: [:material-code-braces: ListAutoshiftsResponseTypeDef](./type_defs.md#listautoshiftsresponsetypedef)




