# Paginators

> [Index](../README.md) > [CloudWatchEvidently](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CloudWatchEvidently](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
    type annotations stubs module [types-aiobotocore-evidently](https://pypi.org/project/types-aiobotocore-evidently/).

## ListExperimentsPaginator

Type annotations and code completion for `#!python session.client("evidently").get_paginator("list_experiments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListExperiments)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_evidently.paginator import ListExperimentsPaginator

session = Session()

session = get_session()
async with session.client("evidently") as client:  # (1)
    paginator: ListExperimentsPaginator = client.get_paginator("list_experiments")  # (2)
    async for item in paginator.paginate(...):
        item: ListExperimentsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchEvidentlyClient](./client.md)
2. paginator: [ListExperimentsPaginator](./paginators.md#listexperimentspaginator)
3. item: [:material-code-braces: ListExperimentsResponseTypeDef](./type_defs.md#listexperimentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListExperimentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    project: str,
    status: ExperimentStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListExperimentsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ExperimentStatusType](./literals.md#experimentstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListExperimentsResponseTypeDef](./type_defs.md#listexperimentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListExperimentsRequestListExperimentsPaginateTypeDef = {  # (1)
    "project": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListExperimentsRequestListExperimentsPaginateTypeDef](./type_defs.md#listexperimentsrequestlistexperimentspaginatetypedef) 
## ListFeaturesPaginator

Type annotations and code completion for `#!python session.client("evidently").get_paginator("list_features")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListFeatures)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_evidently.paginator import ListFeaturesPaginator

session = Session()

session = get_session()
async with session.client("evidently") as client:  # (1)
    paginator: ListFeaturesPaginator = client.get_paginator("list_features")  # (2)
    async for item in paginator.paginate(...):
        item: ListFeaturesResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchEvidentlyClient](./client.md)
2. paginator: [ListFeaturesPaginator](./paginators.md#listfeaturespaginator)
3. item: [:material-code-braces: ListFeaturesResponseTypeDef](./type_defs.md#listfeaturesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFeaturesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    project: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListFeaturesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFeaturesResponseTypeDef](./type_defs.md#listfeaturesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListFeaturesRequestListFeaturesPaginateTypeDef = {  # (1)
    "project": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFeaturesRequestListFeaturesPaginateTypeDef](./type_defs.md#listfeaturesrequestlistfeaturespaginatetypedef) 
## ListLaunchesPaginator

Type annotations and code completion for `#!python session.client("evidently").get_paginator("list_launches")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListLaunches)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_evidently.paginator import ListLaunchesPaginator

session = Session()

session = get_session()
async with session.client("evidently") as client:  # (1)
    paginator: ListLaunchesPaginator = client.get_paginator("list_launches")  # (2)
    async for item in paginator.paginate(...):
        item: ListLaunchesResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchEvidentlyClient](./client.md)
2. paginator: [ListLaunchesPaginator](./paginators.md#listlaunchespaginator)
3. item: [:material-code-braces: ListLaunchesResponseTypeDef](./type_defs.md#listlaunchesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListLaunchesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    project: str,
    status: LaunchStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListLaunchesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: LaunchStatusType](./literals.md#launchstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListLaunchesResponseTypeDef](./type_defs.md#listlaunchesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListLaunchesRequestListLaunchesPaginateTypeDef = {  # (1)
    "project": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLaunchesRequestListLaunchesPaginateTypeDef](./type_defs.md#listlaunchesrequestlistlaunchespaginatetypedef) 
## ListProjectsPaginator

Type annotations and code completion for `#!python session.client("evidently").get_paginator("list_projects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListProjects)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_evidently.paginator import ListProjectsPaginator

session = Session()

session = get_session()
async with session.client("evidently") as client:  # (1)
    paginator: ListProjectsPaginator = client.get_paginator("list_projects")  # (2)
    async for item in paginator.paginate(...):
        item: ListProjectsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchEvidentlyClient](./client.md)
2. paginator: [ListProjectsPaginator](./paginators.md#listprojectspaginator)
3. item: [:material-code-braces: ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListProjectsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListProjectsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListProjectsRequestListProjectsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProjectsRequestListProjectsPaginateTypeDef](./type_defs.md#listprojectsrequestlistprojectspaginatetypedef) 
