# Examples

> [Index](../README.md) > [DocDB](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DocDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#docdb)
    type annotations stubs module [types-aiobotocore-docdb](https://pypi.org/project/types-aiobotocore-docdb/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[docdb]` package installed.

Write your `DocDB` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# DocDBClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("docdb") as client:  # (1)
    result = await client.add_source_identifier_to_subscription()  # (2)
```

1. client: [DocDBClient](./client.md)
2. result: [:material-code-braces: AddSourceIdentifierToSubscriptionResultTypeDef](./type_defs.md#addsourceidentifiertosubscriptionresulttypedef)



#### Paginator usage example

```python
# DescribeCertificatesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("docdb") as client:  # (1)
    paginator = client.get_paginator("describe_certificates")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DocDBClient](./client.md)
2. paginator: [DescribeCertificatesPaginator](./paginators.md#describecertificatespaginator)
3. item: [:material-code-braces: CertificateMessageTypeDef](./type_defs.md#certificatemessagetypedef)



#### Waiter usage example

```python
# DBInstanceAvailableWaiter usage example

from aioboto3.session import Session


session = Session()

async with session.client("docdb") as client:  # (1)
    waiter = client.get_waiter("db_instance_available")  # (2)
    await waiter.wait(...)
```

1. client: [DocDBClient](./client.md)
2. waiter: [DBInstanceAvailableWaiter](./waiters.md#dbinstanceavailablewaiter)


### Explicit type annotations

With `types-aioboto3-lite[docdb]`
or a standalone `types_aiobotocore_docdb` package, you have to explicitly specify
`client: DocDBClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# DocDBClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_docdb.client import DocDBClient
from types_aiobotocore_docdb.type_defs import AddSourceIdentifierToSubscriptionResultTypeDef
from types_aiobotocore_docdb.type_defs import AddSourceIdentifierToSubscriptionMessageTypeDef


session = Session()

client: DocDBClient
async with session.client("docdb") as client:  # (1)
    kwargs: AddSourceIdentifierToSubscriptionMessageTypeDef = {...}  # (2)
    result: AddSourceIdentifierToSubscriptionResultTypeDef = await client.add_source_identifier_to_subscription(**kwargs)  # (3)
```

1. client: [DocDBClient](./client.md)
2. kwargs: [:material-code-braces: AddSourceIdentifierToSubscriptionMessageTypeDef](./type_defs.md#addsourceidentifiertosubscriptionmessagetypedef)
3. result: [:material-code-braces: AddSourceIdentifierToSubscriptionResultTypeDef](./type_defs.md#addsourceidentifiertosubscriptionresulttypedef)



#### Paginator usage example

```python
# DescribeCertificatesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_docdb.client import DocDBClient
from types_aiobotocore_docdb.paginator import DescribeCertificatesPaginator
from types_aiobotocore_docdb.type_defs import CertificateMessageTypeDef


session = Session()

client: DocDBClient
async with session.client("docdb") as client:  # (1)
    paginator: DescribeCertificatesPaginator = client.get_paginator("describe_certificates")  # (2)
    async for item in paginator.paginate(...):
        item: CertificateMessageTypeDef
        print(item)  # (3)
```

1. client: [DocDBClient](./client.md)
2. paginator: [DescribeCertificatesPaginator](./paginators.md#describecertificatespaginator)
3. item: [:material-code-braces: CertificateMessageTypeDef](./type_defs.md#certificatemessagetypedef)



#### Waiter usage example

```python
# DBInstanceAvailableWaiter usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_docdb.client import DocDBClient
from types_aiobotocore_docdb.waiter import DBInstanceAvailableWaiter


session = Session()

async with session.client("docdb") as client:  # (1)
    waiter = client.get_waiter("db_instance_available")  # (2)
    await waiter.wait(...)
```

1. client: [DocDBClient](./client.md)
2. waiter: [DBInstanceAvailableWaiter](./waiters.md#dbinstanceavailablewaiter)


