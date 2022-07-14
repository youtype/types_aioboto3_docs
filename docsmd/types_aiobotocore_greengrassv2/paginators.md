# Paginators

> [Index](../README.md) > [GreengrassV2](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [GreengrassV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
    type annotations stubs module [types-aiobotocore-greengrassv2](https://pypi.org/project/types-aiobotocore-greengrassv2/).

## ListClientDevicesAssociatedWithCoreDevicePaginator

Type annotations and code completion for `#!python session.client("greengrassv2").get_paginator("list_client_devices_associated_with_core_device")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListClientDevicesAssociatedWithCoreDevice)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrassv2.paginator import ListClientDevicesAssociatedWithCoreDevicePaginator

session = Session()

session = get_session()
async with session.client("greengrassv2") as client:  # (1)
    paginator: ListClientDevicesAssociatedWithCoreDevicePaginator = client.get_paginator("list_client_devices_associated_with_core_device")  # (2)
    async for item in paginator.paginate(...):
        item: ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassV2Client](./client.md)
2. paginator: [ListClientDevicesAssociatedWithCoreDevicePaginator](./paginators.md#listclientdevicesassociatedwithcoredevicepaginator)
3. item: [:material-code-braces: ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef](./type_defs.md#listclientdevicesassociatedwithcoredeviceresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListClientDevicesAssociatedWithCoreDevicePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    coreDeviceThingName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef](./type_defs.md#listclientdevicesassociatedwithcoredeviceresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef = {  # (1)
    "coreDeviceThingName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef](./type_defs.md#listclientdevicesassociatedwithcoredevicerequestlistclientdevicesassociatedwithcoredevicepaginatetypedef) 
## ListComponentVersionsPaginator

Type annotations and code completion for `#!python session.client("greengrassv2").get_paginator("list_component_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponentVersions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrassv2.paginator import ListComponentVersionsPaginator

session = Session()

session = get_session()
async with session.client("greengrassv2") as client:  # (1)
    paginator: ListComponentVersionsPaginator = client.get_paginator("list_component_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListComponentVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassV2Client](./client.md)
2. paginator: [ListComponentVersionsPaginator](./paginators.md#listcomponentversionspaginator)
3. item: [:material-code-braces: ListComponentVersionsResponseTypeDef](./type_defs.md#listcomponentversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListComponentVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    arn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListComponentVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListComponentVersionsResponseTypeDef](./type_defs.md#listcomponentversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListComponentVersionsRequestListComponentVersionsPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListComponentVersionsRequestListComponentVersionsPaginateTypeDef](./type_defs.md#listcomponentversionsrequestlistcomponentversionspaginatetypedef) 
## ListComponentsPaginator

Type annotations and code completion for `#!python session.client("greengrassv2").get_paginator("list_components")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponents)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrassv2.paginator import ListComponentsPaginator

session = Session()

session = get_session()
async with session.client("greengrassv2") as client:  # (1)
    paginator: ListComponentsPaginator = client.get_paginator("list_components")  # (2)
    async for item in paginator.paginate(...):
        item: ListComponentsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassV2Client](./client.md)
2. paginator: [ListComponentsPaginator](./paginators.md#listcomponentspaginator)
3. item: [:material-code-braces: ListComponentsResponseTypeDef](./type_defs.md#listcomponentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListComponentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    scope: ComponentVisibilityScopeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListComponentsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ComponentVisibilityScopeType](./literals.md#componentvisibilityscopetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListComponentsResponseTypeDef](./type_defs.md#listcomponentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListComponentsRequestListComponentsPaginateTypeDef = {  # (1)
    "scope": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListComponentsRequestListComponentsPaginateTypeDef](./type_defs.md#listcomponentsrequestlistcomponentspaginatetypedef) 
## ListCoreDevicesPaginator

Type annotations and code completion for `#!python session.client("greengrassv2").get_paginator("list_core_devices")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListCoreDevices)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrassv2.paginator import ListCoreDevicesPaginator

session = Session()

session = get_session()
async with session.client("greengrassv2") as client:  # (1)
    paginator: ListCoreDevicesPaginator = client.get_paginator("list_core_devices")  # (2)
    async for item in paginator.paginate(...):
        item: ListCoreDevicesResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassV2Client](./client.md)
2. paginator: [ListCoreDevicesPaginator](./paginators.md#listcoredevicespaginator)
3. item: [:material-code-braces: ListCoreDevicesResponseTypeDef](./type_defs.md#listcoredevicesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCoreDevicesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    thingGroupArn: str = ...,
    status: CoreDeviceStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListCoreDevicesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: CoreDeviceStatusType](./literals.md#coredevicestatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListCoreDevicesResponseTypeDef](./type_defs.md#listcoredevicesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCoreDevicesRequestListCoreDevicesPaginateTypeDef = {  # (1)
    "thingGroupArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCoreDevicesRequestListCoreDevicesPaginateTypeDef](./type_defs.md#listcoredevicesrequestlistcoredevicespaginatetypedef) 
## ListDeploymentsPaginator

Type annotations and code completion for `#!python session.client("greengrassv2").get_paginator("list_deployments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListDeployments)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrassv2.paginator import ListDeploymentsPaginator

session = Session()

session = get_session()
async with session.client("greengrassv2") as client:  # (1)
    paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeploymentsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassV2Client](./client.md)
2. paginator: [ListDeploymentsPaginator](./paginators.md#listdeploymentspaginator)
3. item: [:material-code-braces: ListDeploymentsResponseTypeDef](./type_defs.md#listdeploymentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDeploymentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    targetArn: str = ...,
    historyFilter: DeploymentHistoryFilterType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListDeploymentsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DeploymentHistoryFilterType](./literals.md#deploymenthistoryfiltertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDeploymentsResponseTypeDef](./type_defs.md#listdeploymentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDeploymentsRequestListDeploymentsPaginateTypeDef = {  # (1)
    "targetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeploymentsRequestListDeploymentsPaginateTypeDef](./type_defs.md#listdeploymentsrequestlistdeploymentspaginatetypedef) 
## ListEffectiveDeploymentsPaginator

Type annotations and code completion for `#!python session.client("greengrassv2").get_paginator("list_effective_deployments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListEffectiveDeployments)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrassv2.paginator import ListEffectiveDeploymentsPaginator

session = Session()

session = get_session()
async with session.client("greengrassv2") as client:  # (1)
    paginator: ListEffectiveDeploymentsPaginator = client.get_paginator("list_effective_deployments")  # (2)
    async for item in paginator.paginate(...):
        item: ListEffectiveDeploymentsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassV2Client](./client.md)
2. paginator: [ListEffectiveDeploymentsPaginator](./paginators.md#listeffectivedeploymentspaginator)
3. item: [:material-code-braces: ListEffectiveDeploymentsResponseTypeDef](./type_defs.md#listeffectivedeploymentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEffectiveDeploymentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    coreDeviceThingName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEffectiveDeploymentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEffectiveDeploymentsResponseTypeDef](./type_defs.md#listeffectivedeploymentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef = {  # (1)
    "coreDeviceThingName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef](./type_defs.md#listeffectivedeploymentsrequestlisteffectivedeploymentspaginatetypedef) 
## ListInstalledComponentsPaginator

Type annotations and code completion for `#!python session.client("greengrassv2").get_paginator("list_installed_components")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListInstalledComponents)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_greengrassv2.paginator import ListInstalledComponentsPaginator

session = Session()

session = get_session()
async with session.client("greengrassv2") as client:  # (1)
    paginator: ListInstalledComponentsPaginator = client.get_paginator("list_installed_components")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstalledComponentsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassV2Client](./client.md)
2. paginator: [ListInstalledComponentsPaginator](./paginators.md#listinstalledcomponentspaginator)
3. item: [:material-code-braces: ListInstalledComponentsResponseTypeDef](./type_defs.md#listinstalledcomponentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListInstalledComponentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    coreDeviceThingName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListInstalledComponentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInstalledComponentsResponseTypeDef](./type_defs.md#listinstalledcomponentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef = {  # (1)
    "coreDeviceThingName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef](./type_defs.md#listinstalledcomponentsrequestlistinstalledcomponentspaginatetypedef) 
