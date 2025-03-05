# Examples

> [Index](../README.md) > [PaymentCryptographyControlPlane](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [PaymentCryptographyControlPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#paymentcryptographycontrolplane)
    type annotations stubs module [types-aiobotocore-payment-cryptography](https://pypi.org/project/types-aiobotocore-payment-cryptography/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[payment-cryptography]` package installed.

Write your `PaymentCryptographyControlPlane` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# PaymentCryptographyControlPlaneClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("payment-cryptography") as client:  # (1)
    result = await client.create_alias()  # (2)
```

1. client: [PaymentCryptographyControlPlaneClient](./client.md)
2. result: [:material-code-braces: CreateAliasOutputTypeDef](./type_defs.md#createaliasoutputtypedef)



#### Paginator usage example

```python
# ListAliasesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("payment-cryptography") as client:  # (1)
    paginator = client.get_paginator("list_aliases")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [PaymentCryptographyControlPlaneClient](./client.md)
2. paginator: [ListAliasesPaginator](./paginators.md#listaliasespaginator)
3. item: [:material-code-braces: ListAliasesOutputTypeDef](./type_defs.md#listaliasesoutputtypedef)




### Explicit type annotations

With `types-aioboto3-lite[payment-cryptography]`
or a standalone `types_aiobotocore_payment_cryptography` package, you have to explicitly specify
`client: PaymentCryptographyControlPlaneClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# PaymentCryptographyControlPlaneClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_payment_cryptography.client import PaymentCryptographyControlPlaneClient
from types_aiobotocore_payment_cryptography.type_defs import CreateAliasOutputTypeDef
from types_aiobotocore_payment_cryptography.type_defs import CreateAliasInputTypeDef


session = Session()

client: PaymentCryptographyControlPlaneClient
async with session.client("payment-cryptography") as client:  # (1)
    kwargs: CreateAliasInputTypeDef = {...}  # (2)
    result: CreateAliasOutputTypeDef = await client.create_alias(**kwargs)  # (3)
```

1. client: [PaymentCryptographyControlPlaneClient](./client.md)
2. kwargs: [:material-code-braces: CreateAliasInputTypeDef](./type_defs.md#createaliasinputtypedef)
3. result: [:material-code-braces: CreateAliasOutputTypeDef](./type_defs.md#createaliasoutputtypedef)



#### Paginator usage example

```python
# ListAliasesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_payment_cryptography.client import PaymentCryptographyControlPlaneClient
from types_aiobotocore_payment_cryptography.paginator import ListAliasesPaginator
from types_aiobotocore_payment_cryptography.type_defs import ListAliasesOutputTypeDef


session = Session()

client: PaymentCryptographyControlPlaneClient
async with session.client("payment-cryptography") as client:  # (1)
    paginator: ListAliasesPaginator = client.get_paginator("list_aliases")  # (2)
    async for item in paginator.paginate(...):
        item: ListAliasesOutputTypeDef
        print(item)  # (3)
```

1. client: [PaymentCryptographyControlPlaneClient](./client.md)
2. paginator: [ListAliasesPaginator](./paginators.md#listaliasespaginator)
3. item: [:material-code-braces: ListAliasesOutputTypeDef](./type_defs.md#listaliasesoutputtypedef)




