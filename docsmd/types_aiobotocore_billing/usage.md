# Examples

> [Index](../README.md) > [Billing](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Billing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing.html#billing)
    type annotations stubs module [types-aiobotocore-billing](https://pypi.org/project/types-aiobotocore-billing/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[billing]` package installed.

Write your `Billing` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# BillingClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("billing") as client:  # (1)
    result = await client.create_billing_view()  # (2)
```

1. client: [BillingClient](./client.md)
2. result: [:material-code-braces: CreateBillingViewResponseTypeDef](./type_defs.md#createbillingviewresponsetypedef)



#### Paginator usage example

```python
# ListBillingViewsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("billing") as client:  # (1)
    paginator = client.get_paginator("list_billing_views")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [BillingClient](./client.md)
2. paginator: [ListBillingViewsPaginator](./paginators.md#listbillingviewspaginator)
3. item: [:material-code-braces: ListBillingViewsResponseTypeDef](./type_defs.md#listbillingviewsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[billing]`
or a standalone `types_aiobotocore_billing` package, you have to explicitly specify
`client: BillingClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# BillingClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_billing.client import BillingClient
from types_aiobotocore_billing.type_defs import CreateBillingViewResponseTypeDef
from types_aiobotocore_billing.type_defs import CreateBillingViewRequestTypeDef


session = Session()

client: BillingClient
async with session.client("billing") as client:  # (1)
    kwargs: CreateBillingViewRequestTypeDef = {...}  # (2)
    result: CreateBillingViewResponseTypeDef = await client.create_billing_view(**kwargs)  # (3)
```

1. client: [BillingClient](./client.md)
2. kwargs: [:material-code-braces: CreateBillingViewRequestTypeDef](./type_defs.md#createbillingviewrequesttypedef)
3. result: [:material-code-braces: CreateBillingViewResponseTypeDef](./type_defs.md#createbillingviewresponsetypedef)



#### Paginator usage example

```python
# ListBillingViewsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_billing.client import BillingClient
from types_aiobotocore_billing.paginator import ListBillingViewsPaginator
from types_aiobotocore_billing.type_defs import ListBillingViewsResponseTypeDef


session = Session()

client: BillingClient
async with session.client("billing") as client:  # (1)
    paginator: ListBillingViewsPaginator = client.get_paginator("list_billing_views")  # (2)
    async for item in paginator.paginate(...):
        item: ListBillingViewsResponseTypeDef
        print(item)  # (3)
```

1. client: [BillingClient](./client.md)
2. paginator: [ListBillingViewsPaginator](./paginators.md#listbillingviewspaginator)
3. item: [:material-code-braces: ListBillingViewsResponseTypeDef](./type_defs.md#listbillingviewsresponsetypedef)




