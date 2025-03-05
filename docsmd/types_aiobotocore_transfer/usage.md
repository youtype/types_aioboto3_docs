# Examples

> [Index](../README.md) > [Transfer](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Transfer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#transfer)
    type annotations stubs module [types-aiobotocore-transfer](https://pypi.org/project/types-aiobotocore-transfer/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[transfer]` package installed.

Write your `Transfer` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# TransferClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("transfer") as client:  # (1)
    result = await client.create_access()  # (2)
```

1. client: [TransferClient](./client.md)
2. result: [:material-code-braces: CreateAccessResponseTypeDef](./type_defs.md#createaccessresponsetypedef)



#### Paginator usage example

```python
# ListAccessesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("transfer") as client:  # (1)
    paginator = client.get_paginator("list_accesses")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [TransferClient](./client.md)
2. paginator: [ListAccessesPaginator](./paginators.md#listaccessespaginator)
3. item: [:material-code-braces: ListAccessesResponseTypeDef](./type_defs.md#listaccessesresponsetypedef)



#### Waiter usage example

```python
# ServerOfflineWaiter usage example

from aioboto3.session import Session


session = Session()

async with session.client("transfer") as client:  # (1)
    waiter = client.get_waiter("server_offline")  # (2)
    await waiter.wait(...)
```

1. client: [TransferClient](./client.md)
2. waiter: [ServerOfflineWaiter](./waiters.md#serverofflinewaiter)


### Explicit type annotations

With `types-aioboto3-lite[transfer]`
or a standalone `types_aiobotocore_transfer` package, you have to explicitly specify
`client: TransferClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# TransferClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_transfer.client import TransferClient
from types_aiobotocore_transfer.type_defs import CreateAccessResponseTypeDef
from types_aiobotocore_transfer.type_defs import CreateAccessRequestTypeDef


session = Session()

client: TransferClient
async with session.client("transfer") as client:  # (1)
    kwargs: CreateAccessRequestTypeDef = {...}  # (2)
    result: CreateAccessResponseTypeDef = await client.create_access(**kwargs)  # (3)
```

1. client: [TransferClient](./client.md)
2. kwargs: [:material-code-braces: CreateAccessRequestTypeDef](./type_defs.md#createaccessrequesttypedef)
3. result: [:material-code-braces: CreateAccessResponseTypeDef](./type_defs.md#createaccessresponsetypedef)



#### Paginator usage example

```python
# ListAccessesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_transfer.client import TransferClient
from types_aiobotocore_transfer.paginator import ListAccessesPaginator
from types_aiobotocore_transfer.type_defs import ListAccessesResponseTypeDef


session = Session()

client: TransferClient
async with session.client("transfer") as client:  # (1)
    paginator: ListAccessesPaginator = client.get_paginator("list_accesses")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccessesResponseTypeDef
        print(item)  # (3)
```

1. client: [TransferClient](./client.md)
2. paginator: [ListAccessesPaginator](./paginators.md#listaccessespaginator)
3. item: [:material-code-braces: ListAccessesResponseTypeDef](./type_defs.md#listaccessesresponsetypedef)



#### Waiter usage example

```python
# ServerOfflineWaiter usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_transfer.client import TransferClient
from types_aiobotocore_transfer.waiter import ServerOfflineWaiter


session = Session()

async with session.client("transfer") as client:  # (1)
    waiter = client.get_waiter("server_offline")  # (2)
    await waiter.wait(...)
```

1. client: [TransferClient](./client.md)
2. waiter: [ServerOfflineWaiter](./waiters.md#serverofflinewaiter)


