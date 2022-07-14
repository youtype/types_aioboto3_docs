# Paginators

> [Index](../README.md) > [EMR](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [EMR](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
    type annotations stubs module [types-aiobotocore-emr](https://pypi.org/project/types-aiobotocore-emr/).

## ListBootstrapActionsPaginator

Type annotations and code completion for `#!python session.client("emr").get_paginator("list_bootstrap_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListBootstrapActions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_emr.paginator import ListBootstrapActionsPaginator

session = Session()

session = get_session()
async with session.client("emr") as client:  # (1)
    paginator: ListBootstrapActionsPaginator = client.get_paginator("list_bootstrap_actions")  # (2)
    async for item in paginator.paginate(...):
        item: ListBootstrapActionsOutputTypeDef
        print(item)  # (3)
```

1. client: [EMRClient](./client.md)
2. paginator: [ListBootstrapActionsPaginator](./paginators.md#listbootstrapactionspaginator)
3. item: [:material-code-braces: ListBootstrapActionsOutputTypeDef](./type_defs.md#listbootstrapactionsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListBootstrapActionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ClusterId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListBootstrapActionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBootstrapActionsOutputTypeDef](./type_defs.md#listbootstrapactionsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef = {  # (1)
    "ClusterId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef](./type_defs.md#listbootstrapactionsinputlistbootstrapactionspaginatetypedef) 
## ListClustersPaginator

Type annotations and code completion for `#!python session.client("emr").get_paginator("list_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListClusters)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_emr.paginator import ListClustersPaginator

session = Session()

session = get_session()
async with session.client("emr") as client:  # (1)
    paginator: ListClustersPaginator = client.get_paginator("list_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: ListClustersOutputTypeDef
        print(item)  # (3)
```

1. client: [EMRClient](./client.md)
2. paginator: [ListClustersPaginator](./paginators.md#listclusterspaginator)
3. item: [:material-code-braces: ListClustersOutputTypeDef](./type_defs.md#listclustersoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListClustersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    CreatedAfter: Union[datetime, str] = ...,
    CreatedBefore: Union[datetime, str] = ...,
    ClusterStates: Sequence[ClusterStateType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListClustersOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ClusterStateType](./literals.md#clusterstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListClustersOutputTypeDef](./type_defs.md#listclustersoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListClustersInputListClustersPaginateTypeDef = {  # (1)
    "CreatedAfter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListClustersInputListClustersPaginateTypeDef](./type_defs.md#listclustersinputlistclusterspaginatetypedef) 
## ListInstanceFleetsPaginator

Type annotations and code completion for `#!python session.client("emr").get_paginator("list_instance_fleets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstanceFleets)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_emr.paginator import ListInstanceFleetsPaginator

session = Session()

session = get_session()
async with session.client("emr") as client:  # (1)
    paginator: ListInstanceFleetsPaginator = client.get_paginator("list_instance_fleets")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstanceFleetsOutputTypeDef
        print(item)  # (3)
```

1. client: [EMRClient](./client.md)
2. paginator: [ListInstanceFleetsPaginator](./paginators.md#listinstancefleetspaginator)
3. item: [:material-code-braces: ListInstanceFleetsOutputTypeDef](./type_defs.md#listinstancefleetsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListInstanceFleetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ClusterId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListInstanceFleetsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInstanceFleetsOutputTypeDef](./type_defs.md#listinstancefleetsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef = {  # (1)
    "ClusterId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef](./type_defs.md#listinstancefleetsinputlistinstancefleetspaginatetypedef) 
## ListInstanceGroupsPaginator

Type annotations and code completion for `#!python session.client("emr").get_paginator("list_instance_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstanceGroups)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_emr.paginator import ListInstanceGroupsPaginator

session = Session()

session = get_session()
async with session.client("emr") as client:  # (1)
    paginator: ListInstanceGroupsPaginator = client.get_paginator("list_instance_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstanceGroupsOutputTypeDef
        print(item)  # (3)
```

1. client: [EMRClient](./client.md)
2. paginator: [ListInstanceGroupsPaginator](./paginators.md#listinstancegroupspaginator)
3. item: [:material-code-braces: ListInstanceGroupsOutputTypeDef](./type_defs.md#listinstancegroupsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListInstanceGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ClusterId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListInstanceGroupsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInstanceGroupsOutputTypeDef](./type_defs.md#listinstancegroupsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef = {  # (1)
    "ClusterId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef](./type_defs.md#listinstancegroupsinputlistinstancegroupspaginatetypedef) 
## ListInstancesPaginator

Type annotations and code completion for `#!python session.client("emr").get_paginator("list_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstances)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_emr.paginator import ListInstancesPaginator

session = Session()

session = get_session()
async with session.client("emr") as client:  # (1)
    paginator: ListInstancesPaginator = client.get_paginator("list_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstancesOutputTypeDef
        print(item)  # (3)
```

1. client: [EMRClient](./client.md)
2. paginator: [ListInstancesPaginator](./paginators.md#listinstancespaginator)
3. item: [:material-code-braces: ListInstancesOutputTypeDef](./type_defs.md#listinstancesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListInstancesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ClusterId: str,
    InstanceGroupId: str = ...,
    InstanceGroupTypes: Sequence[InstanceGroupTypeType] = ...,  # (1)
    InstanceFleetId: str = ...,
    InstanceFleetType: InstanceFleetTypeType = ...,  # (2)
    InstanceStates: Sequence[InstanceStateType] = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AsyncIterator[ListInstancesOutputTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: InstanceGroupTypeType](./literals.md#instancegrouptypetype) 
2. See [:material-code-brackets: InstanceFleetTypeType](./literals.md#instancefleettypetype) 
3. See [:material-code-brackets: InstanceStateType](./literals.md#instancestatetype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListInstancesOutputTypeDef](./type_defs.md#listinstancesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListInstancesInputListInstancesPaginateTypeDef = {  # (1)
    "ClusterId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstancesInputListInstancesPaginateTypeDef](./type_defs.md#listinstancesinputlistinstancespaginatetypedef) 
## ListNotebookExecutionsPaginator

Type annotations and code completion for `#!python session.client("emr").get_paginator("list_notebook_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListNotebookExecutions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_emr.paginator import ListNotebookExecutionsPaginator

session = Session()

session = get_session()
async with session.client("emr") as client:  # (1)
    paginator: ListNotebookExecutionsPaginator = client.get_paginator("list_notebook_executions")  # (2)
    async for item in paginator.paginate(...):
        item: ListNotebookExecutionsOutputTypeDef
        print(item)  # (3)
```

1. client: [EMRClient](./client.md)
2. paginator: [ListNotebookExecutionsPaginator](./paginators.md#listnotebookexecutionspaginator)
3. item: [:material-code-braces: ListNotebookExecutionsOutputTypeDef](./type_defs.md#listnotebookexecutionsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListNotebookExecutionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    EditorId: str = ...,
    Status: NotebookExecutionStatusType = ...,  # (1)
    From: Union[datetime, str] = ...,
    To: Union[datetime, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListNotebookExecutionsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: NotebookExecutionStatusType](./literals.md#notebookexecutionstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListNotebookExecutionsOutputTypeDef](./type_defs.md#listnotebookexecutionsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef = {  # (1)
    "EditorId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef](./type_defs.md#listnotebookexecutionsinputlistnotebookexecutionspaginatetypedef) 
## ListSecurityConfigurationsPaginator

Type annotations and code completion for `#!python session.client("emr").get_paginator("list_security_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListSecurityConfigurations)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_emr.paginator import ListSecurityConfigurationsPaginator

session = Session()

session = get_session()
async with session.client("emr") as client:  # (1)
    paginator: ListSecurityConfigurationsPaginator = client.get_paginator("list_security_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListSecurityConfigurationsOutputTypeDef
        print(item)  # (3)
```

1. client: [EMRClient](./client.md)
2. paginator: [ListSecurityConfigurationsPaginator](./paginators.md#listsecurityconfigurationspaginator)
3. item: [:material-code-braces: ListSecurityConfigurationsOutputTypeDef](./type_defs.md#listsecurityconfigurationsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSecurityConfigurationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSecurityConfigurationsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSecurityConfigurationsOutputTypeDef](./type_defs.md#listsecurityconfigurationsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef](./type_defs.md#listsecurityconfigurationsinputlistsecurityconfigurationspaginatetypedef) 
## ListStepsPaginator

Type annotations and code completion for `#!python session.client("emr").get_paginator("list_steps")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListSteps)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_emr.paginator import ListStepsPaginator

session = Session()

session = get_session()
async with session.client("emr") as client:  # (1)
    paginator: ListStepsPaginator = client.get_paginator("list_steps")  # (2)
    async for item in paginator.paginate(...):
        item: ListStepsOutputTypeDef
        print(item)  # (3)
```

1. client: [EMRClient](./client.md)
2. paginator: [ListStepsPaginator](./paginators.md#liststepspaginator)
3. item: [:material-code-braces: ListStepsOutputTypeDef](./type_defs.md#liststepsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListStepsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ClusterId: str,
    StepStates: Sequence[StepStateType] = ...,  # (1)
    StepIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListStepsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: StepStateType](./literals.md#stepstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListStepsOutputTypeDef](./type_defs.md#liststepsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListStepsInputListStepsPaginateTypeDef = {  # (1)
    "ClusterId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStepsInputListStepsPaginateTypeDef](./type_defs.md#liststepsinputliststepspaginatetypedef) 
## ListStudioSessionMappingsPaginator

Type annotations and code completion for `#!python session.client("emr").get_paginator("list_studio_session_mappings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListStudioSessionMappings)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_emr.paginator import ListStudioSessionMappingsPaginator

session = Session()

session = get_session()
async with session.client("emr") as client:  # (1)
    paginator: ListStudioSessionMappingsPaginator = client.get_paginator("list_studio_session_mappings")  # (2)
    async for item in paginator.paginate(...):
        item: ListStudioSessionMappingsOutputTypeDef
        print(item)  # (3)
```

1. client: [EMRClient](./client.md)
2. paginator: [ListStudioSessionMappingsPaginator](./paginators.md#liststudiosessionmappingspaginator)
3. item: [:material-code-braces: ListStudioSessionMappingsOutputTypeDef](./type_defs.md#liststudiosessionmappingsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListStudioSessionMappingsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    StudioId: str = ...,
    IdentityType: IdentityTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListStudioSessionMappingsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListStudioSessionMappingsOutputTypeDef](./type_defs.md#liststudiosessionmappingsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef = {  # (1)
    "StudioId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef](./type_defs.md#liststudiosessionmappingsinputliststudiosessionmappingspaginatetypedef) 
## ListStudiosPaginator

Type annotations and code completion for `#!python session.client("emr").get_paginator("list_studios")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListStudios)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_emr.paginator import ListStudiosPaginator

session = Session()

session = get_session()
async with session.client("emr") as client:  # (1)
    paginator: ListStudiosPaginator = client.get_paginator("list_studios")  # (2)
    async for item in paginator.paginate(...):
        item: ListStudiosOutputTypeDef
        print(item)  # (3)
```

1. client: [EMRClient](./client.md)
2. paginator: [ListStudiosPaginator](./paginators.md#liststudiospaginator)
3. item: [:material-code-braces: ListStudiosOutputTypeDef](./type_defs.md#liststudiosoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListStudiosPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListStudiosOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListStudiosOutputTypeDef](./type_defs.md#liststudiosoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListStudiosInputListStudiosPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStudiosInputListStudiosPaginateTypeDef](./type_defs.md#liststudiosinputliststudiospaginatetypedef) 
