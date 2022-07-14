# Paginators

> [Index](../README.md) > [AmplifyUIBuilder](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [AmplifyUIBuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
    type annotations stubs module [types-aiobotocore-amplifyuibuilder](https://pypi.org/project/types-aiobotocore-amplifyuibuilder/).

## ExportComponentsPaginator

Type annotations and code completion for `#!python session.client("amplifyuibuilder").get_paginator("export_components")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportComponents)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_amplifyuibuilder.paginator import ExportComponentsPaginator

session = Session()

session = get_session()
async with session.client("amplifyuibuilder") as client:  # (1)
    paginator: ExportComponentsPaginator = client.get_paginator("export_components")  # (2)
    async for item in paginator.paginate(...):
        item: ExportComponentsResponseTypeDef
        print(item)  # (3)
```

1. client: [AmplifyUIBuilderClient](./client.md)
2. paginator: [ExportComponentsPaginator](./paginators.md#exportcomponentspaginator)
3. item: [:material-code-braces: ExportComponentsResponseTypeDef](./type_defs.md#exportcomponentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ExportComponentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    appId: str,
    environmentName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ExportComponentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ExportComponentsResponseTypeDef](./type_defs.md#exportcomponentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ExportComponentsRequestExportComponentsPaginateTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ExportComponentsRequestExportComponentsPaginateTypeDef](./type_defs.md#exportcomponentsrequestexportcomponentspaginatetypedef) 
## ExportThemesPaginator

Type annotations and code completion for `#!python session.client("amplifyuibuilder").get_paginator("export_themes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportThemes)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_amplifyuibuilder.paginator import ExportThemesPaginator

session = Session()

session = get_session()
async with session.client("amplifyuibuilder") as client:  # (1)
    paginator: ExportThemesPaginator = client.get_paginator("export_themes")  # (2)
    async for item in paginator.paginate(...):
        item: ExportThemesResponseTypeDef
        print(item)  # (3)
```

1. client: [AmplifyUIBuilderClient](./client.md)
2. paginator: [ExportThemesPaginator](./paginators.md#exportthemespaginator)
3. item: [:material-code-braces: ExportThemesResponseTypeDef](./type_defs.md#exportthemesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ExportThemesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    appId: str,
    environmentName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ExportThemesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ExportThemesResponseTypeDef](./type_defs.md#exportthemesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ExportThemesRequestExportThemesPaginateTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ExportThemesRequestExportThemesPaginateTypeDef](./type_defs.md#exportthemesrequestexportthemespaginatetypedef) 
## ListComponentsPaginator

Type annotations and code completion for `#!python session.client("amplifyuibuilder").get_paginator("list_components")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListComponents)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_amplifyuibuilder.paginator import ListComponentsPaginator

session = Session()

session = get_session()
async with session.client("amplifyuibuilder") as client:  # (1)
    paginator: ListComponentsPaginator = client.get_paginator("list_components")  # (2)
    async for item in paginator.paginate(...):
        item: ListComponentsResponseTypeDef
        print(item)  # (3)
```

1. client: [AmplifyUIBuilderClient](./client.md)
2. paginator: [ListComponentsPaginator](./paginators.md#listcomponentspaginator)
3. item: [:material-code-braces: ListComponentsResponseTypeDef](./type_defs.md#listcomponentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListComponentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    appId: str,
    environmentName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListComponentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListComponentsResponseTypeDef](./type_defs.md#listcomponentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListComponentsRequestListComponentsPaginateTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListComponentsRequestListComponentsPaginateTypeDef](./type_defs.md#listcomponentsrequestlistcomponentspaginatetypedef) 
## ListThemesPaginator

Type annotations and code completion for `#!python session.client("amplifyuibuilder").get_paginator("list_themes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListThemes)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_amplifyuibuilder.paginator import ListThemesPaginator

session = Session()

session = get_session()
async with session.client("amplifyuibuilder") as client:  # (1)
    paginator: ListThemesPaginator = client.get_paginator("list_themes")  # (2)
    async for item in paginator.paginate(...):
        item: ListThemesResponseTypeDef
        print(item)  # (3)
```

1. client: [AmplifyUIBuilderClient](./client.md)
2. paginator: [ListThemesPaginator](./paginators.md#listthemespaginator)
3. item: [:material-code-braces: ListThemesResponseTypeDef](./type_defs.md#listthemesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListThemesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    appId: str,
    environmentName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListThemesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListThemesResponseTypeDef](./type_defs.md#listthemesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListThemesRequestListThemesPaginateTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThemesRequestListThemesPaginateTypeDef](./type_defs.md#listthemesrequestlistthemespaginatetypedef) 
