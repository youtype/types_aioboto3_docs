# Paginators

> [Index](../README.md) > [AppStream](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [AppStream](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
    type annotations stubs module [types-aiobotocore-appstream](https://pypi.org/project/types-aiobotocore-appstream/).

## DescribeDirectoryConfigsPaginator

Type annotations and code completion for `#!python session.client("appstream").get_paginator("describe_directory_configs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeDirectoryConfigs)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_appstream.paginator import DescribeDirectoryConfigsPaginator

session = Session()

session = get_session()
async with session.client("appstream") as client:  # (1)
    paginator: DescribeDirectoryConfigsPaginator = client.get_paginator("describe_directory_configs")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDirectoryConfigsResultTypeDef
        print(item)  # (3)
```

1. client: [AppStreamClient](./client.md)
2. paginator: [DescribeDirectoryConfigsPaginator](./paginators.md#describedirectoryconfigspaginator)
3. item: [:material-code-braces: DescribeDirectoryConfigsResultTypeDef](./type_defs.md#describedirectoryconfigsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDirectoryConfigsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DirectoryNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeDirectoryConfigsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeDirectoryConfigsResultTypeDef](./type_defs.md#describedirectoryconfigsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef = {  # (1)
    "DirectoryNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef](./type_defs.md#describedirectoryconfigsrequestdescribedirectoryconfigspaginatetypedef) 
## DescribeFleetsPaginator

Type annotations and code completion for `#!python session.client("appstream").get_paginator("describe_fleets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeFleets)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_appstream.paginator import DescribeFleetsPaginator

session = Session()

session = get_session()
async with session.client("appstream") as client:  # (1)
    paginator: DescribeFleetsPaginator = client.get_paginator("describe_fleets")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeFleetsResultTypeDef
        print(item)  # (3)
```

1. client: [AppStreamClient](./client.md)
2. paginator: [DescribeFleetsPaginator](./paginators.md#describefleetspaginator)
3. item: [:material-code-braces: DescribeFleetsResultTypeDef](./type_defs.md#describefleetsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeFleetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Names: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeFleetsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeFleetsResultTypeDef](./type_defs.md#describefleetsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeFleetsRequestDescribeFleetsPaginateTypeDef = {  # (1)
    "Names": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFleetsRequestDescribeFleetsPaginateTypeDef](./type_defs.md#describefleetsrequestdescribefleetspaginatetypedef) 
## DescribeImageBuildersPaginator

Type annotations and code completion for `#!python session.client("appstream").get_paginator("describe_image_builders")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeImageBuilders)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_appstream.paginator import DescribeImageBuildersPaginator

session = Session()

session = get_session()
async with session.client("appstream") as client:  # (1)
    paginator: DescribeImageBuildersPaginator = client.get_paginator("describe_image_builders")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeImageBuildersResultTypeDef
        print(item)  # (3)
```

1. client: [AppStreamClient](./client.md)
2. paginator: [DescribeImageBuildersPaginator](./paginators.md#describeimagebuilderspaginator)
3. item: [:material-code-braces: DescribeImageBuildersResultTypeDef](./type_defs.md#describeimagebuildersresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeImageBuildersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Names: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeImageBuildersResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeImageBuildersResultTypeDef](./type_defs.md#describeimagebuildersresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef = {  # (1)
    "Names": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef](./type_defs.md#describeimagebuildersrequestdescribeimagebuilderspaginatetypedef) 
## DescribeImagesPaginator

Type annotations and code completion for `#!python session.client("appstream").get_paginator("describe_images")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeImages)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_appstream.paginator import DescribeImagesPaginator

session = Session()

session = get_session()
async with session.client("appstream") as client:  # (1)
    paginator: DescribeImagesPaginator = client.get_paginator("describe_images")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeImagesResultTypeDef
        print(item)  # (3)
```

1. client: [AppStreamClient](./client.md)
2. paginator: [DescribeImagesPaginator](./paginators.md#describeimagespaginator)
3. item: [:material-code-braces: DescribeImagesResultTypeDef](./type_defs.md#describeimagesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeImagesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Names: Sequence[str] = ...,
    Arns: Sequence[str] = ...,
    Type: VisibilityTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeImagesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: VisibilityTypeType](./literals.md#visibilitytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeImagesResultTypeDef](./type_defs.md#describeimagesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeImagesRequestDescribeImagesPaginateTypeDef = {  # (1)
    "Names": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeImagesRequestDescribeImagesPaginateTypeDef](./type_defs.md#describeimagesrequestdescribeimagespaginatetypedef) 
## DescribeSessionsPaginator

Type annotations and code completion for `#!python session.client("appstream").get_paginator("describe_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeSessions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_appstream.paginator import DescribeSessionsPaginator

session = Session()

session = get_session()
async with session.client("appstream") as client:  # (1)
    paginator: DescribeSessionsPaginator = client.get_paginator("describe_sessions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSessionsResultTypeDef
        print(item)  # (3)
```

1. client: [AppStreamClient](./client.md)
2. paginator: [DescribeSessionsPaginator](./paginators.md#describesessionspaginator)
3. item: [:material-code-braces: DescribeSessionsResultTypeDef](./type_defs.md#describesessionsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSessionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    StackName: str,
    FleetName: str,
    UserId: str = ...,
    AuthenticationType: AuthenticationTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeSessionsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeSessionsResultTypeDef](./type_defs.md#describesessionsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeSessionsRequestDescribeSessionsPaginateTypeDef = {  # (1)
    "StackName": ...,
    "FleetName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSessionsRequestDescribeSessionsPaginateTypeDef](./type_defs.md#describesessionsrequestdescribesessionspaginatetypedef) 
## DescribeStacksPaginator

Type annotations and code completion for `#!python session.client("appstream").get_paginator("describe_stacks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeStacks)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_appstream.paginator import DescribeStacksPaginator

session = Session()

session = get_session()
async with session.client("appstream") as client:  # (1)
    paginator: DescribeStacksPaginator = client.get_paginator("describe_stacks")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeStacksResultTypeDef
        print(item)  # (3)
```

1. client: [AppStreamClient](./client.md)
2. paginator: [DescribeStacksPaginator](./paginators.md#describestackspaginator)
3. item: [:material-code-braces: DescribeStacksResultTypeDef](./type_defs.md#describestacksresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeStacksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Names: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeStacksResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeStacksResultTypeDef](./type_defs.md#describestacksresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeStacksRequestDescribeStacksPaginateTypeDef = {  # (1)
    "Names": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeStacksRequestDescribeStacksPaginateTypeDef](./type_defs.md#describestacksrequestdescribestackspaginatetypedef) 
## DescribeUserStackAssociationsPaginator

Type annotations and code completion for `#!python session.client("appstream").get_paginator("describe_user_stack_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeUserStackAssociations)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_appstream.paginator import DescribeUserStackAssociationsPaginator

session = Session()

session = get_session()
async with session.client("appstream") as client:  # (1)
    paginator: DescribeUserStackAssociationsPaginator = client.get_paginator("describe_user_stack_associations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeUserStackAssociationsResultTypeDef
        print(item)  # (3)
```

1. client: [AppStreamClient](./client.md)
2. paginator: [DescribeUserStackAssociationsPaginator](./paginators.md#describeuserstackassociationspaginator)
3. item: [:material-code-braces: DescribeUserStackAssociationsResultTypeDef](./type_defs.md#describeuserstackassociationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeUserStackAssociationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    StackName: str = ...,
    UserName: str = ...,
    AuthenticationType: AuthenticationTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeUserStackAssociationsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeUserStackAssociationsResultTypeDef](./type_defs.md#describeuserstackassociationsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef = {  # (1)
    "StackName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef](./type_defs.md#describeuserstackassociationsrequestdescribeuserstackassociationspaginatetypedef) 
## DescribeUsersPaginator

Type annotations and code completion for `#!python session.client("appstream").get_paginator("describe_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.DescribeUsers)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_appstream.paginator import DescribeUsersPaginator

session = Session()

session = get_session()
async with session.client("appstream") as client:  # (1)
    paginator: DescribeUsersPaginator = client.get_paginator("describe_users")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeUsersResultTypeDef
        print(item)  # (3)
```

1. client: [AppStreamClient](./client.md)
2. paginator: [DescribeUsersPaginator](./paginators.md#describeuserspaginator)
3. item: [:material-code-braces: DescribeUsersResultTypeDef](./type_defs.md#describeusersresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeUsersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AuthenticationType: AuthenticationTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeUsersResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeUsersResultTypeDef](./type_defs.md#describeusersresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeUsersRequestDescribeUsersPaginateTypeDef = {  # (1)
    "AuthenticationType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeUsersRequestDescribeUsersPaginateTypeDef](./type_defs.md#describeusersrequestdescribeuserspaginatetypedef) 
## ListAssociatedFleetsPaginator

Type annotations and code completion for `#!python session.client("appstream").get_paginator("list_associated_fleets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.ListAssociatedFleets)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_appstream.paginator import ListAssociatedFleetsPaginator

session = Session()

session = get_session()
async with session.client("appstream") as client:  # (1)
    paginator: ListAssociatedFleetsPaginator = client.get_paginator("list_associated_fleets")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssociatedFleetsResultTypeDef
        print(item)  # (3)
```

1. client: [AppStreamClient](./client.md)
2. paginator: [ListAssociatedFleetsPaginator](./paginators.md#listassociatedfleetspaginator)
3. item: [:material-code-braces: ListAssociatedFleetsResultTypeDef](./type_defs.md#listassociatedfleetsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListAssociatedFleetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    StackName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAssociatedFleetsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAssociatedFleetsResultTypeDef](./type_defs.md#listassociatedfleetsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef = {  # (1)
    "StackName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef](./type_defs.md#listassociatedfleetsrequestlistassociatedfleetspaginatetypedef) 
## ListAssociatedStacksPaginator

Type annotations and code completion for `#!python session.client("appstream").get_paginator("list_associated_stacks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Paginator.ListAssociatedStacks)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_appstream.paginator import ListAssociatedStacksPaginator

session = Session()

session = get_session()
async with session.client("appstream") as client:  # (1)
    paginator: ListAssociatedStacksPaginator = client.get_paginator("list_associated_stacks")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssociatedStacksResultTypeDef
        print(item)  # (3)
```

1. client: [AppStreamClient](./client.md)
2. paginator: [ListAssociatedStacksPaginator](./paginators.md#listassociatedstackspaginator)
3. item: [:material-code-braces: ListAssociatedStacksResultTypeDef](./type_defs.md#listassociatedstacksresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListAssociatedStacksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    FleetName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAssociatedStacksResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAssociatedStacksResultTypeDef](./type_defs.md#listassociatedstacksresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef = {  # (1)
    "FleetName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef](./type_defs.md#listassociatedstacksrequestlistassociatedstackspaginatetypedef) 
