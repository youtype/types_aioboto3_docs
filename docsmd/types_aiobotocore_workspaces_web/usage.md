# Examples

> [Index](../README.md) > [WorkSpacesWeb](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WorkSpacesWeb](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
    type annotations stubs module [types-aiobotocore-workspaces-web](https://pypi.org/project/types-aiobotocore-workspaces-web/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[workspaces-web]` package installed.

Write your `WorkSpacesWeb` code as usual,
type checking and code completion should work out of the box.



```python
# WorkSpacesWebClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("workspaces-web") as client:  # (1)
    result = await client.associate_browser_settings()  # (2)
```

1. client: [WorkSpacesWebClient](./client.md)
2. result: [:material-code-braces: AssociateBrowserSettingsResponseTypeDef](./type_defs.md#associatebrowsersettingsresponsetypedef) 



```python
# ListSessionsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("workspaces-web") as client:  # (1)
    paginator = client.get_paginator("list_sessions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [WorkSpacesWebClient](./client.md)
2. paginator: [ListSessionsPaginator](./paginators.md#listsessionspaginator)
3. item: [:material-code-braces: ListSessionsResponseTypeDef](./type_defs.md#listsessionsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[workspaces-web]`
or a standalone `types_aiobotocore_workspaces_web` package, you have to explicitly specify
`client: WorkSpacesWebClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# WorkSpacesWebClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_workspaces_web.client import WorkSpacesWebClient
from types_aiobotocore_workspaces_web.type_defs import AssociateBrowserSettingsResponseTypeDef
from types_aiobotocore_workspaces_web.type_defs import AssociateBrowserSettingsRequestRequestTypeDef


session = Session()

client: WorkSpacesWebClient
async with session.client("workspaces-web") as client:  # (1)
    kwargs: AssociateBrowserSettingsRequestRequestTypeDef = {...}  # (2)
    result: AssociateBrowserSettingsResponseTypeDef = await client.associate_browser_settings(**kwargs)  # (3)
```

1. client: [WorkSpacesWebClient](./client.md)
2. kwargs: [:material-code-braces: AssociateBrowserSettingsRequestRequestTypeDef](./type_defs.md#associatebrowsersettingsrequestrequesttypedef) 
3. result: [:material-code-braces: AssociateBrowserSettingsResponseTypeDef](./type_defs.md#associatebrowsersettingsresponsetypedef) 



```python
# ListSessionsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_workspaces_web.client import WorkSpacesWebClient
from types_aiobotocore_workspaces_web.paginator import ListSessionsPaginator
from types_aiobotocore_workspaces_web.type_defs import ListSessionsResponseTypeDef


session = Session()

client: WorkSpacesWebClient
async with session.client("workspaces-web") as client:  # (1)
    paginator: ListSessionsPaginator = client.get_paginator("list_sessions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSessionsResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkSpacesWebClient](./client.md)
2. paginator: [ListSessionsPaginator](./paginators.md#listsessionspaginator)
3. item: [:material-code-braces: ListSessionsResponseTypeDef](./type_defs.md#listsessionsresponsetypedef) 




