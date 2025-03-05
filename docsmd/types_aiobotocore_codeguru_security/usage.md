# Examples

> [Index](../README.md) > [CodeGuruSecurity](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CodeGuruSecurity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#codegurusecurity)
    type annotations stubs module [types-aiobotocore-codeguru-security](https://pypi.org/project/types-aiobotocore-codeguru-security/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[codeguru-security]` package installed.

Write your `CodeGuruSecurity` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# CodeGuruSecurityClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("codeguru-security") as client:  # (1)
    result = await client.batch_get_findings()  # (2)
```

1. client: [CodeGuruSecurityClient](./client.md)
2. result: [:material-code-braces: BatchGetFindingsResponseTypeDef](./type_defs.md#batchgetfindingsresponsetypedef)



#### Paginator usage example

```python
# GetFindingsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("codeguru-security") as client:  # (1)
    paginator = client.get_paginator("get_findings")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CodeGuruSecurityClient](./client.md)
2. paginator: [GetFindingsPaginator](./paginators.md#getfindingspaginator)
3. item: [:material-code-braces: GetFindingsResponseTypeDef](./type_defs.md#getfindingsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[codeguru-security]`
or a standalone `types_aiobotocore_codeguru_security` package, you have to explicitly specify
`client: CodeGuruSecurityClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# CodeGuruSecurityClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_codeguru_security.client import CodeGuruSecurityClient
from types_aiobotocore_codeguru_security.type_defs import BatchGetFindingsResponseTypeDef
from types_aiobotocore_codeguru_security.type_defs import BatchGetFindingsRequestTypeDef


session = Session()

client: CodeGuruSecurityClient
async with session.client("codeguru-security") as client:  # (1)
    kwargs: BatchGetFindingsRequestTypeDef = {...}  # (2)
    result: BatchGetFindingsResponseTypeDef = await client.batch_get_findings(**kwargs)  # (3)
```

1. client: [CodeGuruSecurityClient](./client.md)
2. kwargs: [:material-code-braces: BatchGetFindingsRequestTypeDef](./type_defs.md#batchgetfindingsrequesttypedef)
3. result: [:material-code-braces: BatchGetFindingsResponseTypeDef](./type_defs.md#batchgetfindingsresponsetypedef)



#### Paginator usage example

```python
# GetFindingsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_codeguru_security.client import CodeGuruSecurityClient
from types_aiobotocore_codeguru_security.paginator import GetFindingsPaginator
from types_aiobotocore_codeguru_security.type_defs import GetFindingsResponseTypeDef


session = Session()

client: CodeGuruSecurityClient
async with session.client("codeguru-security") as client:  # (1)
    paginator: GetFindingsPaginator = client.get_paginator("get_findings")  # (2)
    async for item in paginator.paginate(...):
        item: GetFindingsResponseTypeDef
        print(item)  # (3)
```

1. client: [CodeGuruSecurityClient](./client.md)
2. paginator: [GetFindingsPaginator](./paginators.md#getfindingspaginator)
3. item: [:material-code-braces: GetFindingsResponseTypeDef](./type_defs.md#getfindingsresponsetypedef)




