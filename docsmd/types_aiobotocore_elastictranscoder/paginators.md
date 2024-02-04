# Paginators

> [Index](../README.md) > [ElasticTranscoder](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ElasticTranscoder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
    type annotations stubs module [types-aiobotocore-elastictranscoder](https://pypi.org/project/types-aiobotocore-elastictranscoder/).

## ListJobsByPipelinePaginator

Type annotations and code completion for `#!python session.client("elastictranscoder").get_paginator("list_jobs_by_pipeline")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByPipeline)

```python
# ListJobsByPipelinePaginator usage example

from aioboto3.session import Session

from types_aiobotocore_elastictranscoder.paginator import ListJobsByPipelinePaginator

session = Session()

session = get_session()
async with session.client("elastictranscoder") as client:  # (1)
    paginator: ListJobsByPipelinePaginator = client.get_paginator("list_jobs_by_pipeline")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobsByPipelineResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [ElasticTranscoderClient](./client.md)
2. paginator: [ListJobsByPipelinePaginator](./paginators.md#listjobsbypipelinepaginator)
3. item: [:material-code-braces: ListJobsByPipelineResponsePaginatorTypeDef](./type_defs.md#listjobsbypipelineresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListJobsByPipelinePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PipelineId: str,
    Ascending: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListJobsByPipelineResponsePaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListJobsByPipelineResponsePaginatorTypeDef](./type_defs.md#listjobsbypipelineresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = {  # (1)
    "PipelineId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef](./type_defs.md#listjobsbypipelinerequestlistjobsbypipelinepaginatetypedef) 
## ListJobsByStatusPaginator

Type annotations and code completion for `#!python session.client("elastictranscoder").get_paginator("list_jobs_by_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByStatus)

```python
# ListJobsByStatusPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_elastictranscoder.paginator import ListJobsByStatusPaginator

session = Session()

session = get_session()
async with session.client("elastictranscoder") as client:  # (1)
    paginator: ListJobsByStatusPaginator = client.get_paginator("list_jobs_by_status")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobsByStatusResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [ElasticTranscoderClient](./client.md)
2. paginator: [ListJobsByStatusPaginator](./paginators.md#listjobsbystatuspaginator)
3. item: [:material-code-braces: ListJobsByStatusResponsePaginatorTypeDef](./type_defs.md#listjobsbystatusresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListJobsByStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Status: str,
    Ascending: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListJobsByStatusResponsePaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListJobsByStatusResponsePaginatorTypeDef](./type_defs.md#listjobsbystatusresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListJobsByStatusRequestListJobsByStatusPaginateTypeDef = {  # (1)
    "Status": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsByStatusRequestListJobsByStatusPaginateTypeDef](./type_defs.md#listjobsbystatusrequestlistjobsbystatuspaginatetypedef) 
## ListPipelinesPaginator

Type annotations and code completion for `#!python session.client("elastictranscoder").get_paginator("list_pipelines")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPipelines)

```python
# ListPipelinesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_elastictranscoder.paginator import ListPipelinesPaginator

session = Session()

session = get_session()
async with session.client("elastictranscoder") as client:  # (1)
    paginator: ListPipelinesPaginator = client.get_paginator("list_pipelines")  # (2)
    async for item in paginator.paginate(...):
        item: ListPipelinesResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [ElasticTranscoderClient](./client.md)
2. paginator: [ListPipelinesPaginator](./paginators.md#listpipelinespaginator)
3. item: [:material-code-braces: ListPipelinesResponsePaginatorTypeDef](./type_defs.md#listpipelinesresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListPipelinesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Ascending: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPipelinesResponsePaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPipelinesResponsePaginatorTypeDef](./type_defs.md#listpipelinesresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPipelinesRequestListPipelinesPaginateTypeDef = {  # (1)
    "Ascending": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPipelinesRequestListPipelinesPaginateTypeDef](./type_defs.md#listpipelinesrequestlistpipelinespaginatetypedef) 
## ListPresetsPaginator

Type annotations and code completion for `#!python session.client("elastictranscoder").get_paginator("list_presets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPresets)

```python
# ListPresetsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_elastictranscoder.paginator import ListPresetsPaginator

session = Session()

session = get_session()
async with session.client("elastictranscoder") as client:  # (1)
    paginator: ListPresetsPaginator = client.get_paginator("list_presets")  # (2)
    async for item in paginator.paginate(...):
        item: ListPresetsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [ElasticTranscoderClient](./client.md)
2. paginator: [ListPresetsPaginator](./paginators.md#listpresetspaginator)
3. item: [:material-code-braces: ListPresetsResponsePaginatorTypeDef](./type_defs.md#listpresetsresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListPresetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Ascending: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPresetsResponsePaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPresetsResponsePaginatorTypeDef](./type_defs.md#listpresetsresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPresetsRequestListPresetsPaginateTypeDef = {  # (1)
    "Ascending": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPresetsRequestListPresetsPaginateTypeDef](./type_defs.md#listpresetsrequestlistpresetspaginatetypedef) 
