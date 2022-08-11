# Paginators

> [Index](../README.md) > [Connect](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Connect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
    type annotations stubs module [types-aiobotocore-connect](https://pypi.org/project/types-aiobotocore-connect/).

## GetMetricDataPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("get_metric_data")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.GetMetricData)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import GetMetricDataPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: GetMetricDataPaginator = client.get_paginator("get_metric_data")  # (2)
    async for item in paginator.paginate(...):
        item: GetMetricDataResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [GetMetricDataPaginator](./paginators.md#getmetricdatapaginator)
3. item: [:material-code-braces: GetMetricDataResponseTypeDef](./type_defs.md#getmetricdataresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetMetricDataPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    StartTime: Union[datetime, str],
    EndTime: Union[datetime, str],
    Filters: FiltersTypeDef,  # (1)
    HistoricalMetrics: Sequence[HistoricalMetricTypeDef],  # (2)
    Groupings: Sequence[GroupingType] = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AsyncIterator[GetMetricDataResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef) 
2. See [:material-code-braces: HistoricalMetricTypeDef](./type_defs.md#historicalmetrictypedef) 
3. See [:material-code-brackets: GroupingType](./literals.md#groupingtype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: GetMetricDataResponseTypeDef](./type_defs.md#getmetricdataresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetMetricDataRequestGetMetricDataPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "StartTime": ...,
    "EndTime": ...,
    "Filters": ...,
    "HistoricalMetrics": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetMetricDataRequestGetMetricDataPaginateTypeDef](./type_defs.md#getmetricdatarequestgetmetricdatapaginatetypedef) 
## ListAgentStatusesPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_agent_statuses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListAgentStatuses)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListAgentStatusesPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListAgentStatusesPaginator = client.get_paginator("list_agent_statuses")  # (2)
    async for item in paginator.paginate(...):
        item: ListAgentStatusResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListAgentStatusesPaginator](./paginators.md#listagentstatusespaginator)
3. item: [:material-code-braces: ListAgentStatusResponseTypeDef](./type_defs.md#listagentstatusresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAgentStatusesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    AgentStatusTypes: Sequence[AgentStatusTypeType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListAgentStatusResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AgentStatusTypeType](./literals.md#agentstatustypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAgentStatusResponseTypeDef](./type_defs.md#listagentstatusresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAgentStatusRequestListAgentStatusesPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAgentStatusRequestListAgentStatusesPaginateTypeDef](./type_defs.md#listagentstatusrequestlistagentstatusespaginatetypedef) 
## ListApprovedOriginsPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_approved_origins")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListApprovedOrigins)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListApprovedOriginsPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListApprovedOriginsPaginator = client.get_paginator("list_approved_origins")  # (2)
    async for item in paginator.paginate(...):
        item: ListApprovedOriginsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListApprovedOriginsPaginator](./paginators.md#listapprovedoriginspaginator)
3. item: [:material-code-braces: ListApprovedOriginsResponseTypeDef](./type_defs.md#listapprovedoriginsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListApprovedOriginsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListApprovedOriginsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListApprovedOriginsResponseTypeDef](./type_defs.md#listapprovedoriginsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef](./type_defs.md#listapprovedoriginsrequestlistapprovedoriginspaginatetypedef) 
## ListBotsPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_bots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListBots)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListBotsPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListBotsPaginator = client.get_paginator("list_bots")  # (2)
    async for item in paginator.paginate(...):
        item: ListBotsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListBotsPaginator](./paginators.md#listbotspaginator)
3. item: [:material-code-braces: ListBotsResponseTypeDef](./type_defs.md#listbotsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListBotsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    LexVersion: LexVersionType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListBotsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: LexVersionType](./literals.md#lexversiontype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListBotsResponseTypeDef](./type_defs.md#listbotsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListBotsRequestListBotsPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "LexVersion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBotsRequestListBotsPaginateTypeDef](./type_defs.md#listbotsrequestlistbotspaginatetypedef) 
## ListContactFlowModulesPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_contact_flow_modules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactFlowModules)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListContactFlowModulesPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListContactFlowModulesPaginator = client.get_paginator("list_contact_flow_modules")  # (2)
    async for item in paginator.paginate(...):
        item: ListContactFlowModulesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListContactFlowModulesPaginator](./paginators.md#listcontactflowmodulespaginator)
3. item: [:material-code-braces: ListContactFlowModulesResponseTypeDef](./type_defs.md#listcontactflowmodulesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListContactFlowModulesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    ContactFlowModuleState: ContactFlowModuleStateType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListContactFlowModulesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ContactFlowModuleStateType](./literals.md#contactflowmodulestatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListContactFlowModulesResponseTypeDef](./type_defs.md#listcontactflowmodulesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef](./type_defs.md#listcontactflowmodulesrequestlistcontactflowmodulespaginatetypedef) 
## ListContactFlowsPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_contact_flows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactFlows)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListContactFlowsPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListContactFlowsPaginator = client.get_paginator("list_contact_flows")  # (2)
    async for item in paginator.paginate(...):
        item: ListContactFlowsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListContactFlowsPaginator](./paginators.md#listcontactflowspaginator)
3. item: [:material-code-braces: ListContactFlowsResponseTypeDef](./type_defs.md#listcontactflowsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListContactFlowsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    ContactFlowTypes: Sequence[ContactFlowTypeType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListContactFlowsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ContactFlowTypeType](./literals.md#contactflowtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListContactFlowsResponseTypeDef](./type_defs.md#listcontactflowsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListContactFlowsRequestListContactFlowsPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListContactFlowsRequestListContactFlowsPaginateTypeDef](./type_defs.md#listcontactflowsrequestlistcontactflowspaginatetypedef) 
## ListContactReferencesPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_contact_references")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactReferences)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListContactReferencesPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListContactReferencesPaginator = client.get_paginator("list_contact_references")  # (2)
    async for item in paginator.paginate(...):
        item: ListContactReferencesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListContactReferencesPaginator](./paginators.md#listcontactreferencespaginator)
3. item: [:material-code-braces: ListContactReferencesResponseTypeDef](./type_defs.md#listcontactreferencesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListContactReferencesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    ReferenceTypes: Sequence[ReferenceTypeType],  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListContactReferencesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ReferenceTypeType](./literals.md#referencetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListContactReferencesResponseTypeDef](./type_defs.md#listcontactreferencesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListContactReferencesRequestListContactReferencesPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
    "ReferenceTypes": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListContactReferencesRequestListContactReferencesPaginateTypeDef](./type_defs.md#listcontactreferencesrequestlistcontactreferencespaginatetypedef) 
## ListDefaultVocabulariesPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_default_vocabularies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListDefaultVocabularies)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListDefaultVocabulariesPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListDefaultVocabulariesPaginator = client.get_paginator("list_default_vocabularies")  # (2)
    async for item in paginator.paginate(...):
        item: ListDefaultVocabulariesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListDefaultVocabulariesPaginator](./paginators.md#listdefaultvocabulariespaginator)
3. item: [:material-code-braces: ListDefaultVocabulariesResponseTypeDef](./type_defs.md#listdefaultvocabulariesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDefaultVocabulariesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    LanguageCode: VocabularyLanguageCodeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListDefaultVocabulariesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDefaultVocabulariesResponseTypeDef](./type_defs.md#listdefaultvocabulariesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef](./type_defs.md#listdefaultvocabulariesrequestlistdefaultvocabulariespaginatetypedef) 
## ListHoursOfOperationsPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_hours_of_operations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListHoursOfOperations)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListHoursOfOperationsPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListHoursOfOperationsPaginator = client.get_paginator("list_hours_of_operations")  # (2)
    async for item in paginator.paginate(...):
        item: ListHoursOfOperationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListHoursOfOperationsPaginator](./paginators.md#listhoursofoperationspaginator)
3. item: [:material-code-braces: ListHoursOfOperationsResponseTypeDef](./type_defs.md#listhoursofoperationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListHoursOfOperationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListHoursOfOperationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListHoursOfOperationsResponseTypeDef](./type_defs.md#listhoursofoperationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef](./type_defs.md#listhoursofoperationsrequestlisthoursofoperationspaginatetypedef) 
## ListInstanceAttributesPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_instance_attributes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstanceAttributes)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListInstanceAttributesPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListInstanceAttributesPaginator = client.get_paginator("list_instance_attributes")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstanceAttributesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListInstanceAttributesPaginator](./paginators.md#listinstanceattributespaginator)
3. item: [:material-code-braces: ListInstanceAttributesResponseTypeDef](./type_defs.md#listinstanceattributesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListInstanceAttributesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListInstanceAttributesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInstanceAttributesResponseTypeDef](./type_defs.md#listinstanceattributesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef](./type_defs.md#listinstanceattributesrequestlistinstanceattributespaginatetypedef) 
## ListInstanceStorageConfigsPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_instance_storage_configs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstanceStorageConfigs)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListInstanceStorageConfigsPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListInstanceStorageConfigsPaginator = client.get_paginator("list_instance_storage_configs")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstanceStorageConfigsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListInstanceStorageConfigsPaginator](./paginators.md#listinstancestorageconfigspaginator)
3. item: [:material-code-braces: ListInstanceStorageConfigsResponseTypeDef](./type_defs.md#listinstancestorageconfigsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListInstanceStorageConfigsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    ResourceType: InstanceStorageResourceTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListInstanceStorageConfigsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: InstanceStorageResourceTypeType](./literals.md#instancestorageresourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListInstanceStorageConfigsResponseTypeDef](./type_defs.md#listinstancestorageconfigsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "ResourceType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef](./type_defs.md#listinstancestorageconfigsrequestlistinstancestorageconfigspaginatetypedef) 
## ListInstancesPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstances)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListInstancesPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListInstancesPaginator = client.get_paginator("list_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstancesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListInstancesPaginator](./paginators.md#listinstancespaginator)
3. item: [:material-code-braces: ListInstancesResponseTypeDef](./type_defs.md#listinstancesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListInstancesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListInstancesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInstancesResponseTypeDef](./type_defs.md#listinstancesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListInstancesRequestListInstancesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstancesRequestListInstancesPaginateTypeDef](./type_defs.md#listinstancesrequestlistinstancespaginatetypedef) 
## ListIntegrationAssociationsPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_integration_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListIntegrationAssociations)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListIntegrationAssociationsPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListIntegrationAssociationsPaginator = client.get_paginator("list_integration_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListIntegrationAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListIntegrationAssociationsPaginator](./paginators.md#listintegrationassociationspaginator)
3. item: [:material-code-braces: ListIntegrationAssociationsResponseTypeDef](./type_defs.md#listintegrationassociationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListIntegrationAssociationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    IntegrationType: IntegrationTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListIntegrationAssociationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListIntegrationAssociationsResponseTypeDef](./type_defs.md#listintegrationassociationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef](./type_defs.md#listintegrationassociationsrequestlistintegrationassociationspaginatetypedef) 
## ListLambdaFunctionsPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_lambda_functions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListLambdaFunctions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListLambdaFunctionsPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListLambdaFunctionsPaginator = client.get_paginator("list_lambda_functions")  # (2)
    async for item in paginator.paginate(...):
        item: ListLambdaFunctionsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListLambdaFunctionsPaginator](./paginators.md#listlambdafunctionspaginator)
3. item: [:material-code-braces: ListLambdaFunctionsResponseTypeDef](./type_defs.md#listlambdafunctionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListLambdaFunctionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListLambdaFunctionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListLambdaFunctionsResponseTypeDef](./type_defs.md#listlambdafunctionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef](./type_defs.md#listlambdafunctionsrequestlistlambdafunctionspaginatetypedef) 
## ListLexBotsPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_lex_bots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListLexBots)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListLexBotsPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListLexBotsPaginator = client.get_paginator("list_lex_bots")  # (2)
    async for item in paginator.paginate(...):
        item: ListLexBotsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListLexBotsPaginator](./paginators.md#listlexbotspaginator)
3. item: [:material-code-braces: ListLexBotsResponseTypeDef](./type_defs.md#listlexbotsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListLexBotsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListLexBotsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListLexBotsResponseTypeDef](./type_defs.md#listlexbotsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListLexBotsRequestListLexBotsPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLexBotsRequestListLexBotsPaginateTypeDef](./type_defs.md#listlexbotsrequestlistlexbotspaginatetypedef) 
## ListPhoneNumbersPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_phone_numbers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPhoneNumbers)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListPhoneNumbersPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListPhoneNumbersPaginator = client.get_paginator("list_phone_numbers")  # (2)
    async for item in paginator.paginate(...):
        item: ListPhoneNumbersResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListPhoneNumbersPaginator](./paginators.md#listphonenumberspaginator)
3. item: [:material-code-braces: ListPhoneNumbersResponseTypeDef](./type_defs.md#listphonenumbersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPhoneNumbersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,  # (1)
    PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListPhoneNumbersResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
2. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListPhoneNumbersResponseTypeDef](./type_defs.md#listphonenumbersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef](./type_defs.md#listphonenumbersrequestlistphonenumberspaginatetypedef) 
## ListPromptsPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_prompts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPrompts)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListPromptsPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListPromptsPaginator = client.get_paginator("list_prompts")  # (2)
    async for item in paginator.paginate(...):
        item: ListPromptsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListPromptsPaginator](./paginators.md#listpromptspaginator)
3. item: [:material-code-braces: ListPromptsResponseTypeDef](./type_defs.md#listpromptsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPromptsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPromptsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPromptsResponseTypeDef](./type_defs.md#listpromptsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPromptsRequestListPromptsPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPromptsRequestListPromptsPaginateTypeDef](./type_defs.md#listpromptsrequestlistpromptspaginatetypedef) 
## ListQueueQuickConnectsPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_queue_quick_connects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQueueQuickConnects)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListQueueQuickConnectsPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListQueueQuickConnectsPaginator = client.get_paginator("list_queue_quick_connects")  # (2)
    async for item in paginator.paginate(...):
        item: ListQueueQuickConnectsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListQueueQuickConnectsPaginator](./paginators.md#listqueuequickconnectspaginator)
3. item: [:material-code-braces: ListQueueQuickConnectsResponseTypeDef](./type_defs.md#listqueuequickconnectsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListQueueQuickConnectsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    QueueId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListQueueQuickConnectsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListQueueQuickConnectsResponseTypeDef](./type_defs.md#listqueuequickconnectsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "QueueId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef](./type_defs.md#listqueuequickconnectsrequestlistqueuequickconnectspaginatetypedef) 
## ListQueuesPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_queues")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQueues)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListQueuesPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListQueuesPaginator = client.get_paginator("list_queues")  # (2)
    async for item in paginator.paginate(...):
        item: ListQueuesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListQueuesPaginator](./paginators.md#listqueuespaginator)
3. item: [:material-code-braces: ListQueuesResponseTypeDef](./type_defs.md#listqueuesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListQueuesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    QueueTypes: Sequence[QueueTypeType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListQueuesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: QueueTypeType](./literals.md#queuetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListQueuesResponseTypeDef](./type_defs.md#listqueuesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListQueuesRequestListQueuesPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListQueuesRequestListQueuesPaginateTypeDef](./type_defs.md#listqueuesrequestlistqueuespaginatetypedef) 
## ListQuickConnectsPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_quick_connects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQuickConnects)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListQuickConnectsPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListQuickConnectsPaginator = client.get_paginator("list_quick_connects")  # (2)
    async for item in paginator.paginate(...):
        item: ListQuickConnectsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListQuickConnectsPaginator](./paginators.md#listquickconnectspaginator)
3. item: [:material-code-braces: ListQuickConnectsResponseTypeDef](./type_defs.md#listquickconnectsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListQuickConnectsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    QuickConnectTypes: Sequence[QuickConnectTypeType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListQuickConnectsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: QuickConnectTypeType](./literals.md#quickconnecttypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListQuickConnectsResponseTypeDef](./type_defs.md#listquickconnectsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListQuickConnectsRequestListQuickConnectsPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListQuickConnectsRequestListQuickConnectsPaginateTypeDef](./type_defs.md#listquickconnectsrequestlistquickconnectspaginatetypedef) 
## ListRoutingProfileQueuesPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_routing_profile_queues")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRoutingProfileQueues)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListRoutingProfileQueuesPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListRoutingProfileQueuesPaginator = client.get_paginator("list_routing_profile_queues")  # (2)
    async for item in paginator.paginate(...):
        item: ListRoutingProfileQueuesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListRoutingProfileQueuesPaginator](./paginators.md#listroutingprofilequeuespaginator)
3. item: [:material-code-braces: ListRoutingProfileQueuesResponseTypeDef](./type_defs.md#listroutingprofilequeuesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRoutingProfileQueuesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    RoutingProfileId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRoutingProfileQueuesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRoutingProfileQueuesResponseTypeDef](./type_defs.md#listroutingprofilequeuesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "RoutingProfileId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef](./type_defs.md#listroutingprofilequeuesrequestlistroutingprofilequeuespaginatetypedef) 
## ListRoutingProfilesPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_routing_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRoutingProfiles)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListRoutingProfilesPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListRoutingProfilesPaginator = client.get_paginator("list_routing_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListRoutingProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListRoutingProfilesPaginator](./paginators.md#listroutingprofilespaginator)
3. item: [:material-code-braces: ListRoutingProfilesResponseTypeDef](./type_defs.md#listroutingprofilesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRoutingProfilesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRoutingProfilesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRoutingProfilesResponseTypeDef](./type_defs.md#listroutingprofilesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef](./type_defs.md#listroutingprofilesrequestlistroutingprofilespaginatetypedef) 
## ListSecurityKeysPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_security_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityKeys)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListSecurityKeysPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListSecurityKeysPaginator = client.get_paginator("list_security_keys")  # (2)
    async for item in paginator.paginate(...):
        item: ListSecurityKeysResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListSecurityKeysPaginator](./paginators.md#listsecuritykeyspaginator)
3. item: [:material-code-braces: ListSecurityKeysResponseTypeDef](./type_defs.md#listsecuritykeysresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSecurityKeysPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSecurityKeysResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSecurityKeysResponseTypeDef](./type_defs.md#listsecuritykeysresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSecurityKeysRequestListSecurityKeysPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSecurityKeysRequestListSecurityKeysPaginateTypeDef](./type_defs.md#listsecuritykeysrequestlistsecuritykeyspaginatetypedef) 
## ListSecurityProfilePermissionsPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_security_profile_permissions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityProfilePermissions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListSecurityProfilePermissionsPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListSecurityProfilePermissionsPaginator = client.get_paginator("list_security_profile_permissions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSecurityProfilePermissionsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListSecurityProfilePermissionsPaginator](./paginators.md#listsecurityprofilepermissionspaginator)
3. item: [:material-code-braces: ListSecurityProfilePermissionsResponseTypeDef](./type_defs.md#listsecurityprofilepermissionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSecurityProfilePermissionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    SecurityProfileId: str,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSecurityProfilePermissionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSecurityProfilePermissionsResponseTypeDef](./type_defs.md#listsecurityprofilepermissionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef = {  # (1)
    "SecurityProfileId": ...,
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef](./type_defs.md#listsecurityprofilepermissionsrequestlistsecurityprofilepermissionspaginatetypedef) 
## ListSecurityProfilesPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_security_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityProfiles)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListSecurityProfilesPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListSecurityProfilesPaginator = client.get_paginator("list_security_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListSecurityProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListSecurityProfilesPaginator](./paginators.md#listsecurityprofilespaginator)
3. item: [:material-code-braces: ListSecurityProfilesResponseTypeDef](./type_defs.md#listsecurityprofilesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSecurityProfilesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSecurityProfilesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSecurityProfilesResponseTypeDef](./type_defs.md#listsecurityprofilesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef](./type_defs.md#listsecurityprofilesrequestlistsecurityprofilespaginatetypedef) 
## ListUseCasesPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_use_cases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUseCases)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListUseCasesPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListUseCasesPaginator = client.get_paginator("list_use_cases")  # (2)
    async for item in paginator.paginate(...):
        item: ListUseCasesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListUseCasesPaginator](./paginators.md#listusecasespaginator)
3. item: [:material-code-braces: ListUseCasesResponseTypeDef](./type_defs.md#listusecasesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUseCasesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    IntegrationAssociationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListUseCasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUseCasesResponseTypeDef](./type_defs.md#listusecasesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListUseCasesRequestListUseCasesPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "IntegrationAssociationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUseCasesRequestListUseCasesPaginateTypeDef](./type_defs.md#listusecasesrequestlistusecasespaginatetypedef) 
## ListUserHierarchyGroupsPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_user_hierarchy_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUserHierarchyGroups)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListUserHierarchyGroupsPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListUserHierarchyGroupsPaginator = client.get_paginator("list_user_hierarchy_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListUserHierarchyGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListUserHierarchyGroupsPaginator](./paginators.md#listuserhierarchygroupspaginator)
3. item: [:material-code-braces: ListUserHierarchyGroupsResponseTypeDef](./type_defs.md#listuserhierarchygroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUserHierarchyGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListUserHierarchyGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUserHierarchyGroupsResponseTypeDef](./type_defs.md#listuserhierarchygroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef](./type_defs.md#listuserhierarchygroupsrequestlistuserhierarchygroupspaginatetypedef) 
## ListUsersPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("list_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUsers)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import ListUsersPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: ListUsersPaginator = client.get_paginator("list_users")  # (2)
    async for item in paginator.paginate(...):
        item: ListUsersResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListUsersPaginator](./paginators.md#listuserspaginator)
3. item: [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUsersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListUsersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListUsersRequestListUsersPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestListUsersPaginateTypeDef](./type_defs.md#listusersrequestlistuserspaginatetypedef) 
## SearchVocabulariesPaginator

Type annotations and code completion for `#!python session.client("connect").get_paginator("search_vocabularies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchVocabularies)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_connect.paginator import SearchVocabulariesPaginator

session = Session()

session = get_session()
async with session.client("connect") as client:  # (1)
    paginator: SearchVocabulariesPaginator = client.get_paginator("search_vocabularies")  # (2)
    async for item in paginator.paginate(...):
        item: SearchVocabulariesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [SearchVocabulariesPaginator](./paginators.md#searchvocabulariespaginator)
3. item: [:material-code-braces: SearchVocabulariesResponseTypeDef](./type_defs.md#searchvocabulariesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchVocabulariesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceId: str,
    State: VocabularyStateType = ...,  # (1)
    NameStartsWith: str = ...,
    LanguageCode: VocabularyLanguageCodeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[SearchVocabulariesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
2. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: SearchVocabulariesResponseTypeDef](./type_defs.md#searchvocabulariesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SearchVocabulariesRequestSearchVocabulariesPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchVocabulariesRequestSearchVocabulariesPaginateTypeDef](./type_defs.md#searchvocabulariesrequestsearchvocabulariespaginatetypedef) 
