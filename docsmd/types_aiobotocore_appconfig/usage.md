# Examples

> [Index](../README.md) > [AppConfig](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AppConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#appconfig)
    type annotations stubs module [types-aiobotocore-appconfig](https://pypi.org/project/types-aiobotocore-appconfig/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[appconfig]` package installed.

Write your `AppConfig` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# AppConfigClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("appconfig") as client:  # (1)
    result = await client.create_application()  # (2)
```

1. client: [AppConfigClient](./client.md)
2. result: [:material-code-braces: ApplicationResponseTypeDef](./type_defs.md#applicationresponsetypedef)



#### Paginator usage example

```python
# ListApplicationsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("appconfig") as client:  # (1)
    paginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AppConfigClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: [:material-code-braces: ApplicationsTypeDef](./type_defs.md#applicationstypedef)




### Explicit type annotations

With `types-aioboto3-lite[appconfig]`
or a standalone `types_aiobotocore_appconfig` package, you have to explicitly specify
`client: AppConfigClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# AppConfigClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_appconfig.client import AppConfigClient
from types_aiobotocore_appconfig.type_defs import ApplicationResponseTypeDef
from types_aiobotocore_appconfig.type_defs import CreateApplicationRequestTypeDef


session = Session()

client: AppConfigClient
async with session.client("appconfig") as client:  # (1)
    kwargs: CreateApplicationRequestTypeDef = {...}  # (2)
    result: ApplicationResponseTypeDef = await client.create_application(**kwargs)  # (3)
```

1. client: [AppConfigClient](./client.md)
2. kwargs: [:material-code-braces: CreateApplicationRequestTypeDef](./type_defs.md#createapplicationrequesttypedef)
3. result: [:material-code-braces: ApplicationResponseTypeDef](./type_defs.md#applicationresponsetypedef)



#### Paginator usage example

```python
# ListApplicationsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_appconfig.client import AppConfigClient
from types_aiobotocore_appconfig.paginator import ListApplicationsPaginator
from types_aiobotocore_appconfig.type_defs import ApplicationsTypeDef


session = Session()

client: AppConfigClient
async with session.client("appconfig") as client:  # (1)
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        item: ApplicationsTypeDef
        print(item)  # (3)
```

1. client: [AppConfigClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: [:material-code-braces: ApplicationsTypeDef](./type_defs.md#applicationstypedef)




