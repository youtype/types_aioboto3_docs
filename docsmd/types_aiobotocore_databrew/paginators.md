# Paginators

> [Index](../README.md) > [GlueDataBrew](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [GlueDataBrew](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
    type annotations stubs module [types-aiobotocore-databrew](https://pypi.org/project/types-aiobotocore-databrew/).

## ListDatasetsPaginator

Type annotations and code completion for `#!python session.client("databrew").get_paginator("list_datasets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListDatasets)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_databrew.paginator import ListDatasetsPaginator

session = Session()

session = get_session()
async with session.client("databrew") as client:  # (1)
    paginator: ListDatasetsPaginator = client.get_paginator("list_datasets")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatasetsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueDataBrewClient](./client.md)
2. paginator: [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
3. item: [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDatasetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDatasetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDatasetsRequestListDatasetsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetsRequestListDatasetsPaginateTypeDef](./type_defs.md#listdatasetsrequestlistdatasetspaginatetypedef) 
## ListJobRunsPaginator

Type annotations and code completion for `#!python session.client("databrew").get_paginator("list_job_runs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListJobRuns)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_databrew.paginator import ListJobRunsPaginator

session = Session()

session = get_session()
async with session.client("databrew") as client:  # (1)
    paginator: ListJobRunsPaginator = client.get_paginator("list_job_runs")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobRunsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueDataBrewClient](./client.md)
2. paginator: [ListJobRunsPaginator](./paginators.md#listjobrunspaginator)
3. item: [:material-code-braces: ListJobRunsResponseTypeDef](./type_defs.md#listjobrunsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListJobRunsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Name: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListJobRunsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListJobRunsResponseTypeDef](./type_defs.md#listjobrunsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListJobRunsRequestListJobRunsPaginateTypeDef = {  # (1)
    "Name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobRunsRequestListJobRunsPaginateTypeDef](./type_defs.md#listjobrunsrequestlistjobrunspaginatetypedef) 
## ListJobsPaginator

Type annotations and code completion for `#!python session.client("databrew").get_paginator("list_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListJobs)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_databrew.paginator import ListJobsPaginator

session = Session()

session = get_session()
async with session.client("databrew") as client:  # (1)
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueDataBrewClient](./client.md)
2. paginator: [ListJobsPaginator](./paginators.md#listjobspaginator)
3. item: [:material-code-braces: ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DatasetName: str = ...,
    ProjectName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListJobsRequestListJobsPaginateTypeDef = {  # (1)
    "DatasetName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestListJobsPaginateTypeDef](./type_defs.md#listjobsrequestlistjobspaginatetypedef) 
## ListProjectsPaginator

Type annotations and code completion for `#!python session.client("databrew").get_paginator("list_projects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListProjects)

```python title="Usage example"
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
## ListRecipeVersionsPaginator

Type annotations and code completion for `#!python session.client("databrew").get_paginator("list_recipe_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRecipeVersions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_databrew.paginator import ListRecipeVersionsPaginator

session = Session()

session = get_session()
async with session.client("databrew") as client:  # (1)
    paginator: ListRecipeVersionsPaginator = client.get_paginator("list_recipe_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecipeVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueDataBrewClient](./client.md)
2. paginator: [ListRecipeVersionsPaginator](./paginators.md#listrecipeversionspaginator)
3. item: [:material-code-braces: ListRecipeVersionsResponseTypeDef](./type_defs.md#listrecipeversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRecipeVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Name: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRecipeVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRecipeVersionsResponseTypeDef](./type_defs.md#listrecipeversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef = {  # (1)
    "Name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef](./type_defs.md#listrecipeversionsrequestlistrecipeversionspaginatetypedef) 
## ListRecipesPaginator

Type annotations and code completion for `#!python session.client("databrew").get_paginator("list_recipes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRecipes)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_databrew.paginator import ListRecipesPaginator

session = Session()

session = get_session()
async with session.client("databrew") as client:  # (1)
    paginator: ListRecipesPaginator = client.get_paginator("list_recipes")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecipesResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueDataBrewClient](./client.md)
2. paginator: [ListRecipesPaginator](./paginators.md#listrecipespaginator)
3. item: [:material-code-braces: ListRecipesResponseTypeDef](./type_defs.md#listrecipesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRecipesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    RecipeVersion: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRecipesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRecipesResponseTypeDef](./type_defs.md#listrecipesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRecipesRequestListRecipesPaginateTypeDef = {  # (1)
    "RecipeVersion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecipesRequestListRecipesPaginateTypeDef](./type_defs.md#listrecipesrequestlistrecipespaginatetypedef) 
## ListRulesetsPaginator

Type annotations and code completion for `#!python session.client("databrew").get_paginator("list_rulesets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRulesets)

```python title="Usage example"
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

```python title="Method definition"
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


```python title="Usage example with kwargs"
kwargs: ListRulesetsRequestListRulesetsPaginateTypeDef = {  # (1)
    "TargetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRulesetsRequestListRulesetsPaginateTypeDef](./type_defs.md#listrulesetsrequestlistrulesetspaginatetypedef) 
## ListSchedulesPaginator

Type annotations and code completion for `#!python session.client("databrew").get_paginator("list_schedules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListSchedules)

```python title="Usage example"
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

```python title="Method definition"
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


```python title="Usage example with kwargs"
kwargs: ListSchedulesRequestListSchedulesPaginateTypeDef = {  # (1)
    "JobName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchedulesRequestListSchedulesPaginateTypeDef](./type_defs.md#listschedulesrequestlistschedulespaginatetypedef) 
