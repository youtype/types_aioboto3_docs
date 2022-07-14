# Paginators

> [Index](../README.md) > [Schemas](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Schemas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
    type annotations stubs module [types-aiobotocore-schemas](https://pypi.org/project/types-aiobotocore-schemas/).

## ListDiscoverersPaginator

Type annotations and code completion for `#!python session.client("schemas").get_paginator("list_discoverers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListDiscoverers)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_schemas.paginator import ListDiscoverersPaginator

session = Session()

session = get_session()
async with session.client("schemas") as client:  # (1)
    paginator: ListDiscoverersPaginator = client.get_paginator("list_discoverers")  # (2)
    async for item in paginator.paginate(...):
        item: ListDiscoverersResponseTypeDef
        print(item)  # (3)
```

1. client: [SchemasClient](./client.md)
2. paginator: [ListDiscoverersPaginator](./paginators.md#listdiscovererspaginator)
3. item: [:material-code-braces: ListDiscoverersResponseTypeDef](./type_defs.md#listdiscoverersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDiscoverersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DiscovererIdPrefix: str = ...,
    SourceArnPrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDiscoverersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDiscoverersResponseTypeDef](./type_defs.md#listdiscoverersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDiscoverersRequestListDiscoverersPaginateTypeDef = {  # (1)
    "DiscovererIdPrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDiscoverersRequestListDiscoverersPaginateTypeDef](./type_defs.md#listdiscoverersrequestlistdiscovererspaginatetypedef) 
## ListRegistriesPaginator

Type annotations and code completion for `#!python session.client("schemas").get_paginator("list_registries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListRegistries)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_schemas.paginator import ListRegistriesPaginator

session = Session()

session = get_session()
async with session.client("schemas") as client:  # (1)
    paginator: ListRegistriesPaginator = client.get_paginator("list_registries")  # (2)
    async for item in paginator.paginate(...):
        item: ListRegistriesResponseTypeDef
        print(item)  # (3)
```

1. client: [SchemasClient](./client.md)
2. paginator: [ListRegistriesPaginator](./paginators.md#listregistriespaginator)
3. item: [:material-code-braces: ListRegistriesResponseTypeDef](./type_defs.md#listregistriesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRegistriesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    RegistryNamePrefix: str = ...,
    Scope: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRegistriesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRegistriesResponseTypeDef](./type_defs.md#listregistriesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRegistriesRequestListRegistriesPaginateTypeDef = {  # (1)
    "RegistryNamePrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRegistriesRequestListRegistriesPaginateTypeDef](./type_defs.md#listregistriesrequestlistregistriespaginatetypedef) 
## ListSchemaVersionsPaginator

Type annotations and code completion for `#!python session.client("schemas").get_paginator("list_schema_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemaVersions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_schemas.paginator import ListSchemaVersionsPaginator

session = Session()

session = get_session()
async with session.client("schemas") as client:  # (1)
    paginator: ListSchemaVersionsPaginator = client.get_paginator("list_schema_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSchemaVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [SchemasClient](./client.md)
2. paginator: [ListSchemaVersionsPaginator](./paginators.md#listschemaversionspaginator)
3. item: [:material-code-braces: ListSchemaVersionsResponseTypeDef](./type_defs.md#listschemaversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSchemaVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    RegistryName: str,
    SchemaName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSchemaVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSchemaVersionsResponseTypeDef](./type_defs.md#listschemaversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = {  # (1)
    "RegistryName": ...,
    "SchemaName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef](./type_defs.md#listschemaversionsrequestlistschemaversionspaginatetypedef) 
## ListSchemasPaginator

Type annotations and code completion for `#!python session.client("schemas").get_paginator("list_schemas")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemas)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_schemas.paginator import ListSchemasPaginator

session = Session()

session = get_session()
async with session.client("schemas") as client:  # (1)
    paginator: ListSchemasPaginator = client.get_paginator("list_schemas")  # (2)
    async for item in paginator.paginate(...):
        item: ListSchemasResponseTypeDef
        print(item)  # (3)
```

1. client: [SchemasClient](./client.md)
2. paginator: [ListSchemasPaginator](./paginators.md#listschemaspaginator)
3. item: [:material-code-braces: ListSchemasResponseTypeDef](./type_defs.md#listschemasresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSchemasPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    RegistryName: str,
    SchemaNamePrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSchemasResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSchemasResponseTypeDef](./type_defs.md#listschemasresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSchemasRequestListSchemasPaginateTypeDef = {  # (1)
    "RegistryName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchemasRequestListSchemasPaginateTypeDef](./type_defs.md#listschemasrequestlistschemaspaginatetypedef) 
## SearchSchemasPaginator

Type annotations and code completion for `#!python session.client("schemas").get_paginator("search_schemas")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.SearchSchemas)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_schemas.paginator import SearchSchemasPaginator

session = Session()

session = get_session()
async with session.client("schemas") as client:  # (1)
    paginator: SearchSchemasPaginator = client.get_paginator("search_schemas")  # (2)
    async for item in paginator.paginate(...):
        item: SearchSchemasResponseTypeDef
        print(item)  # (3)
```

1. client: [SchemasClient](./client.md)
2. paginator: [SearchSchemasPaginator](./paginators.md#searchschemaspaginator)
3. item: [:material-code-braces: SearchSchemasResponseTypeDef](./type_defs.md#searchschemasresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchSchemasPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Keywords: str,
    RegistryName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[SearchSchemasResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: SearchSchemasResponseTypeDef](./type_defs.md#searchschemasresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SearchSchemasRequestSearchSchemasPaginateTypeDef = {  # (1)
    "Keywords": ...,
    "RegistryName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchSchemasRequestSearchSchemasPaginateTypeDef](./type_defs.md#searchschemasrequestsearchschemaspaginatetypedef) 
