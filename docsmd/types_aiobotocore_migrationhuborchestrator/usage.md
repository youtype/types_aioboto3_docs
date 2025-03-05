# Examples

> [Index](../README.md) > [MigrationHubOrchestrator](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MigrationHubOrchestrator](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#migrationhuborchestrator)
    type annotations stubs module [types-aiobotocore-migrationhuborchestrator](https://pypi.org/project/types-aiobotocore-migrationhuborchestrator/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[migrationhuborchestrator]` package installed.

Write your `MigrationHubOrchestrator` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# MigrationHubOrchestratorClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("migrationhuborchestrator") as client:  # (1)
    result = await client.create_template()  # (2)
```

1. client: [MigrationHubOrchestratorClient](./client.md)
2. result: [:material-code-braces: CreateTemplateResponseTypeDef](./type_defs.md#createtemplateresponsetypedef)



#### Paginator usage example

```python
# ListPluginsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("migrationhuborchestrator") as client:  # (1)
    paginator = client.get_paginator("list_plugins")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MigrationHubOrchestratorClient](./client.md)
2. paginator: [ListPluginsPaginator](./paginators.md#listpluginspaginator)
3. item: [:material-code-braces: ListPluginsResponseTypeDef](./type_defs.md#listpluginsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[migrationhuborchestrator]`
or a standalone `types_aiobotocore_migrationhuborchestrator` package, you have to explicitly specify
`client: MigrationHubOrchestratorClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# MigrationHubOrchestratorClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_migrationhuborchestrator.client import MigrationHubOrchestratorClient
from types_aiobotocore_migrationhuborchestrator.type_defs import CreateTemplateResponseTypeDef
from types_aiobotocore_migrationhuborchestrator.type_defs import CreateTemplateRequestTypeDef


session = Session()

client: MigrationHubOrchestratorClient
async with session.client("migrationhuborchestrator") as client:  # (1)
    kwargs: CreateTemplateRequestTypeDef = {...}  # (2)
    result: CreateTemplateResponseTypeDef = await client.create_template(**kwargs)  # (3)
```

1. client: [MigrationHubOrchestratorClient](./client.md)
2. kwargs: [:material-code-braces: CreateTemplateRequestTypeDef](./type_defs.md#createtemplaterequesttypedef)
3. result: [:material-code-braces: CreateTemplateResponseTypeDef](./type_defs.md#createtemplateresponsetypedef)



#### Paginator usage example

```python
# ListPluginsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_migrationhuborchestrator.client import MigrationHubOrchestratorClient
from types_aiobotocore_migrationhuborchestrator.paginator import ListPluginsPaginator
from types_aiobotocore_migrationhuborchestrator.type_defs import ListPluginsResponseTypeDef


session = Session()

client: MigrationHubOrchestratorClient
async with session.client("migrationhuborchestrator") as client:  # (1)
    paginator: ListPluginsPaginator = client.get_paginator("list_plugins")  # (2)
    async for item in paginator.paginate(...):
        item: ListPluginsResponseTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubOrchestratorClient](./client.md)
2. paginator: [ListPluginsPaginator](./paginators.md#listpluginspaginator)
3. item: [:material-code-braces: ListPluginsResponseTypeDef](./type_defs.md#listpluginsresponsetypedef)




