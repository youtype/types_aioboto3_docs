# Examples

> [Index](../README.md) > [SimpleDB](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SimpleDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#simpledb)
    type annotations stubs module [types-aiobotocore-sdb](https://pypi.org/project/types-aiobotocore-sdb/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[sdb]` package installed.

Write your `SimpleDB` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# SimpleDBClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("sdb") as client:  # (1)
    result = await client.batch_delete_attributes()  # (2)
```

1. client: [SimpleDBClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# ListDomainsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("sdb") as client:  # (1)
    paginator = client.get_paginator("list_domains")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SimpleDBClient](./client.md)
2. paginator: [ListDomainsPaginator](./paginators.md#listdomainspaginator)
3. item: [:material-code-braces: ListDomainsResultTypeDef](./type_defs.md#listdomainsresulttypedef)




### Explicit type annotations

With `types-aioboto3-lite[sdb]`
or a standalone `types_aiobotocore_sdb` package, you have to explicitly specify
`client: SimpleDBClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# SimpleDBClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_sdb.client import SimpleDBClient
from types_aiobotocore_sdb.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_sdb.type_defs import BatchDeleteAttributesRequestTypeDef


session = Session()

client: SimpleDBClient
async with session.client("sdb") as client:  # (1)
    kwargs: BatchDeleteAttributesRequestTypeDef = {...}  # (2)
    result: EmptyResponseMetadataTypeDef = await client.batch_delete_attributes(**kwargs)  # (3)
```

1. client: [SimpleDBClient](./client.md)
2. kwargs: [:material-code-braces: BatchDeleteAttributesRequestTypeDef](./type_defs.md#batchdeleteattributesrequesttypedef)
3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# ListDomainsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_sdb.client import SimpleDBClient
from types_aiobotocore_sdb.paginator import ListDomainsPaginator
from types_aiobotocore_sdb.type_defs import ListDomainsResultTypeDef


session = Session()

client: SimpleDBClient
async with session.client("sdb") as client:  # (1)
    paginator: ListDomainsPaginator = client.get_paginator("list_domains")  # (2)
    async for item in paginator.paginate(...):
        item: ListDomainsResultTypeDef
        print(item)  # (3)
```

1. client: [SimpleDBClient](./client.md)
2. paginator: [ListDomainsPaginator](./paginators.md#listdomainspaginator)
3. item: [:material-code-braces: ListDomainsResultTypeDef](./type_defs.md#listdomainsresulttypedef)




