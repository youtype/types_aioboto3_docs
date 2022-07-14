# Paginators

> [Index](../README.md) > [MigrationHubRefactorSpaces](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MigrationHubRefactorSpaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
    type annotations stubs module [types-aiobotocore-migration-hub-refactor-spaces](https://pypi.org/project/types-aiobotocore-migration-hub-refactor-spaces/).

## ListApplicationsPaginator

Type annotations and code completion for `#!python session.client("migration-hub-refactor-spaces").get_paginator("list_applications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListApplications)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_migration_hub_refactor_spaces.paginator import ListApplicationsPaginator

session = Session()

session = get_session()
async with session.client("migration-hub-refactor-spaces") as client:  # (1)
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationsResponseTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubRefactorSpacesClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListApplicationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    EnvironmentIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListApplicationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListApplicationsRequestListApplicationsPaginateTypeDef = {  # (1)
    "EnvironmentIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationsRequestListApplicationsPaginateTypeDef](./type_defs.md#listapplicationsrequestlistapplicationspaginatetypedef) 
## ListEnvironmentVpcsPaginator

Type annotations and code completion for `#!python session.client("migration-hub-refactor-spaces").get_paginator("list_environment_vpcs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListEnvironmentVpcs)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_migration_hub_refactor_spaces.paginator import ListEnvironmentVpcsPaginator

session = Session()

session = get_session()
async with session.client("migration-hub-refactor-spaces") as client:  # (1)
    paginator: ListEnvironmentVpcsPaginator = client.get_paginator("list_environment_vpcs")  # (2)
    async for item in paginator.paginate(...):
        item: ListEnvironmentVpcsResponseTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubRefactorSpacesClient](./client.md)
2. paginator: [ListEnvironmentVpcsPaginator](./paginators.md#listenvironmentvpcspaginator)
3. item: [:material-code-braces: ListEnvironmentVpcsResponseTypeDef](./type_defs.md#listenvironmentvpcsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEnvironmentVpcsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    EnvironmentIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEnvironmentVpcsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEnvironmentVpcsResponseTypeDef](./type_defs.md#listenvironmentvpcsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef = {  # (1)
    "EnvironmentIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef](./type_defs.md#listenvironmentvpcsrequestlistenvironmentvpcspaginatetypedef) 
## ListEnvironmentsPaginator

Type annotations and code completion for `#!python session.client("migration-hub-refactor-spaces").get_paginator("list_environments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListEnvironments)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_migration_hub_refactor_spaces.paginator import ListEnvironmentsPaginator

session = Session()

session = get_session()
async with session.client("migration-hub-refactor-spaces") as client:  # (1)
    paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")  # (2)
    async for item in paginator.paginate(...):
        item: ListEnvironmentsResponseTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubRefactorSpacesClient](./client.md)
2. paginator: [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)
3. item: [:material-code-braces: ListEnvironmentsResponseTypeDef](./type_defs.md#listenvironmentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEnvironmentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEnvironmentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEnvironmentsResponseTypeDef](./type_defs.md#listenvironmentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentsRequestListEnvironmentsPaginateTypeDef](./type_defs.md#listenvironmentsrequestlistenvironmentspaginatetypedef) 
## ListRoutesPaginator

Type annotations and code completion for `#!python session.client("migration-hub-refactor-spaces").get_paginator("list_routes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListRoutes)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_migration_hub_refactor_spaces.paginator import ListRoutesPaginator

session = Session()

session = get_session()
async with session.client("migration-hub-refactor-spaces") as client:  # (1)
    paginator: ListRoutesPaginator = client.get_paginator("list_routes")  # (2)
    async for item in paginator.paginate(...):
        item: ListRoutesResponseTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubRefactorSpacesClient](./client.md)
2. paginator: [ListRoutesPaginator](./paginators.md#listroutespaginator)
3. item: [:material-code-braces: ListRoutesResponseTypeDef](./type_defs.md#listroutesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRoutesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ApplicationIdentifier: str,
    EnvironmentIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRoutesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRoutesResponseTypeDef](./type_defs.md#listroutesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRoutesRequestListRoutesPaginateTypeDef = {  # (1)
    "ApplicationIdentifier": ...,
    "EnvironmentIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRoutesRequestListRoutesPaginateTypeDef](./type_defs.md#listroutesrequestlistroutespaginatetypedef) 
## ListServicesPaginator

Type annotations and code completion for `#!python session.client("migration-hub-refactor-spaces").get_paginator("list_services")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListServices)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_migration_hub_refactor_spaces.paginator import ListServicesPaginator

session = Session()

session = get_session()
async with session.client("migration-hub-refactor-spaces") as client:  # (1)
    paginator: ListServicesPaginator = client.get_paginator("list_services")  # (2)
    async for item in paginator.paginate(...):
        item: ListServicesResponseTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubRefactorSpacesClient](./client.md)
2. paginator: [ListServicesPaginator](./paginators.md#listservicespaginator)
3. item: [:material-code-braces: ListServicesResponseTypeDef](./type_defs.md#listservicesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListServicesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ApplicationIdentifier: str,
    EnvironmentIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListServicesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListServicesResponseTypeDef](./type_defs.md#listservicesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListServicesRequestListServicesPaginateTypeDef = {  # (1)
    "ApplicationIdentifier": ...,
    "EnvironmentIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListServicesRequestListServicesPaginateTypeDef](./type_defs.md#listservicesrequestlistservicespaginatetypedef) 
