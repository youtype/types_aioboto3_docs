# Examples

> [Index](../README.md) > [Braket](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Braket](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#braket)
    type annotations stubs module [types-aiobotocore-braket](https://pypi.org/project/types-aiobotocore-braket/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[braket]` package installed.

Write your `Braket` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# BraketClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("braket") as client:  # (1)
    result = await client.cancel_job()  # (2)
```

1. client: [BraketClient](./client.md)
2. result: [:material-code-braces: CancelJobResponseTypeDef](./type_defs.md#canceljobresponsetypedef)



#### Paginator usage example

```python
# SearchDevicesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("braket") as client:  # (1)
    paginator = client.get_paginator("search_devices")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [BraketClient](./client.md)
2. paginator: [SearchDevicesPaginator](./paginators.md#searchdevicespaginator)
3. item: [:material-code-braces: SearchDevicesResponseTypeDef](./type_defs.md#searchdevicesresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[braket]`
or a standalone `types_aiobotocore_braket` package, you have to explicitly specify
`client: BraketClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# BraketClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_braket.client import BraketClient
from types_aiobotocore_braket.type_defs import CancelJobResponseTypeDef
from types_aiobotocore_braket.type_defs import CancelJobRequestTypeDef


session = Session()

client: BraketClient
async with session.client("braket") as client:  # (1)
    kwargs: CancelJobRequestTypeDef = {...}  # (2)
    result: CancelJobResponseTypeDef = await client.cancel_job(**kwargs)  # (3)
```

1. client: [BraketClient](./client.md)
2. kwargs: [:material-code-braces: CancelJobRequestTypeDef](./type_defs.md#canceljobrequesttypedef)
3. result: [:material-code-braces: CancelJobResponseTypeDef](./type_defs.md#canceljobresponsetypedef)



#### Paginator usage example

```python
# SearchDevicesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_braket.client import BraketClient
from types_aiobotocore_braket.paginator import SearchDevicesPaginator
from types_aiobotocore_braket.type_defs import SearchDevicesResponseTypeDef


session = Session()

client: BraketClient
async with session.client("braket") as client:  # (1)
    paginator: SearchDevicesPaginator = client.get_paginator("search_devices")  # (2)
    async for item in paginator.paginate(...):
        item: SearchDevicesResponseTypeDef
        print(item)  # (3)
```

1. client: [BraketClient](./client.md)
2. paginator: [SearchDevicesPaginator](./paginators.md#searchdevicespaginator)
3. item: [:material-code-braces: SearchDevicesResponseTypeDef](./type_defs.md#searchdevicesresponsetypedef)




