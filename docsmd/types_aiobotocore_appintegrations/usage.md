# Examples

> [Index](../README.md) > [AppIntegrationsService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AppIntegrationsService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#appintegrationsservice)
    type annotations stubs module [types-aiobotocore-appintegrations](https://pypi.org/project/types-aiobotocore-appintegrations/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[appintegrations]` package installed.

Write your `AppIntegrationsService` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# AppIntegrationsServiceClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("appintegrations") as client:  # (1)
    result = await client.create_application()  # (2)
```

1. client: [AppIntegrationsServiceClient](./client.md)
2. result: [:material-code-braces: CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef)



#### Paginator usage example

```python
# ListApplicationAssociationsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("appintegrations") as client:  # (1)
    paginator = client.get_paginator("list_application_associations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AppIntegrationsServiceClient](./client.md)
2. paginator: [ListApplicationAssociationsPaginator](./paginators.md#listapplicationassociationspaginator)
3. item: [:material-code-braces: ListApplicationAssociationsResponseTypeDef](./type_defs.md#listapplicationassociationsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[appintegrations]`
or a standalone `types_aiobotocore_appintegrations` package, you have to explicitly specify
`client: AppIntegrationsServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# AppIntegrationsServiceClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_appintegrations.client import AppIntegrationsServiceClient
from types_aiobotocore_appintegrations.type_defs import CreateApplicationResponseTypeDef
from types_aiobotocore_appintegrations.type_defs import CreateApplicationRequestTypeDef


session = Session()

client: AppIntegrationsServiceClient
async with session.client("appintegrations") as client:  # (1)
    kwargs: CreateApplicationRequestTypeDef = {...}  # (2)
    result: CreateApplicationResponseTypeDef = await client.create_application(**kwargs)  # (3)
```

1. client: [AppIntegrationsServiceClient](./client.md)
2. kwargs: [:material-code-braces: CreateApplicationRequestTypeDef](./type_defs.md#createapplicationrequesttypedef)
3. result: [:material-code-braces: CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef)



#### Paginator usage example

```python
# ListApplicationAssociationsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_appintegrations.client import AppIntegrationsServiceClient
from types_aiobotocore_appintegrations.paginator import ListApplicationAssociationsPaginator
from types_aiobotocore_appintegrations.type_defs import ListApplicationAssociationsResponseTypeDef


session = Session()

client: AppIntegrationsServiceClient
async with session.client("appintegrations") as client:  # (1)
    paginator: ListApplicationAssociationsPaginator = client.get_paginator("list_application_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [AppIntegrationsServiceClient](./client.md)
2. paginator: [ListApplicationAssociationsPaginator](./paginators.md#listapplicationassociationspaginator)
3. item: [:material-code-braces: ListApplicationAssociationsResponseTypeDef](./type_defs.md#listapplicationassociationsresponsetypedef)




