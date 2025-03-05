# Examples

> [Index](../README.md) > [AmplifyUIBuilder](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AmplifyUIBuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#amplifyuibuilder)
    type annotations stubs module [types-aiobotocore-amplifyuibuilder](https://pypi.org/project/types-aiobotocore-amplifyuibuilder/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[amplifyuibuilder]` package installed.

Write your `AmplifyUIBuilder` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# AmplifyUIBuilderClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("amplifyuibuilder") as client:  # (1)
    result = await client.create_component()  # (2)
```

1. client: [AmplifyUIBuilderClient](./client.md)
2. result: [:material-code-braces: CreateComponentResponseTypeDef](./type_defs.md#createcomponentresponsetypedef)



#### Paginator usage example

```python
# ExportComponentsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("amplifyuibuilder") as client:  # (1)
    paginator = client.get_paginator("export_components")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AmplifyUIBuilderClient](./client.md)
2. paginator: [ExportComponentsPaginator](./paginators.md#exportcomponentspaginator)
3. item: [:material-code-braces: ExportComponentsResponseTypeDef](./type_defs.md#exportcomponentsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[amplifyuibuilder]`
or a standalone `types_aiobotocore_amplifyuibuilder` package, you have to explicitly specify
`client: AmplifyUIBuilderClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# AmplifyUIBuilderClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_amplifyuibuilder.client import AmplifyUIBuilderClient
from types_aiobotocore_amplifyuibuilder.type_defs import CreateComponentResponseTypeDef
from types_aiobotocore_amplifyuibuilder.type_defs import CreateComponentRequestTypeDef


session = Session()

client: AmplifyUIBuilderClient
async with session.client("amplifyuibuilder") as client:  # (1)
    kwargs: CreateComponentRequestTypeDef = {...}  # (2)
    result: CreateComponentResponseTypeDef = await client.create_component(**kwargs)  # (3)
```

1. client: [AmplifyUIBuilderClient](./client.md)
2. kwargs: [:material-code-braces: CreateComponentRequestTypeDef](./type_defs.md#createcomponentrequesttypedef)
3. result: [:material-code-braces: CreateComponentResponseTypeDef](./type_defs.md#createcomponentresponsetypedef)



#### Paginator usage example

```python
# ExportComponentsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_amplifyuibuilder.client import AmplifyUIBuilderClient
from types_aiobotocore_amplifyuibuilder.paginator import ExportComponentsPaginator
from types_aiobotocore_amplifyuibuilder.type_defs import ExportComponentsResponseTypeDef


session = Session()

client: AmplifyUIBuilderClient
async with session.client("amplifyuibuilder") as client:  # (1)
    paginator: ExportComponentsPaginator = client.get_paginator("export_components")  # (2)
    async for item in paginator.paginate(...):
        item: ExportComponentsResponseTypeDef
        print(item)  # (3)
```

1. client: [AmplifyUIBuilderClient](./client.md)
2. paginator: [ExportComponentsPaginator](./paginators.md#exportcomponentspaginator)
3. item: [:material-code-braces: ExportComponentsResponseTypeDef](./type_defs.md#exportcomponentsresponsetypedef)




