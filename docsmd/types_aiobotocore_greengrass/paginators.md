# Paginators

> [Index](../README.md) > [Greengrass](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Greengrass](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
    type annotations stubs module [types-aiobotocore-greengrass](https://pypi.org/project/types-aiobotocore-greengrass/).

## ListBulkDeploymentDetailedReportsPaginator

Type annotations and code completion for `#!python session.client("greengrass").get_paginator("list_bulk_deployment_detailed_reports")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListBulkDeploymentDetailedReports)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrass.paginator import ListBulkDeploymentDetailedReportsPaginator

session = Session()

session = get_session()
async with session.client("greengrass") as client:  # (1)
    paginator: ListBulkDeploymentDetailedReportsPaginator = client.get_paginator("list_bulk_deployment_detailed_reports")  # (2)
    async for item in paginator.paginate(...):
        item: ListBulkDeploymentDetailedReportsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListBulkDeploymentDetailedReportsPaginator](./paginators.md#listbulkdeploymentdetailedreportspaginator)
3. item: [:material-code-braces: ListBulkDeploymentDetailedReportsResponseTypeDef](./type_defs.md#listbulkdeploymentdetailedreportsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListBulkDeploymentDetailedReportsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    BulkDeploymentId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListBulkDeploymentDetailedReportsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBulkDeploymentDetailedReportsResponseTypeDef](./type_defs.md#listbulkdeploymentdetailedreportsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef = {  # (1)
    "BulkDeploymentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef](./type_defs.md#listbulkdeploymentdetailedreportsrequestlistbulkdeploymentdetailedreportspaginatetypedef) 
## ListBulkDeploymentsPaginator

Type annotations and code completion for `#!python session.client("greengrass").get_paginator("list_bulk_deployments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListBulkDeployments)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrass.paginator import ListBulkDeploymentsPaginator

session = Session()

session = get_session()
async with session.client("greengrass") as client:  # (1)
    paginator: ListBulkDeploymentsPaginator = client.get_paginator("list_bulk_deployments")  # (2)
    async for item in paginator.paginate(...):
        item: ListBulkDeploymentsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListBulkDeploymentsPaginator](./paginators.md#listbulkdeploymentspaginator)
3. item: [:material-code-braces: ListBulkDeploymentsResponseTypeDef](./type_defs.md#listbulkdeploymentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListBulkDeploymentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListBulkDeploymentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBulkDeploymentsResponseTypeDef](./type_defs.md#listbulkdeploymentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef](./type_defs.md#listbulkdeploymentsrequestlistbulkdeploymentspaginatetypedef) 
## ListConnectorDefinitionVersionsPaginator

Type annotations and code completion for `#!python session.client("greengrass").get_paginator("list_connector_definition_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListConnectorDefinitionVersions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrass.paginator import ListConnectorDefinitionVersionsPaginator

session = Session()

session = get_session()
async with session.client("greengrass") as client:  # (1)
    paginator: ListConnectorDefinitionVersionsPaginator = client.get_paginator("list_connector_definition_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListConnectorDefinitionVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListConnectorDefinitionVersionsPaginator](./paginators.md#listconnectordefinitionversionspaginator)
3. item: [:material-code-braces: ListConnectorDefinitionVersionsResponseTypeDef](./type_defs.md#listconnectordefinitionversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConnectorDefinitionVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ConnectorDefinitionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListConnectorDefinitionVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListConnectorDefinitionVersionsResponseTypeDef](./type_defs.md#listconnectordefinitionversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef = {  # (1)
    "ConnectorDefinitionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef](./type_defs.md#listconnectordefinitionversionsrequestlistconnectordefinitionversionspaginatetypedef) 
## ListConnectorDefinitionsPaginator

Type annotations and code completion for `#!python session.client("greengrass").get_paginator("list_connector_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListConnectorDefinitions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrass.paginator import ListConnectorDefinitionsPaginator

session = Session()

session = get_session()
async with session.client("greengrass") as client:  # (1)
    paginator: ListConnectorDefinitionsPaginator = client.get_paginator("list_connector_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: ListConnectorDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListConnectorDefinitionsPaginator](./paginators.md#listconnectordefinitionspaginator)
3. item: [:material-code-braces: ListConnectorDefinitionsResponseTypeDef](./type_defs.md#listconnectordefinitionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConnectorDefinitionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListConnectorDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListConnectorDefinitionsResponseTypeDef](./type_defs.md#listconnectordefinitionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef](./type_defs.md#listconnectordefinitionsrequestlistconnectordefinitionspaginatetypedef) 
## ListCoreDefinitionVersionsPaginator

Type annotations and code completion for `#!python session.client("greengrass").get_paginator("list_core_definition_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListCoreDefinitionVersions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrass.paginator import ListCoreDefinitionVersionsPaginator

session = Session()

session = get_session()
async with session.client("greengrass") as client:  # (1)
    paginator: ListCoreDefinitionVersionsPaginator = client.get_paginator("list_core_definition_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListCoreDefinitionVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListCoreDefinitionVersionsPaginator](./paginators.md#listcoredefinitionversionspaginator)
3. item: [:material-code-braces: ListCoreDefinitionVersionsResponseTypeDef](./type_defs.md#listcoredefinitionversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCoreDefinitionVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    CoreDefinitionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCoreDefinitionVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCoreDefinitionVersionsResponseTypeDef](./type_defs.md#listcoredefinitionversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef = {  # (1)
    "CoreDefinitionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef](./type_defs.md#listcoredefinitionversionsrequestlistcoredefinitionversionspaginatetypedef) 
## ListCoreDefinitionsPaginator

Type annotations and code completion for `#!python session.client("greengrass").get_paginator("list_core_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListCoreDefinitions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrass.paginator import ListCoreDefinitionsPaginator

session = Session()

session = get_session()
async with session.client("greengrass") as client:  # (1)
    paginator: ListCoreDefinitionsPaginator = client.get_paginator("list_core_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: ListCoreDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListCoreDefinitionsPaginator](./paginators.md#listcoredefinitionspaginator)
3. item: [:material-code-braces: ListCoreDefinitionsResponseTypeDef](./type_defs.md#listcoredefinitionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCoreDefinitionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCoreDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCoreDefinitionsResponseTypeDef](./type_defs.md#listcoredefinitionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef](./type_defs.md#listcoredefinitionsrequestlistcoredefinitionspaginatetypedef) 
## ListDeploymentsPaginator

Type annotations and code completion for `#!python session.client("greengrass").get_paginator("list_deployments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeployments)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrass.paginator import ListDeploymentsPaginator

session = Session()

session = get_session()
async with session.client("greengrass") as client:  # (1)
    paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeploymentsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListDeploymentsPaginator](./paginators.md#listdeploymentspaginator)
3. item: [:material-code-braces: ListDeploymentsResponseTypeDef](./type_defs.md#listdeploymentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDeploymentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GroupId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDeploymentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDeploymentsResponseTypeDef](./type_defs.md#listdeploymentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDeploymentsRequestListDeploymentsPaginateTypeDef = {  # (1)
    "GroupId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeploymentsRequestListDeploymentsPaginateTypeDef](./type_defs.md#listdeploymentsrequestlistdeploymentspaginatetypedef) 
## ListDeviceDefinitionVersionsPaginator

Type annotations and code completion for `#!python session.client("greengrass").get_paginator("list_device_definition_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeviceDefinitionVersions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrass.paginator import ListDeviceDefinitionVersionsPaginator

session = Session()

session = get_session()
async with session.client("greengrass") as client:  # (1)
    paginator: ListDeviceDefinitionVersionsPaginator = client.get_paginator("list_device_definition_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeviceDefinitionVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListDeviceDefinitionVersionsPaginator](./paginators.md#listdevicedefinitionversionspaginator)
3. item: [:material-code-braces: ListDeviceDefinitionVersionsResponseTypeDef](./type_defs.md#listdevicedefinitionversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDeviceDefinitionVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DeviceDefinitionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDeviceDefinitionVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDeviceDefinitionVersionsResponseTypeDef](./type_defs.md#listdevicedefinitionversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef = {  # (1)
    "DeviceDefinitionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef](./type_defs.md#listdevicedefinitionversionsrequestlistdevicedefinitionversionspaginatetypedef) 
## ListDeviceDefinitionsPaginator

Type annotations and code completion for `#!python session.client("greengrass").get_paginator("list_device_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeviceDefinitions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrass.paginator import ListDeviceDefinitionsPaginator

session = Session()

session = get_session()
async with session.client("greengrass") as client:  # (1)
    paginator: ListDeviceDefinitionsPaginator = client.get_paginator("list_device_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeviceDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListDeviceDefinitionsPaginator](./paginators.md#listdevicedefinitionspaginator)
3. item: [:material-code-braces: ListDeviceDefinitionsResponseTypeDef](./type_defs.md#listdevicedefinitionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDeviceDefinitionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDeviceDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDeviceDefinitionsResponseTypeDef](./type_defs.md#listdevicedefinitionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef](./type_defs.md#listdevicedefinitionsrequestlistdevicedefinitionspaginatetypedef) 
## ListFunctionDefinitionVersionsPaginator

Type annotations and code completion for `#!python session.client("greengrass").get_paginator("list_function_definition_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListFunctionDefinitionVersions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrass.paginator import ListFunctionDefinitionVersionsPaginator

session = Session()

session = get_session()
async with session.client("greengrass") as client:  # (1)
    paginator: ListFunctionDefinitionVersionsPaginator = client.get_paginator("list_function_definition_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListFunctionDefinitionVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListFunctionDefinitionVersionsPaginator](./paginators.md#listfunctiondefinitionversionspaginator)
3. item: [:material-code-braces: ListFunctionDefinitionVersionsResponseTypeDef](./type_defs.md#listfunctiondefinitionversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFunctionDefinitionVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    FunctionDefinitionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListFunctionDefinitionVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFunctionDefinitionVersionsResponseTypeDef](./type_defs.md#listfunctiondefinitionversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef = {  # (1)
    "FunctionDefinitionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef](./type_defs.md#listfunctiondefinitionversionsrequestlistfunctiondefinitionversionspaginatetypedef) 
## ListFunctionDefinitionsPaginator

Type annotations and code completion for `#!python session.client("greengrass").get_paginator("list_function_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListFunctionDefinitions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrass.paginator import ListFunctionDefinitionsPaginator

session = Session()

session = get_session()
async with session.client("greengrass") as client:  # (1)
    paginator: ListFunctionDefinitionsPaginator = client.get_paginator("list_function_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: ListFunctionDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListFunctionDefinitionsPaginator](./paginators.md#listfunctiondefinitionspaginator)
3. item: [:material-code-braces: ListFunctionDefinitionsResponseTypeDef](./type_defs.md#listfunctiondefinitionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFunctionDefinitionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListFunctionDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFunctionDefinitionsResponseTypeDef](./type_defs.md#listfunctiondefinitionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef](./type_defs.md#listfunctiondefinitionsrequestlistfunctiondefinitionspaginatetypedef) 
## ListGroupVersionsPaginator

Type annotations and code completion for `#!python session.client("greengrass").get_paginator("list_group_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListGroupVersions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrass.paginator import ListGroupVersionsPaginator

session = Session()

session = get_session()
async with session.client("greengrass") as client:  # (1)
    paginator: ListGroupVersionsPaginator = client.get_paginator("list_group_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListGroupVersionsPaginator](./paginators.md#listgroupversionspaginator)
3. item: [:material-code-braces: ListGroupVersionsResponseTypeDef](./type_defs.md#listgroupversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGroupVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GroupId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListGroupVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGroupVersionsResponseTypeDef](./type_defs.md#listgroupversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListGroupVersionsRequestListGroupVersionsPaginateTypeDef = {  # (1)
    "GroupId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupVersionsRequestListGroupVersionsPaginateTypeDef](./type_defs.md#listgroupversionsrequestlistgroupversionspaginatetypedef) 
## ListGroupsPaginator

Type annotations and code completion for `#!python session.client("greengrass").get_paginator("list_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListGroups)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrass.paginator import ListGroupsPaginator

session = Session()

session = get_session()
async with session.client("greengrass") as client:  # (1)
    paginator: ListGroupsPaginator = client.get_paginator("list_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListGroupsPaginator](./paginators.md#listgroupspaginator)
3. item: [:material-code-braces: ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListGroupsRequestListGroupsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupsRequestListGroupsPaginateTypeDef](./type_defs.md#listgroupsrequestlistgroupspaginatetypedef) 
## ListLoggerDefinitionVersionsPaginator

Type annotations and code completion for `#!python session.client("greengrass").get_paginator("list_logger_definition_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListLoggerDefinitionVersions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrass.paginator import ListLoggerDefinitionVersionsPaginator

session = Session()

session = get_session()
async with session.client("greengrass") as client:  # (1)
    paginator: ListLoggerDefinitionVersionsPaginator = client.get_paginator("list_logger_definition_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListLoggerDefinitionVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListLoggerDefinitionVersionsPaginator](./paginators.md#listloggerdefinitionversionspaginator)
3. item: [:material-code-braces: ListLoggerDefinitionVersionsResponseTypeDef](./type_defs.md#listloggerdefinitionversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListLoggerDefinitionVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    LoggerDefinitionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListLoggerDefinitionVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListLoggerDefinitionVersionsResponseTypeDef](./type_defs.md#listloggerdefinitionversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef = {  # (1)
    "LoggerDefinitionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef](./type_defs.md#listloggerdefinitionversionsrequestlistloggerdefinitionversionspaginatetypedef) 
## ListLoggerDefinitionsPaginator

Type annotations and code completion for `#!python session.client("greengrass").get_paginator("list_logger_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListLoggerDefinitions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrass.paginator import ListLoggerDefinitionsPaginator

session = Session()

session = get_session()
async with session.client("greengrass") as client:  # (1)
    paginator: ListLoggerDefinitionsPaginator = client.get_paginator("list_logger_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: ListLoggerDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListLoggerDefinitionsPaginator](./paginators.md#listloggerdefinitionspaginator)
3. item: [:material-code-braces: ListLoggerDefinitionsResponseTypeDef](./type_defs.md#listloggerdefinitionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListLoggerDefinitionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListLoggerDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListLoggerDefinitionsResponseTypeDef](./type_defs.md#listloggerdefinitionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef](./type_defs.md#listloggerdefinitionsrequestlistloggerdefinitionspaginatetypedef) 
## ListResourceDefinitionVersionsPaginator

Type annotations and code completion for `#!python session.client("greengrass").get_paginator("list_resource_definition_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListResourceDefinitionVersions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrass.paginator import ListResourceDefinitionVersionsPaginator

session = Session()

session = get_session()
async with session.client("greengrass") as client:  # (1)
    paginator: ListResourceDefinitionVersionsPaginator = client.get_paginator("list_resource_definition_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceDefinitionVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListResourceDefinitionVersionsPaginator](./paginators.md#listresourcedefinitionversionspaginator)
3. item: [:material-code-braces: ListResourceDefinitionVersionsResponseTypeDef](./type_defs.md#listresourcedefinitionversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResourceDefinitionVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceDefinitionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListResourceDefinitionVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResourceDefinitionVersionsResponseTypeDef](./type_defs.md#listresourcedefinitionversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef = {  # (1)
    "ResourceDefinitionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef](./type_defs.md#listresourcedefinitionversionsrequestlistresourcedefinitionversionspaginatetypedef) 
## ListResourceDefinitionsPaginator

Type annotations and code completion for `#!python session.client("greengrass").get_paginator("list_resource_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListResourceDefinitions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrass.paginator import ListResourceDefinitionsPaginator

session = Session()

session = get_session()
async with session.client("greengrass") as client:  # (1)
    paginator: ListResourceDefinitionsPaginator = client.get_paginator("list_resource_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListResourceDefinitionsPaginator](./paginators.md#listresourcedefinitionspaginator)
3. item: [:material-code-braces: ListResourceDefinitionsResponseTypeDef](./type_defs.md#listresourcedefinitionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResourceDefinitionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListResourceDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResourceDefinitionsResponseTypeDef](./type_defs.md#listresourcedefinitionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef](./type_defs.md#listresourcedefinitionsrequestlistresourcedefinitionspaginatetypedef) 
## ListSubscriptionDefinitionVersionsPaginator

Type annotations and code completion for `#!python session.client("greengrass").get_paginator("list_subscription_definition_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListSubscriptionDefinitionVersions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrass.paginator import ListSubscriptionDefinitionVersionsPaginator

session = Session()

session = get_session()
async with session.client("greengrass") as client:  # (1)
    paginator: ListSubscriptionDefinitionVersionsPaginator = client.get_paginator("list_subscription_definition_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSubscriptionDefinitionVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListSubscriptionDefinitionVersionsPaginator](./paginators.md#listsubscriptiondefinitionversionspaginator)
3. item: [:material-code-braces: ListSubscriptionDefinitionVersionsResponseTypeDef](./type_defs.md#listsubscriptiondefinitionversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSubscriptionDefinitionVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    SubscriptionDefinitionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSubscriptionDefinitionVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSubscriptionDefinitionVersionsResponseTypeDef](./type_defs.md#listsubscriptiondefinitionversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef = {  # (1)
    "SubscriptionDefinitionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef](./type_defs.md#listsubscriptiondefinitionversionsrequestlistsubscriptiondefinitionversionspaginatetypedef) 
## ListSubscriptionDefinitionsPaginator

Type annotations and code completion for `#!python session.client("greengrass").get_paginator("list_subscription_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListSubscriptionDefinitions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrass.paginator import ListSubscriptionDefinitionsPaginator

session = Session()

session = get_session()
async with session.client("greengrass") as client:  # (1)
    paginator: ListSubscriptionDefinitionsPaginator = client.get_paginator("list_subscription_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSubscriptionDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListSubscriptionDefinitionsPaginator](./paginators.md#listsubscriptiondefinitionspaginator)
3. item: [:material-code-braces: ListSubscriptionDefinitionsResponseTypeDef](./type_defs.md#listsubscriptiondefinitionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSubscriptionDefinitionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSubscriptionDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSubscriptionDefinitionsResponseTypeDef](./type_defs.md#listsubscriptiondefinitionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef](./type_defs.md#listsubscriptiondefinitionsrequestlistsubscriptiondefinitionspaginatetypedef) 
