# Paginators

> [Index](../README.md) > [AppRegistry](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [AppRegistry](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
    type annotations stubs module [types-aiobotocore-servicecatalog-appregistry](https://pypi.org/project/types-aiobotocore-servicecatalog-appregistry/).

## ListApplicationsPaginator

Type annotations and code completion for `#!python session.client("servicecatalog-appregistry").get_paginator("list_applications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListApplications)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_servicecatalog_appregistry.paginator import ListApplicationsPaginator

session = Session()

session = get_session()
async with session.client("servicecatalog-appregistry") as client:  # (1)
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationsResponseTypeDef
        print(item)  # (3)
```

1. client: [AppRegistryClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListApplicationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListApplicationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListApplicationsRequestListApplicationsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationsRequestListApplicationsPaginateTypeDef](./type_defs.md#listapplicationsrequestlistapplicationspaginatetypedef) 
## ListAssociatedAttributeGroupsPaginator

Type annotations and code completion for `#!python session.client("servicecatalog-appregistry").get_paginator("list_associated_attribute_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedAttributeGroups)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_servicecatalog_appregistry.paginator import ListAssociatedAttributeGroupsPaginator

session = Session()

session = get_session()
async with session.client("servicecatalog-appregistry") as client:  # (1)
    paginator: ListAssociatedAttributeGroupsPaginator = client.get_paginator("list_associated_attribute_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssociatedAttributeGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [AppRegistryClient](./client.md)
2. paginator: [ListAssociatedAttributeGroupsPaginator](./paginators.md#listassociatedattributegroupspaginator)
3. item: [:material-code-braces: ListAssociatedAttributeGroupsResponseTypeDef](./type_defs.md#listassociatedattributegroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssociatedAttributeGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    application: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAssociatedAttributeGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAssociatedAttributeGroupsResponseTypeDef](./type_defs.md#listassociatedattributegroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = {  # (1)
    "application": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef](./type_defs.md#listassociatedattributegroupsrequestlistassociatedattributegroupspaginatetypedef) 
## ListAssociatedResourcesPaginator

Type annotations and code completion for `#!python session.client("servicecatalog-appregistry").get_paginator("list_associated_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedResources)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_servicecatalog_appregistry.paginator import ListAssociatedResourcesPaginator

session = Session()

session = get_session()
async with session.client("servicecatalog-appregistry") as client:  # (1)
    paginator: ListAssociatedResourcesPaginator = client.get_paginator("list_associated_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssociatedResourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [AppRegistryClient](./client.md)
2. paginator: [ListAssociatedResourcesPaginator](./paginators.md#listassociatedresourcespaginator)
3. item: [:material-code-braces: ListAssociatedResourcesResponseTypeDef](./type_defs.md#listassociatedresourcesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssociatedResourcesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    application: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAssociatedResourcesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAssociatedResourcesResponseTypeDef](./type_defs.md#listassociatedresourcesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = {  # (1)
    "application": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef](./type_defs.md#listassociatedresourcesrequestlistassociatedresourcespaginatetypedef) 
## ListAttributeGroupsPaginator

Type annotations and code completion for `#!python session.client("servicecatalog-appregistry").get_paginator("list_attribute_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroups)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_servicecatalog_appregistry.paginator import ListAttributeGroupsPaginator

session = Session()

session = get_session()
async with session.client("servicecatalog-appregistry") as client:  # (1)
    paginator: ListAttributeGroupsPaginator = client.get_paginator("list_attribute_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListAttributeGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [AppRegistryClient](./client.md)
2. paginator: [ListAttributeGroupsPaginator](./paginators.md#listattributegroupspaginator)
3. item: [:material-code-braces: ListAttributeGroupsResponseTypeDef](./type_defs.md#listattributegroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAttributeGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAttributeGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAttributeGroupsResponseTypeDef](./type_defs.md#listattributegroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef](./type_defs.md#listattributegroupsrequestlistattributegroupspaginatetypedef) 
