# Examples

> [Index](../README.md) > [WorkSpaces](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WorkSpaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#workspaces)
    type annotations stubs module [types-aiobotocore-workspaces](https://pypi.org/project/types-aiobotocore-workspaces/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[workspaces]` package installed.

Write your `WorkSpaces` code as usual,
type checking and code completion should work out of the box.



```python
# WorkSpacesClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("workspaces") as client:  # (1)
    result = await client.accept_account_link_invitation()  # (2)
```

1. client: [WorkSpacesClient](./client.md)
2. result: [:material-code-braces: AcceptAccountLinkInvitationResultTypeDef](./type_defs.md#acceptaccountlinkinvitationresulttypedef) 



```python
# DescribeAccountModificationsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("workspaces") as client:  # (1)
    paginator = client.get_paginator("describe_account_modifications")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [WorkSpacesClient](./client.md)
2. paginator: [DescribeAccountModificationsPaginator](./paginators.md#describeaccountmodificationspaginator)
3. item: [:material-code-braces: DescribeAccountModificationsResultTypeDef](./type_defs.md#describeaccountmodificationsresulttypedef) 




### Explicit type annotations

With `types-aioboto3-lite[workspaces]`
or a standalone `types_aiobotocore_workspaces` package, you have to explicitly specify
`client: WorkSpacesClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# WorkSpacesClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_workspaces.client import WorkSpacesClient
from types_aiobotocore_workspaces.type_defs import AcceptAccountLinkInvitationResultTypeDef
from types_aiobotocore_workspaces.type_defs import AcceptAccountLinkInvitationRequestRequestTypeDef


session = Session()

client: WorkSpacesClient
async with session.client("workspaces") as client:  # (1)
    kwargs: AcceptAccountLinkInvitationRequestRequestTypeDef = {...}  # (2)
    result: AcceptAccountLinkInvitationResultTypeDef = await client.accept_account_link_invitation(**kwargs)  # (3)
```

1. client: [WorkSpacesClient](./client.md)
2. kwargs: [:material-code-braces: AcceptAccountLinkInvitationRequestRequestTypeDef](./type_defs.md#acceptaccountlinkinvitationrequestrequesttypedef) 
3. result: [:material-code-braces: AcceptAccountLinkInvitationResultTypeDef](./type_defs.md#acceptaccountlinkinvitationresulttypedef) 



```python
# DescribeAccountModificationsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_workspaces.client import WorkSpacesClient
from types_aiobotocore_workspaces.paginator import DescribeAccountModificationsPaginator
from types_aiobotocore_workspaces.type_defs import DescribeAccountModificationsResultTypeDef


session = Session()

client: WorkSpacesClient
async with session.client("workspaces") as client:  # (1)
    paginator: DescribeAccountModificationsPaginator = client.get_paginator("describe_account_modifications")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAccountModificationsResultTypeDef
        print(item)  # (3)
```

1. client: [WorkSpacesClient](./client.md)
2. paginator: [DescribeAccountModificationsPaginator](./paginators.md#describeaccountmodificationspaginator)
3. item: [:material-code-braces: DescribeAccountModificationsResultTypeDef](./type_defs.md#describeaccountmodificationsresulttypedef) 



