# Examples

> [Index](../README.md) > [Support](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Support](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#support)
    type annotations stubs module [types-aiobotocore-support](https://pypi.org/project/types-aiobotocore-support/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[support]` package installed.

Write your `Support` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# SupportClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("support") as client:  # (1)
    result = await client.add_attachments_to_set()  # (2)
```

1. client: [SupportClient](./client.md)
2. result: [:material-code-braces: AddAttachmentsToSetResponseTypeDef](./type_defs.md#addattachmentstosetresponsetypedef)



#### Paginator usage example

```python
# DescribeCasesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("support") as client:  # (1)
    paginator = client.get_paginator("describe_cases")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SupportClient](./client.md)
2. paginator: [DescribeCasesPaginator](./paginators.md#describecasespaginator)
3. item: [:material-code-braces: DescribeCasesResponseTypeDef](./type_defs.md#describecasesresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[support]`
or a standalone `types_aiobotocore_support` package, you have to explicitly specify
`client: SupportClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# SupportClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_support.client import SupportClient
from types_aiobotocore_support.type_defs import AddAttachmentsToSetResponseTypeDef
from types_aiobotocore_support.type_defs import AddAttachmentsToSetRequestTypeDef


session = Session()

client: SupportClient
async with session.client("support") as client:  # (1)
    kwargs: AddAttachmentsToSetRequestTypeDef = {...}  # (2)
    result: AddAttachmentsToSetResponseTypeDef = await client.add_attachments_to_set(**kwargs)  # (3)
```

1. client: [SupportClient](./client.md)
2. kwargs: [:material-code-braces: AddAttachmentsToSetRequestTypeDef](./type_defs.md#addattachmentstosetrequesttypedef)
3. result: [:material-code-braces: AddAttachmentsToSetResponseTypeDef](./type_defs.md#addattachmentstosetresponsetypedef)



#### Paginator usage example

```python
# DescribeCasesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_support.client import SupportClient
from types_aiobotocore_support.paginator import DescribeCasesPaginator
from types_aiobotocore_support.type_defs import DescribeCasesResponseTypeDef


session = Session()

client: SupportClient
async with session.client("support") as client:  # (1)
    paginator: DescribeCasesPaginator = client.get_paginator("describe_cases")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeCasesResponseTypeDef
        print(item)  # (3)
```

1. client: [SupportClient](./client.md)
2. paginator: [DescribeCasesPaginator](./paginators.md#describecasespaginator)
3. item: [:material-code-braces: DescribeCasesResponseTypeDef](./type_defs.md#describecasesresponsetypedef)




