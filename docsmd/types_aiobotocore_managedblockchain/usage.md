# Examples

> [Index](../README.md) > [ManagedBlockchain](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ManagedBlockchain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#managedblockchain)
    type annotations stubs module [types-aiobotocore-managedblockchain](https://pypi.org/project/types-aiobotocore-managedblockchain/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[managedblockchain]` package installed.

Write your `ManagedBlockchain` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ManagedBlockchainClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("managedblockchain") as client:  # (1)
    result = await client.create_accessor()  # (2)
```

1. client: [ManagedBlockchainClient](./client.md)
2. result: [:material-code-braces: CreateAccessorOutputTypeDef](./type_defs.md#createaccessoroutputtypedef)



#### Paginator usage example

```python
# ListAccessorsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("managedblockchain") as client:  # (1)
    paginator = client.get_paginator("list_accessors")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ManagedBlockchainClient](./client.md)
2. paginator: [ListAccessorsPaginator](./paginators.md#listaccessorspaginator)
3. item: [:material-code-braces: ListAccessorsOutputTypeDef](./type_defs.md#listaccessorsoutputtypedef)




### Explicit type annotations

With `types-aioboto3-lite[managedblockchain]`
or a standalone `types_aiobotocore_managedblockchain` package, you have to explicitly specify
`client: ManagedBlockchainClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ManagedBlockchainClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_managedblockchain.client import ManagedBlockchainClient
from types_aiobotocore_managedblockchain.type_defs import CreateAccessorOutputTypeDef
from types_aiobotocore_managedblockchain.type_defs import CreateAccessorInputTypeDef


session = Session()

client: ManagedBlockchainClient
async with session.client("managedblockchain") as client:  # (1)
    kwargs: CreateAccessorInputTypeDef = {...}  # (2)
    result: CreateAccessorOutputTypeDef = await client.create_accessor(**kwargs)  # (3)
```

1. client: [ManagedBlockchainClient](./client.md)
2. kwargs: [:material-code-braces: CreateAccessorInputTypeDef](./type_defs.md#createaccessorinputtypedef)
3. result: [:material-code-braces: CreateAccessorOutputTypeDef](./type_defs.md#createaccessoroutputtypedef)



#### Paginator usage example

```python
# ListAccessorsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_managedblockchain.client import ManagedBlockchainClient
from types_aiobotocore_managedblockchain.paginator import ListAccessorsPaginator
from types_aiobotocore_managedblockchain.type_defs import ListAccessorsOutputTypeDef


session = Session()

client: ManagedBlockchainClient
async with session.client("managedblockchain") as client:  # (1)
    paginator: ListAccessorsPaginator = client.get_paginator("list_accessors")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccessorsOutputTypeDef
        print(item)  # (3)
```

1. client: [ManagedBlockchainClient](./client.md)
2. paginator: [ListAccessorsPaginator](./paginators.md#listaccessorspaginator)
3. item: [:material-code-braces: ListAccessorsOutputTypeDef](./type_defs.md#listaccessorsoutputtypedef)




