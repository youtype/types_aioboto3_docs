# Examples

> [Index](../README.md) > [WorkMail](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WorkMail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
    type annotations stubs module [types-aiobotocore-workmail](https://pypi.org/project/types-aiobotocore-workmail/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[workmail]` package installed.

Write your `WorkMail` code as usual,
type checking and code completion should work out of the box.



```python
# WorkMailClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("workmail") as client:  # (1)
    result = await client.assume_impersonation_role()  # (2)
```

1. client: [WorkMailClient](./client.md)
2. result: [:material-code-braces: AssumeImpersonationRoleResponseTypeDef](./type_defs.md#assumeimpersonationroleresponsetypedef) 



```python
# ListAliasesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("workmail") as client:  # (1)
    paginator = client.get_paginator("list_aliases")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [WorkMailClient](./client.md)
2. paginator: [ListAliasesPaginator](./paginators.md#listaliasespaginator)
3. item: [:material-code-braces: ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[workmail]`
or a standalone `types_aiobotocore_workmail` package, you have to explicitly specify
`client: WorkMailClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# WorkMailClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_workmail.client import WorkMailClient
from types_aiobotocore_workmail.type_defs import AssumeImpersonationRoleResponseTypeDef
from types_aiobotocore_workmail.type_defs import AssumeImpersonationRoleRequestRequestTypeDef


session = Session()

client: WorkMailClient
async with session.client("workmail") as client:  # (1)
    kwargs: AssumeImpersonationRoleRequestRequestTypeDef = {...}  # (2)
    result: AssumeImpersonationRoleResponseTypeDef = await client.assume_impersonation_role(**kwargs)  # (3)
```

1. client: [WorkMailClient](./client.md)
2. kwargs: [:material-code-braces: AssumeImpersonationRoleRequestRequestTypeDef](./type_defs.md#assumeimpersonationrolerequestrequesttypedef) 
3. result: [:material-code-braces: AssumeImpersonationRoleResponseTypeDef](./type_defs.md#assumeimpersonationroleresponsetypedef) 



```python
# ListAliasesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_workmail.client import WorkMailClient
from types_aiobotocore_workmail.paginator import ListAliasesPaginator
from types_aiobotocore_workmail.type_defs import ListAliasesResponseTypeDef


session = Session()

client: WorkMailClient
async with session.client("workmail") as client:  # (1)
    paginator: ListAliasesPaginator = client.get_paginator("list_aliases")  # (2)
    async for item in paginator.paginate(...):
        item: ListAliasesResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkMailClient](./client.md)
2. paginator: [ListAliasesPaginator](./paginators.md#listaliasespaginator)
3. item: [:material-code-braces: ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef) 




