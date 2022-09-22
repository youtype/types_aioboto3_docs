# Paginators

> [Index](../README.md) > [mgn](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [mgn](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
    type annotations stubs module [types-aiobotocore-mgn](https://pypi.org/project/types-aiobotocore-mgn/).

## DescribeJobLogItemsPaginator

Type annotations and code completion for `#!python session.client("mgn").get_paginator("describe_job_log_items")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobLogItems)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_mgn.paginator import DescribeJobLogItemsPaginator

session = Session()

session = get_session()
async with session.client("mgn") as client:  # (1)
    paginator: DescribeJobLogItemsPaginator = client.get_paginator("describe_job_log_items")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeJobLogItemsResponseTypeDef
        print(item)  # (3)
```

1. client: [mgnClient](./client.md)
2. paginator: [DescribeJobLogItemsPaginator](./paginators.md#describejoblogitemspaginator)
3. item: [:material-code-braces: DescribeJobLogItemsResponseTypeDef](./type_defs.md#describejoblogitemsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeJobLogItemsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    jobID: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeJobLogItemsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeJobLogItemsResponseTypeDef](./type_defs.md#describejoblogitemsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = {  # (1)
    "jobID": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef](./type_defs.md#describejoblogitemsrequestdescribejoblogitemspaginatetypedef) 
## DescribeJobsPaginator

Type annotations and code completion for `#!python session.client("mgn").get_paginator("describe_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobs)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_mgn.paginator import DescribeJobsPaginator

session = Session()

session = get_session()
async with session.client("mgn") as client:  # (1)
    paginator: DescribeJobsPaginator = client.get_paginator("describe_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [mgnClient](./client.md)
2. paginator: [DescribeJobsPaginator](./paginators.md#describejobspaginator)
3. item: [:material-code-braces: DescribeJobsResponseTypeDef](./type_defs.md#describejobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filters: DescribeJobsRequestFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DescribeJobsRequestFiltersTypeDef](./type_defs.md#describejobsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeJobsResponseTypeDef](./type_defs.md#describejobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeJobsRequestDescribeJobsPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeJobsRequestDescribeJobsPaginateTypeDef](./type_defs.md#describejobsrequestdescribejobspaginatetypedef) 
## DescribeLaunchConfigurationTemplatesPaginator

Type annotations and code completion for `#!python session.client("mgn").get_paginator("describe_launch_configuration_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeLaunchConfigurationTemplates)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_mgn.paginator import DescribeLaunchConfigurationTemplatesPaginator

session = Session()

session = get_session()
async with session.client("mgn") as client:  # (1)
    paginator: DescribeLaunchConfigurationTemplatesPaginator = client.get_paginator("describe_launch_configuration_templates")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeLaunchConfigurationTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [mgnClient](./client.md)
2. paginator: [DescribeLaunchConfigurationTemplatesPaginator](./paginators.md#describelaunchconfigurationtemplatespaginator)
3. item: [:material-code-braces: DescribeLaunchConfigurationTemplatesResponseTypeDef](./type_defs.md#describelaunchconfigurationtemplatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeLaunchConfigurationTemplatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    launchConfigurationTemplateIDs: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeLaunchConfigurationTemplatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeLaunchConfigurationTemplatesResponseTypeDef](./type_defs.md#describelaunchconfigurationtemplatesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef = {  # (1)
    "launchConfigurationTemplateIDs": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef](./type_defs.md#describelaunchconfigurationtemplatesrequestdescribelaunchconfigurationtemplatespaginatetypedef) 
## DescribeReplicationConfigurationTemplatesPaginator

Type annotations and code completion for `#!python session.client("mgn").get_paginator("describe_replication_configuration_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeReplicationConfigurationTemplates)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_mgn.paginator import DescribeReplicationConfigurationTemplatesPaginator

session = Session()

session = get_session()
async with session.client("mgn") as client:  # (1)
    paginator: DescribeReplicationConfigurationTemplatesPaginator = client.get_paginator("describe_replication_configuration_templates")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeReplicationConfigurationTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [mgnClient](./client.md)
2. paginator: [DescribeReplicationConfigurationTemplatesPaginator](./paginators.md#describereplicationconfigurationtemplatespaginator)
3. item: [:material-code-braces: DescribeReplicationConfigurationTemplatesResponseTypeDef](./type_defs.md#describereplicationconfigurationtemplatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReplicationConfigurationTemplatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    replicationConfigurationTemplateIDs: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeReplicationConfigurationTemplatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeReplicationConfigurationTemplatesResponseTypeDef](./type_defs.md#describereplicationconfigurationtemplatesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef = {  # (1)
    "replicationConfigurationTemplateIDs": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef](./type_defs.md#describereplicationconfigurationtemplatesrequestdescribereplicationconfigurationtemplatespaginatetypedef) 
## DescribeSourceServersPaginator

Type annotations and code completion for `#!python session.client("mgn").get_paginator("describe_source_servers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeSourceServers)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_mgn.paginator import DescribeSourceServersPaginator

session = Session()

session = get_session()
async with session.client("mgn") as client:  # (1)
    paginator: DescribeSourceServersPaginator = client.get_paginator("describe_source_servers")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSourceServersResponseTypeDef
        print(item)  # (3)
```

1. client: [mgnClient](./client.md)
2. paginator: [DescribeSourceServersPaginator](./paginators.md#describesourceserverspaginator)
3. item: [:material-code-braces: DescribeSourceServersResponseTypeDef](./type_defs.md#describesourceserversresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSourceServersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filters: DescribeSourceServersRequestFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeSourceServersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DescribeSourceServersRequestFiltersTypeDef](./type_defs.md#describesourceserversrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeSourceServersResponseTypeDef](./type_defs.md#describesourceserversresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef](./type_defs.md#describesourceserversrequestdescribesourceserverspaginatetypedef) 
## DescribeVcenterClientsPaginator

Type annotations and code completion for `#!python session.client("mgn").get_paginator("describe_vcenter_clients")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeVcenterClients)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_mgn.paginator import DescribeVcenterClientsPaginator

session = Session()

session = get_session()
async with session.client("mgn") as client:  # (1)
    paginator: DescribeVcenterClientsPaginator = client.get_paginator("describe_vcenter_clients")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeVcenterClientsResponseTypeDef
        print(item)  # (3)
```

1. client: [mgnClient](./client.md)
2. paginator: [DescribeVcenterClientsPaginator](./paginators.md#describevcenterclientspaginator)
3. item: [:material-code-braces: DescribeVcenterClientsResponseTypeDef](./type_defs.md#describevcenterclientsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeVcenterClientsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeVcenterClientsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeVcenterClientsResponseTypeDef](./type_defs.md#describevcenterclientsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef](./type_defs.md#describevcenterclientsrequestdescribevcenterclientspaginatetypedef) 
