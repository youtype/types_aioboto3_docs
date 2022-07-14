# Paginators

> [Index](../README.md) > [IoTThingsGraph](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [IoTThingsGraph](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
    type annotations stubs module [types-aiobotocore-iotthingsgraph](https://pypi.org/project/types-aiobotocore-iotthingsgraph/).

## GetFlowTemplateRevisionsPaginator

Type annotations and code completion for `#!python session.client("iotthingsgraph").get_paginator("get_flow_template_revisions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetFlowTemplateRevisions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iotthingsgraph.paginator import GetFlowTemplateRevisionsPaginator

session = Session()

session = get_session()
async with session.client("iotthingsgraph") as client:  # (1)
    paginator: GetFlowTemplateRevisionsPaginator = client.get_paginator("get_flow_template_revisions")  # (2)
    async for item in paginator.paginate(...):
        item: GetFlowTemplateRevisionsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTThingsGraphClient](./client.md)
2. paginator: [GetFlowTemplateRevisionsPaginator](./paginators.md#getflowtemplaterevisionspaginator)
3. item: [:material-code-braces: GetFlowTemplateRevisionsResponseTypeDef](./type_defs.md#getflowtemplaterevisionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetFlowTemplateRevisionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    id: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetFlowTemplateRevisionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetFlowTemplateRevisionsResponseTypeDef](./type_defs.md#getflowtemplaterevisionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = {  # (1)
    "id": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef](./type_defs.md#getflowtemplaterevisionsrequestgetflowtemplaterevisionspaginatetypedef) 
## GetSystemTemplateRevisionsPaginator

Type annotations and code completion for `#!python session.client("iotthingsgraph").get_paginator("get_system_template_revisions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetSystemTemplateRevisions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iotthingsgraph.paginator import GetSystemTemplateRevisionsPaginator

session = Session()

session = get_session()
async with session.client("iotthingsgraph") as client:  # (1)
    paginator: GetSystemTemplateRevisionsPaginator = client.get_paginator("get_system_template_revisions")  # (2)
    async for item in paginator.paginate(...):
        item: GetSystemTemplateRevisionsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTThingsGraphClient](./client.md)
2. paginator: [GetSystemTemplateRevisionsPaginator](./paginators.md#getsystemtemplaterevisionspaginator)
3. item: [:material-code-braces: GetSystemTemplateRevisionsResponseTypeDef](./type_defs.md#getsystemtemplaterevisionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetSystemTemplateRevisionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    id: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetSystemTemplateRevisionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetSystemTemplateRevisionsResponseTypeDef](./type_defs.md#getsystemtemplaterevisionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = {  # (1)
    "id": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef](./type_defs.md#getsystemtemplaterevisionsrequestgetsystemtemplaterevisionspaginatetypedef) 
## ListFlowExecutionMessagesPaginator

Type annotations and code completion for `#!python session.client("iotthingsgraph").get_paginator("list_flow_execution_messages")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListFlowExecutionMessages)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iotthingsgraph.paginator import ListFlowExecutionMessagesPaginator

session = Session()

session = get_session()
async with session.client("iotthingsgraph") as client:  # (1)
    paginator: ListFlowExecutionMessagesPaginator = client.get_paginator("list_flow_execution_messages")  # (2)
    async for item in paginator.paginate(...):
        item: ListFlowExecutionMessagesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTThingsGraphClient](./client.md)
2. paginator: [ListFlowExecutionMessagesPaginator](./paginators.md#listflowexecutionmessagespaginator)
3. item: [:material-code-braces: ListFlowExecutionMessagesResponseTypeDef](./type_defs.md#listflowexecutionmessagesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFlowExecutionMessagesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    flowExecutionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListFlowExecutionMessagesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFlowExecutionMessagesResponseTypeDef](./type_defs.md#listflowexecutionmessagesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = {  # (1)
    "flowExecutionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef](./type_defs.md#listflowexecutionmessagesrequestlistflowexecutionmessagespaginatetypedef) 
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.client("iotthingsgraph").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListTagsForResource)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iotthingsgraph.paginator import ListTagsForResourcePaginator

session = Session()

session = get_session()
async with session.client("iotthingsgraph") as client:  # (1)
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsForResourceResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTThingsGraphClient](./client.md)
2. paginator: [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
3. item: [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    resourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTagsForResourceRequestListTagsForResourcePaginateTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestListTagsForResourcePaginateTypeDef](./type_defs.md#listtagsforresourcerequestlisttagsforresourcepaginatetypedef) 
## SearchEntitiesPaginator

Type annotations and code completion for `#!python session.client("iotthingsgraph").get_paginator("search_entities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchEntities)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iotthingsgraph.paginator import SearchEntitiesPaginator

session = Session()

session = get_session()
async with session.client("iotthingsgraph") as client:  # (1)
    paginator: SearchEntitiesPaginator = client.get_paginator("search_entities")  # (2)
    async for item in paginator.paginate(...):
        item: SearchEntitiesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTThingsGraphClient](./client.md)
2. paginator: [SearchEntitiesPaginator](./paginators.md#searchentitiespaginator)
3. item: [:material-code-braces: SearchEntitiesResponseTypeDef](./type_defs.md#searchentitiesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchEntitiesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    entityTypes: Sequence[EntityTypeType],  # (1)
    filters: Sequence[EntityFilterTypeDef] = ...,  # (2)
    namespaceVersion: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[SearchEntitiesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
2. See [:material-code-braces: EntityFilterTypeDef](./type_defs.md#entityfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: SearchEntitiesResponseTypeDef](./type_defs.md#searchentitiesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SearchEntitiesRequestSearchEntitiesPaginateTypeDef = {  # (1)
    "entityTypes": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchEntitiesRequestSearchEntitiesPaginateTypeDef](./type_defs.md#searchentitiesrequestsearchentitiespaginatetypedef) 
## SearchFlowExecutionsPaginator

Type annotations and code completion for `#!python session.client("iotthingsgraph").get_paginator("search_flow_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchFlowExecutions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iotthingsgraph.paginator import SearchFlowExecutionsPaginator

session = Session()

session = get_session()
async with session.client("iotthingsgraph") as client:  # (1)
    paginator: SearchFlowExecutionsPaginator = client.get_paginator("search_flow_executions")  # (2)
    async for item in paginator.paginate(...):
        item: SearchFlowExecutionsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTThingsGraphClient](./client.md)
2. paginator: [SearchFlowExecutionsPaginator](./paginators.md#searchflowexecutionspaginator)
3. item: [:material-code-braces: SearchFlowExecutionsResponseTypeDef](./type_defs.md#searchflowexecutionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchFlowExecutionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    systemInstanceId: str,
    flowExecutionId: str = ...,
    startTime: Union[datetime, str] = ...,
    endTime: Union[datetime, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[SearchFlowExecutionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: SearchFlowExecutionsResponseTypeDef](./type_defs.md#searchflowexecutionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = {  # (1)
    "systemInstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef](./type_defs.md#searchflowexecutionsrequestsearchflowexecutionspaginatetypedef) 
## SearchFlowTemplatesPaginator

Type annotations and code completion for `#!python session.client("iotthingsgraph").get_paginator("search_flow_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchFlowTemplates)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iotthingsgraph.paginator import SearchFlowTemplatesPaginator

session = Session()

session = get_session()
async with session.client("iotthingsgraph") as client:  # (1)
    paginator: SearchFlowTemplatesPaginator = client.get_paginator("search_flow_templates")  # (2)
    async for item in paginator.paginate(...):
        item: SearchFlowTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTThingsGraphClient](./client.md)
2. paginator: [SearchFlowTemplatesPaginator](./paginators.md#searchflowtemplatespaginator)
3. item: [:material-code-braces: SearchFlowTemplatesResponseTypeDef](./type_defs.md#searchflowtemplatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchFlowTemplatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filters: Sequence[FlowTemplateFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[SearchFlowTemplatesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FlowTemplateFilterTypeDef](./type_defs.md#flowtemplatefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SearchFlowTemplatesResponseTypeDef](./type_defs.md#searchflowtemplatesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef](./type_defs.md#searchflowtemplatesrequestsearchflowtemplatespaginatetypedef) 
## SearchSystemInstancesPaginator

Type annotations and code completion for `#!python session.client("iotthingsgraph").get_paginator("search_system_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchSystemInstances)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iotthingsgraph.paginator import SearchSystemInstancesPaginator

session = Session()

session = get_session()
async with session.client("iotthingsgraph") as client:  # (1)
    paginator: SearchSystemInstancesPaginator = client.get_paginator("search_system_instances")  # (2)
    async for item in paginator.paginate(...):
        item: SearchSystemInstancesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTThingsGraphClient](./client.md)
2. paginator: [SearchSystemInstancesPaginator](./paginators.md#searchsysteminstancespaginator)
3. item: [:material-code-braces: SearchSystemInstancesResponseTypeDef](./type_defs.md#searchsysteminstancesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchSystemInstancesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filters: Sequence[SystemInstanceFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[SearchSystemInstancesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SystemInstanceFilterTypeDef](./type_defs.md#systeminstancefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SearchSystemInstancesResponseTypeDef](./type_defs.md#searchsysteminstancesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef](./type_defs.md#searchsysteminstancesrequestsearchsysteminstancespaginatetypedef) 
## SearchSystemTemplatesPaginator

Type annotations and code completion for `#!python session.client("iotthingsgraph").get_paginator("search_system_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchSystemTemplates)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iotthingsgraph.paginator import SearchSystemTemplatesPaginator

session = Session()

session = get_session()
async with session.client("iotthingsgraph") as client:  # (1)
    paginator: SearchSystemTemplatesPaginator = client.get_paginator("search_system_templates")  # (2)
    async for item in paginator.paginate(...):
        item: SearchSystemTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTThingsGraphClient](./client.md)
2. paginator: [SearchSystemTemplatesPaginator](./paginators.md#searchsystemtemplatespaginator)
3. item: [:material-code-braces: SearchSystemTemplatesResponseTypeDef](./type_defs.md#searchsystemtemplatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchSystemTemplatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filters: Sequence[SystemTemplateFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[SearchSystemTemplatesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SystemTemplateFilterTypeDef](./type_defs.md#systemtemplatefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SearchSystemTemplatesResponseTypeDef](./type_defs.md#searchsystemtemplatesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef](./type_defs.md#searchsystemtemplatesrequestsearchsystemtemplatespaginatetypedef) 
## SearchThingsPaginator

Type annotations and code completion for `#!python session.client("iotthingsgraph").get_paginator("search_things")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchThings)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iotthingsgraph.paginator import SearchThingsPaginator

session = Session()

session = get_session()
async with session.client("iotthingsgraph") as client:  # (1)
    paginator: SearchThingsPaginator = client.get_paginator("search_things")  # (2)
    async for item in paginator.paginate(...):
        item: SearchThingsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTThingsGraphClient](./client.md)
2. paginator: [SearchThingsPaginator](./paginators.md#searchthingspaginator)
3. item: [:material-code-braces: SearchThingsResponseTypeDef](./type_defs.md#searchthingsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchThingsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    entityId: str,
    namespaceVersion: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[SearchThingsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: SearchThingsResponseTypeDef](./type_defs.md#searchthingsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SearchThingsRequestSearchThingsPaginateTypeDef = {  # (1)
    "entityId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchThingsRequestSearchThingsPaginateTypeDef](./type_defs.md#searchthingsrequestsearchthingspaginatetypedef) 
