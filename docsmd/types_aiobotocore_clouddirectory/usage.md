# Examples

> [Index](../README.md) > [CloudDirectory](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudDirectory](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#clouddirectory)
    type annotations stubs module [types-aiobotocore-clouddirectory](https://pypi.org/project/types-aiobotocore-clouddirectory/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[clouddirectory]` package installed.

Write your `CloudDirectory` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# CloudDirectoryClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("clouddirectory") as client:  # (1)
    result = await client.apply_schema()  # (2)
```

1. client: [CloudDirectoryClient](./client.md)
2. result: [:material-code-braces: ApplySchemaResponseTypeDef](./type_defs.md#applyschemaresponsetypedef)



#### Paginator usage example

```python
# ListAppliedSchemaArnsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("clouddirectory") as client:  # (1)
    paginator = client.get_paginator("list_applied_schema_arns")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CloudDirectoryClient](./client.md)
2. paginator: [ListAppliedSchemaArnsPaginator](./paginators.md#listappliedschemaarnspaginator)
3. item: [:material-code-braces: ListAppliedSchemaArnsResponseTypeDef](./type_defs.md#listappliedschemaarnsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[clouddirectory]`
or a standalone `types_aiobotocore_clouddirectory` package, you have to explicitly specify
`client: CloudDirectoryClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# CloudDirectoryClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_clouddirectory.client import CloudDirectoryClient
from types_aiobotocore_clouddirectory.type_defs import ApplySchemaResponseTypeDef
from types_aiobotocore_clouddirectory.type_defs import ApplySchemaRequestTypeDef


session = Session()

client: CloudDirectoryClient
async with session.client("clouddirectory") as client:  # (1)
    kwargs: ApplySchemaRequestTypeDef = {...}  # (2)
    result: ApplySchemaResponseTypeDef = await client.apply_schema(**kwargs)  # (3)
```

1. client: [CloudDirectoryClient](./client.md)
2. kwargs: [:material-code-braces: ApplySchemaRequestTypeDef](./type_defs.md#applyschemarequesttypedef)
3. result: [:material-code-braces: ApplySchemaResponseTypeDef](./type_defs.md#applyschemaresponsetypedef)



#### Paginator usage example

```python
# ListAppliedSchemaArnsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_clouddirectory.client import CloudDirectoryClient
from types_aiobotocore_clouddirectory.paginator import ListAppliedSchemaArnsPaginator
from types_aiobotocore_clouddirectory.type_defs import ListAppliedSchemaArnsResponseTypeDef


session = Session()

client: CloudDirectoryClient
async with session.client("clouddirectory") as client:  # (1)
    paginator: ListAppliedSchemaArnsPaginator = client.get_paginator("list_applied_schema_arns")  # (2)
    async for item in paginator.paginate(...):
        item: ListAppliedSchemaArnsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudDirectoryClient](./client.md)
2. paginator: [ListAppliedSchemaArnsPaginator](./paginators.md#listappliedschemaarnspaginator)
3. item: [:material-code-braces: ListAppliedSchemaArnsResponseTypeDef](./type_defs.md#listappliedschemaarnsresponsetypedef)




