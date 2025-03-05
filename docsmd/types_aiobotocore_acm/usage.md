# Examples

> [Index](../README.md) > [ACM](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ACM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#acm)
    type annotations stubs module [types-aiobotocore-acm](https://pypi.org/project/types-aiobotocore-acm/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[acm]` package installed.

Write your `ACM` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ACMClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("acm") as client:  # (1)
    result = await client.add_tags_to_certificate()  # (2)
```

1. client: [ACMClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# ListCertificatesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("acm") as client:  # (1)
    paginator = client.get_paginator("list_certificates")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ACMClient](./client.md)
2. paginator: [ListCertificatesPaginator](./paginators.md#listcertificatespaginator)
3. item: [:material-code-braces: ListCertificatesResponseTypeDef](./type_defs.md#listcertificatesresponsetypedef)



#### Waiter usage example

```python
# CertificateValidatedWaiter usage example

from aioboto3.session import Session


session = Session()

async with session.client("acm") as client:  # (1)
    waiter = client.get_waiter("certificate_validated")  # (2)
    await waiter.wait(...)
```

1. client: [ACMClient](./client.md)
2. waiter: [CertificateValidatedWaiter](./waiters.md#certificatevalidatedwaiter)


### Explicit type annotations

With `types-aioboto3-lite[acm]`
or a standalone `types_aiobotocore_acm` package, you have to explicitly specify
`client: ACMClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ACMClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_acm.client import ACMClient
from types_aiobotocore_acm.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_acm.type_defs import AddTagsToCertificateRequestTypeDef


session = Session()

client: ACMClient
async with session.client("acm") as client:  # (1)
    kwargs: AddTagsToCertificateRequestTypeDef = {...}  # (2)
    result: EmptyResponseMetadataTypeDef = await client.add_tags_to_certificate(**kwargs)  # (3)
```

1. client: [ACMClient](./client.md)
2. kwargs: [:material-code-braces: AddTagsToCertificateRequestTypeDef](./type_defs.md#addtagstocertificaterequesttypedef)
3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# ListCertificatesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_acm.client import ACMClient
from types_aiobotocore_acm.paginator import ListCertificatesPaginator
from types_aiobotocore_acm.type_defs import ListCertificatesResponseTypeDef


session = Session()

client: ACMClient
async with session.client("acm") as client:  # (1)
    paginator: ListCertificatesPaginator = client.get_paginator("list_certificates")  # (2)
    async for item in paginator.paginate(...):
        item: ListCertificatesResponseTypeDef
        print(item)  # (3)
```

1. client: [ACMClient](./client.md)
2. paginator: [ListCertificatesPaginator](./paginators.md#listcertificatespaginator)
3. item: [:material-code-braces: ListCertificatesResponseTypeDef](./type_defs.md#listcertificatesresponsetypedef)



#### Waiter usage example

```python
# CertificateValidatedWaiter usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_acm.client import ACMClient
from types_aiobotocore_acm.waiter import CertificateValidatedWaiter


session = Session()

async with session.client("acm") as client:  # (1)
    waiter = client.get_waiter("certificate_validated")  # (2)
    await waiter.wait(...)
```

1. client: [ACMClient](./client.md)
2. waiter: [CertificateValidatedWaiter](./waiters.md#certificatevalidatedwaiter)


