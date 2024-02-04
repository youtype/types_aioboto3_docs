# Paginators

> [Index](../README.md) > [GlueDataBrew](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [GlueDataBrew](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
    type annotations stubs module [types-aiobotocore-databrew](https://pypi.org/project/types-aiobotocore-databrew/).

## ListDatasetsPaginator

Type annotations and code completion for `#!python session.client("databrew").get_paginator("list_datasets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListDatasets)

```python
# ListDatasetsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_databrew.paginator import ListDatasetsPaginator

session = Session()

session = get_session()
async with session.client("databrew") as client:  # (1)
    paginator: ListDatasetsPaginator = client.get_paginator("list_datasets")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatasetsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [GlueDataBrewClient](./client.md)
2. paginator: [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
3. item: [:material-code-braces: ListDatasetsResponsePaginatorTypeDef](./type_defs.md#listdatasetsresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListDatasetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDatasetsResponsePaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDatasetsResponsePaginatorTypeDef](./type_defs.md#listdatasetsresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDatasetsRequestListDatasetsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetsRequestListDatasetsPaginateTypeDef](./type_defs.md#listdatasetsrequestlistdatasetspaginatetypedef) 
## ListJobRunsPaginator

Type annotations and code completion for `#!python session.client("databrew").get_paginator("list_job_runs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListJobRuns)

```python
# ListJobRunsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_databrew.paginator import ListJobRunsPaginator

session = Session()

session = get_session()
async with session.client("databrew") as client:  # (1)
    paginator: ListJobRunsPaginator = client.get_paginator("list_job_runs")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobRunsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [GlueDataBrewClient](./client.md)
2. paginator: [ListJobRunsPaginator](./paginators.md#listjobrunspaginator)
3. item: [:material-code-braces: ListJobRunsResponsePaginatorTypeDef](./type_defs.md#listjobrunsresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListJobRunsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Name: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListJobRunsResponsePaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListJobRunsResponsePaginatorTypeDef](./type_defs.md#listjobrunsresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListJobRunsRequestListJobRunsPaginateTypeDef = {  # (1)
    "Name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobRunsRequestListJobRunsPaginateTypeDef](./type_defs.md#listjobrunsrequestlistjobrunspaginatetypedef) 
## ListJobsPaginator

Type annotations and code completion for `#!python session.client("databrew").get_paginator("list_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListJobs)

```python
# ListJobsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_databrew.paginator import ListJobsPaginator

session = Session()

session = get_session()
async with session.client("databrew") as client:  # (1)
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [GlueDataBrewClient](./client.md)
2. paginator: [ListJobsPaginator](./paginators.md#listjobspaginator)
3. item: [:material-code-braces: ListJobsResponsePaginatorTypeDef](./type_defs.md#listjobsresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DatasetName: str = ...,
    ProjectName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListJobsResponsePaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListJobsResponsePaginatorTypeDef](./type_defs.md#listjobsresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListJobsRequestListJobsPaginateTypeDef = {  # (1)
    "DatasetName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestListJobsPaginateTypeDef](./type_defs.md#listjobsrequestlistjobspaginatetypedef) 
## ListProjectsPaginator

Type annotations and code completion for `#!python session.client("databrew").get_paginator("list_projects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListProjects)

```python
# ListProjectsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_databrew.paginator import ListProjectsPaginator

session = Session()

session = get_session()
async with session.client("databrew") as client:  # (1)
    paginator: ListProjectsPaginator = client.get_paginator("list_projects")  # (2)
    async for item in paginator.paginate(...):
        item: ListProjectsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueDataBrewClient](./client.md)
2. paginator: [ListProjectsPaginator](./paginators.md#listprojectspaginator)
3. item: [:material-code-braces: ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListProjectsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListProjectsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListProjectsRequestListProjectsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProjectsRequestListProjectsPaginateTypeDef](./type_defs.md#listprojectsrequestlistprojectspaginatetypedef) 
## ListRecipeVersionsPaginator

Type annotations and code completion for `#!python session.client("databrew").get_paginator("list_recipe_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRecipeVersions)

```python
# ListRecipeVersionsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_databrew.paginator import ListRecipeVersionsPaginator

session = Session()

session = get_session()
async with session.client("databrew") as client:  # (1)
    paginator: ListRecipeVersionsPaginator = client.get_paginator("list_recipe_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecipeVersionsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [GlueDataBrewClient](./client.md)
2. paginator: [ListRecipeVersionsPaginator](./paginators.md#listrecipeversionspaginator)
3. item: [:material-code-braces: ListRecipeVersionsResponsePaginatorTypeDef](./type_defs.md#listrecipeversionsresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListRecipeVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Name: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRecipeVersionsResponsePaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRecipeVersionsResponsePaginatorTypeDef](./type_defs.md#listrecipeversionsresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef = {  # (1)
    "Name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef](./type_defs.md#listrecipeversionsrequestlistrecipeversionspaginatetypedef) 
## ListRecipesPaginator

Type annotations and code completion for `#!python session.client("databrew").get_paginator("list_recipes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRecipes)

```python
# ListRecipesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_databrew.paginator import ListRecipesPaginator

session = Session()

session = get_session()
async with session.client("databrew") as client:  # (1)
    paginator: ListRecipesPaginator = client.get_paginator("list_recipes")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecipesResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [GlueDataBrewClient](./client.md)
2. paginator: [ListRecipesPaginator](./paginators.md#listrecipespaginator)
3. item: [:material-code-braces: ListRecipesResponsePaginatorTypeDef](./type_defs.md#listrecipesresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListRecipesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RecipeVersion: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRecipesResponsePaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRecipesResponsePaginatorTypeDef](./type_defs.md#listrecipesresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRecipesRequestListRecipesPaginateTypeDef = {  # (1)
    "RecipeVersion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecipesRequestListRecipesPaginateTypeDef](./type_defs.md#listrecipesrequestlistrecipespaginatetypedef) 
## ListRulesetsPaginator

Type annotations and code completion for `#!python session.client("databrew").get_paginator("list_rulesets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRulesets)

```python
# ListRulesetsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_databrew.paginator import ListRulesetsPaginator

session = Session()

session = get_session()
async with session.client("databrew") as client:  # (1)
    paginator: ListRulesetsPaginator = client.get_paginator("list_rulesets")  # (2)
    async for item in paginator.paginate(...):
        item: ListRulesetsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueDataBrewClient](./client.md)
2. paginator: [ListRulesetsPaginator](./paginators.md#listrulesetspaginator)
3. item: [:material-code-braces: ListRulesetsResponseTypeDef](./type_defs.md#listrulesetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRulesetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TargetArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRulesetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRulesetsResponseTypeDef](./type_defs.md#listrulesetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRulesetsRequestListRulesetsPaginateTypeDef = {  # (1)
    "TargetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRulesetsRequestListRulesetsPaginateTypeDef](./type_defs.md#listrulesetsrequestlistrulesetspaginatetypedef) 
## ListSchedulesPaginator

Type annotations and code completion for `#!python session.client("databrew").get_paginator("list_schedules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListSchedules)

```python
# ListSchedulesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_databrew.paginator import ListSchedulesPaginator

session = Session()

session = get_session()
async with session.client("databrew") as client:  # (1)
    paginator: ListSchedulesPaginator = client.get_paginator("list_schedules")  # (2)
    async for item in paginator.paginate(...):
        item: ListSchedulesResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueDataBrewClient](./client.md)
2. paginator: [ListSchedulesPaginator](./paginators.md#listschedulespaginator)
3. item: [:material-code-braces: ListSchedulesResponseTypeDef](./type_defs.md#listschedulesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSchedulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    JobName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSchedulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSchedulesResponseTypeDef](./type_defs.md#listschedulesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSchedulesRequestListSchedulesPaginateTypeDef = {  # (1)
    "JobName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchedulesRequestListSchedulesPaginateTypeDef](./type_defs.md#listschedulesrequestlistschedulespaginatetypedef) 
