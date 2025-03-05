# Examples

> [Index](../README.md) > [EntityResolution](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EntityResolution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#entityresolution)
    type annotations stubs module [types-aiobotocore-entityresolution](https://pypi.org/project/types-aiobotocore-entityresolution/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[entityresolution]` package installed.

Write your `EntityResolution` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# EntityResolutionClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("entityresolution") as client:  # (1)
    result = await client.add_policy_statement()  # (2)
```

1. client: [EntityResolutionClient](./client.md)
2. result: [:material-code-braces: AddPolicyStatementOutputTypeDef](./type_defs.md#addpolicystatementoutputtypedef)



#### Paginator usage example

```python
# ListIdMappingJobsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("entityresolution") as client:  # (1)
    paginator = client.get_paginator("list_id_mapping_jobs")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [EntityResolutionClient](./client.md)
2. paginator: [ListIdMappingJobsPaginator](./paginators.md#listidmappingjobspaginator)
3. item: [:material-code-braces: ListIdMappingJobsOutputTypeDef](./type_defs.md#listidmappingjobsoutputtypedef)




### Explicit type annotations

With `types-aioboto3-lite[entityresolution]`
or a standalone `types_aiobotocore_entityresolution` package, you have to explicitly specify
`client: EntityResolutionClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# EntityResolutionClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_entityresolution.client import EntityResolutionClient
from types_aiobotocore_entityresolution.type_defs import AddPolicyStatementOutputTypeDef
from types_aiobotocore_entityresolution.type_defs import AddPolicyStatementInputTypeDef


session = Session()

client: EntityResolutionClient
async with session.client("entityresolution") as client:  # (1)
    kwargs: AddPolicyStatementInputTypeDef = {...}  # (2)
    result: AddPolicyStatementOutputTypeDef = await client.add_policy_statement(**kwargs)  # (3)
```

1. client: [EntityResolutionClient](./client.md)
2. kwargs: [:material-code-braces: AddPolicyStatementInputTypeDef](./type_defs.md#addpolicystatementinputtypedef)
3. result: [:material-code-braces: AddPolicyStatementOutputTypeDef](./type_defs.md#addpolicystatementoutputtypedef)



#### Paginator usage example

```python
# ListIdMappingJobsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_entityresolution.client import EntityResolutionClient
from types_aiobotocore_entityresolution.paginator import ListIdMappingJobsPaginator
from types_aiobotocore_entityresolution.type_defs import ListIdMappingJobsOutputTypeDef


session = Session()

client: EntityResolutionClient
async with session.client("entityresolution") as client:  # (1)
    paginator: ListIdMappingJobsPaginator = client.get_paginator("list_id_mapping_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListIdMappingJobsOutputTypeDef
        print(item)  # (3)
```

1. client: [EntityResolutionClient](./client.md)
2. paginator: [ListIdMappingJobsPaginator](./paginators.md#listidmappingjobspaginator)
3. item: [:material-code-braces: ListIdMappingJobsOutputTypeDef](./type_defs.md#listidmappingjobsoutputtypedef)




