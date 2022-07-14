# Paginators

> [Index](../README.md) > [Batch](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Batch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
    type annotations stubs module [types-aiobotocore-batch](https://pypi.org/project/types-aiobotocore-batch/).

## DescribeComputeEnvironmentsPaginator

Type annotations and code completion for `#!python session.client("batch").get_paginator("describe_compute_environments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeComputeEnvironments)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_batch.paginator import DescribeComputeEnvironmentsPaginator

session = Session()

session = get_session()
async with session.client("batch") as client:  # (1)
    paginator: DescribeComputeEnvironmentsPaginator = client.get_paginator("describe_compute_environments")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeComputeEnvironmentsResponseTypeDef
        print(item)  # (3)
```

1. client: [BatchClient](./client.md)
2. paginator: [DescribeComputeEnvironmentsPaginator](./paginators.md#describecomputeenvironmentspaginator)
3. item: [:material-code-braces: DescribeComputeEnvironmentsResponseTypeDef](./type_defs.md#describecomputeenvironmentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeComputeEnvironmentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    computeEnvironments: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeComputeEnvironmentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeComputeEnvironmentsResponseTypeDef](./type_defs.md#describecomputeenvironmentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef = {  # (1)
    "computeEnvironments": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef](./type_defs.md#describecomputeenvironmentsrequestdescribecomputeenvironmentspaginatetypedef) 
## DescribeJobDefinitionsPaginator

Type annotations and code completion for `#!python session.client("batch").get_paginator("describe_job_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobDefinitions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_batch.paginator import DescribeJobDefinitionsPaginator

session = Session()

session = get_session()
async with session.client("batch") as client:  # (1)
    paginator: DescribeJobDefinitionsPaginator = client.get_paginator("describe_job_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeJobDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [BatchClient](./client.md)
2. paginator: [DescribeJobDefinitionsPaginator](./paginators.md#describejobdefinitionspaginator)
3. item: [:material-code-braces: DescribeJobDefinitionsResponseTypeDef](./type_defs.md#describejobdefinitionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeJobDefinitionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    jobDefinitions: Sequence[str] = ...,
    jobDefinitionName: str = ...,
    status: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeJobDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeJobDefinitionsResponseTypeDef](./type_defs.md#describejobdefinitionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef = {  # (1)
    "jobDefinitions": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef](./type_defs.md#describejobdefinitionsrequestdescribejobdefinitionspaginatetypedef) 
## DescribeJobQueuesPaginator

Type annotations and code completion for `#!python session.client("batch").get_paginator("describe_job_queues")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobQueues)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_batch.paginator import DescribeJobQueuesPaginator

session = Session()

session = get_session()
async with session.client("batch") as client:  # (1)
    paginator: DescribeJobQueuesPaginator = client.get_paginator("describe_job_queues")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeJobQueuesResponseTypeDef
        print(item)  # (3)
```

1. client: [BatchClient](./client.md)
2. paginator: [DescribeJobQueuesPaginator](./paginators.md#describejobqueuespaginator)
3. item: [:material-code-braces: DescribeJobQueuesResponseTypeDef](./type_defs.md#describejobqueuesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeJobQueuesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    jobQueues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeJobQueuesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeJobQueuesResponseTypeDef](./type_defs.md#describejobqueuesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef = {  # (1)
    "jobQueues": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef](./type_defs.md#describejobqueuesrequestdescribejobqueuespaginatetypedef) 
## ListJobsPaginator

Type annotations and code completion for `#!python session.client("batch").get_paginator("list_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListJobs)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_batch.paginator import ListJobsPaginator

session = Session()

session = get_session()
async with session.client("batch") as client:  # (1)
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [BatchClient](./client.md)
2. paginator: [ListJobsPaginator](./paginators.md#listjobspaginator)
3. item: [:material-code-braces: ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    jobQueue: str = ...,
    arrayJobId: str = ...,
    multiNodeJobId: str = ...,
    jobStatus: JobStatusType = ...,  # (1)
    filters: Sequence[KeyValuesPairTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListJobsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: KeyValuesPairTypeDef](./type_defs.md#keyvaluespairtypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListJobsRequestListJobsPaginateTypeDef = {  # (1)
    "jobQueue": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestListJobsPaginateTypeDef](./type_defs.md#listjobsrequestlistjobspaginatetypedef) 
## ListSchedulingPoliciesPaginator

Type annotations and code completion for `#!python session.client("batch").get_paginator("list_scheduling_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListSchedulingPolicies)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_batch.paginator import ListSchedulingPoliciesPaginator

session = Session()

session = get_session()
async with session.client("batch") as client:  # (1)
    paginator: ListSchedulingPoliciesPaginator = client.get_paginator("list_scheduling_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListSchedulingPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [BatchClient](./client.md)
2. paginator: [ListSchedulingPoliciesPaginator](./paginators.md#listschedulingpoliciespaginator)
3. item: [:material-code-braces: ListSchedulingPoliciesResponseTypeDef](./type_defs.md#listschedulingpoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSchedulingPoliciesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSchedulingPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSchedulingPoliciesResponseTypeDef](./type_defs.md#listschedulingpoliciesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef](./type_defs.md#listschedulingpoliciesrequestlistschedulingpoliciespaginatetypedef) 
