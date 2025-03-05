# Examples

> [Index](../README.md) > [Account](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Account](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#account)
    type annotations stubs module [types-aiobotocore-account](https://pypi.org/project/types-aiobotocore-account/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[account]` package installed.

Write your `Account` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# AccountClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("account") as client:  # (1)
    result = await client.accept_primary_email_update()  # (2)
```

1. client: [AccountClient](./client.md)
2. result: [:material-code-braces: AcceptPrimaryEmailUpdateResponseTypeDef](./type_defs.md#acceptprimaryemailupdateresponsetypedef)



#### Paginator usage example

```python
# ListRegionsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("account") as client:  # (1)
    paginator = client.get_paginator("list_regions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AccountClient](./client.md)
2. paginator: [ListRegionsPaginator](./paginators.md#listregionspaginator)
3. item: [:material-code-braces: ListRegionsResponseTypeDef](./type_defs.md#listregionsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[account]`
or a standalone `types_aiobotocore_account` package, you have to explicitly specify
`client: AccountClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# AccountClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_account.client import AccountClient
from types_aiobotocore_account.type_defs import AcceptPrimaryEmailUpdateResponseTypeDef
from types_aiobotocore_account.type_defs import AcceptPrimaryEmailUpdateRequestTypeDef


session = Session()

client: AccountClient
async with session.client("account") as client:  # (1)
    kwargs: AcceptPrimaryEmailUpdateRequestTypeDef = {...}  # (2)
    result: AcceptPrimaryEmailUpdateResponseTypeDef = await client.accept_primary_email_update(**kwargs)  # (3)
```

1. client: [AccountClient](./client.md)
2. kwargs: [:material-code-braces: AcceptPrimaryEmailUpdateRequestTypeDef](./type_defs.md#acceptprimaryemailupdaterequesttypedef)
3. result: [:material-code-braces: AcceptPrimaryEmailUpdateResponseTypeDef](./type_defs.md#acceptprimaryemailupdateresponsetypedef)



#### Paginator usage example

```python
# ListRegionsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_account.client import AccountClient
from types_aiobotocore_account.paginator import ListRegionsPaginator
from types_aiobotocore_account.type_defs import ListRegionsResponseTypeDef


session = Session()

client: AccountClient
async with session.client("account") as client:  # (1)
    paginator: ListRegionsPaginator = client.get_paginator("list_regions")  # (2)
    async for item in paginator.paginate(...):
        item: ListRegionsResponseTypeDef
        print(item)  # (3)
```

1. client: [AccountClient](./client.md)
2. paginator: [ListRegionsPaginator](./paginators.md#listregionspaginator)
3. item: [:material-code-braces: ListRegionsResponseTypeDef](./type_defs.md#listregionsresponsetypedef)




