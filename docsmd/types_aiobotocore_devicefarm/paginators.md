# Paginators

> [Index](../README.md) > [DeviceFarm](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [DeviceFarm](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
    type annotations stubs module [types-aiobotocore-devicefarm](https://pypi.org/project/types-aiobotocore-devicefarm/).

## GetOfferingStatusPaginator

Type annotations and code completion for `#!python session.client("devicefarm").get_paginator("get_offering_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.GetOfferingStatus)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_devicefarm.paginator import GetOfferingStatusPaginator

session = Session()

session = get_session()
async with session.client("devicefarm") as client:  # (1)
    paginator: GetOfferingStatusPaginator = client.get_paginator("get_offering_status")  # (2)
    async for item in paginator.paginate(...):
        item: GetOfferingStatusResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [GetOfferingStatusPaginator](./paginators.md#getofferingstatuspaginator)
3. item: [:material-code-braces: GetOfferingStatusResultTypeDef](./type_defs.md#getofferingstatusresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetOfferingStatusPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetOfferingStatusResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetOfferingStatusResultTypeDef](./type_defs.md#getofferingstatusresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef](./type_defs.md#getofferingstatusrequestgetofferingstatuspaginatetypedef) 
## ListArtifactsPaginator

Type annotations and code completion for `#!python session.client("devicefarm").get_paginator("list_artifacts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListArtifacts)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_devicefarm.paginator import ListArtifactsPaginator

session = Session()

session = get_session()
async with session.client("devicefarm") as client:  # (1)
    paginator: ListArtifactsPaginator = client.get_paginator("list_artifacts")  # (2)
    async for item in paginator.paginate(...):
        item: ListArtifactsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListArtifactsPaginator](./paginators.md#listartifactspaginator)
3. item: [:material-code-braces: ListArtifactsResultTypeDef](./type_defs.md#listartifactsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListArtifactsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    arn: str,
    type: ArtifactCategoryType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListArtifactsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ArtifactCategoryType](./literals.md#artifactcategorytype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListArtifactsResultTypeDef](./type_defs.md#listartifactsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListArtifactsRequestListArtifactsPaginateTypeDef = {  # (1)
    "arn": ...,
    "type": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListArtifactsRequestListArtifactsPaginateTypeDef](./type_defs.md#listartifactsrequestlistartifactspaginatetypedef) 
## ListDeviceInstancesPaginator

Type annotations and code completion for `#!python session.client("devicefarm").get_paginator("list_device_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDeviceInstances)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_devicefarm.paginator import ListDeviceInstancesPaginator

session = Session()

session = get_session()
async with session.client("devicefarm") as client:  # (1)
    paginator: ListDeviceInstancesPaginator = client.get_paginator("list_device_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeviceInstancesResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListDeviceInstancesPaginator](./paginators.md#listdeviceinstancespaginator)
3. item: [:material-code-braces: ListDeviceInstancesResultTypeDef](./type_defs.md#listdeviceinstancesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListDeviceInstancesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDeviceInstancesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDeviceInstancesResultTypeDef](./type_defs.md#listdeviceinstancesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef](./type_defs.md#listdeviceinstancesrequestlistdeviceinstancespaginatetypedef) 
## ListDevicePoolsPaginator

Type annotations and code completion for `#!python session.client("devicefarm").get_paginator("list_device_pools")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDevicePools)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_devicefarm.paginator import ListDevicePoolsPaginator

session = Session()

session = get_session()
async with session.client("devicefarm") as client:  # (1)
    paginator: ListDevicePoolsPaginator = client.get_paginator("list_device_pools")  # (2)
    async for item in paginator.paginate(...):
        item: ListDevicePoolsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListDevicePoolsPaginator](./paginators.md#listdevicepoolspaginator)
3. item: [:material-code-braces: ListDevicePoolsResultTypeDef](./type_defs.md#listdevicepoolsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListDevicePoolsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    arn: str,
    type: DevicePoolTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListDevicePoolsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DevicePoolTypeType](./literals.md#devicepooltypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDevicePoolsResultTypeDef](./type_defs.md#listdevicepoolsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListDevicePoolsRequestListDevicePoolsPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDevicePoolsRequestListDevicePoolsPaginateTypeDef](./type_defs.md#listdevicepoolsrequestlistdevicepoolspaginatetypedef) 
## ListDevicesPaginator

Type annotations and code completion for `#!python session.client("devicefarm").get_paginator("list_devices")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDevices)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_devicefarm.paginator import ListDevicesPaginator

session = Session()

session = get_session()
async with session.client("devicefarm") as client:  # (1)
    paginator: ListDevicesPaginator = client.get_paginator("list_devices")  # (2)
    async for item in paginator.paginate(...):
        item: ListDevicesResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListDevicesPaginator](./paginators.md#listdevicespaginator)
3. item: [:material-code-braces: ListDevicesResultTypeDef](./type_defs.md#listdevicesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListDevicesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    arn: str = ...,
    filters: Sequence[DeviceFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListDevicesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DeviceFilterTypeDef](./type_defs.md#devicefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDevicesResultTypeDef](./type_defs.md#listdevicesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListDevicesRequestListDevicesPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDevicesRequestListDevicesPaginateTypeDef](./type_defs.md#listdevicesrequestlistdevicespaginatetypedef) 
## ListInstanceProfilesPaginator

Type annotations and code completion for `#!python session.client("devicefarm").get_paginator("list_instance_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListInstanceProfiles)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_devicefarm.paginator import ListInstanceProfilesPaginator

session = Session()

session = get_session()
async with session.client("devicefarm") as client:  # (1)
    paginator: ListInstanceProfilesPaginator = client.get_paginator("list_instance_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstanceProfilesResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListInstanceProfilesPaginator](./paginators.md#listinstanceprofilespaginator)
3. item: [:material-code-braces: ListInstanceProfilesResultTypeDef](./type_defs.md#listinstanceprofilesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListInstanceProfilesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListInstanceProfilesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInstanceProfilesResultTypeDef](./type_defs.md#listinstanceprofilesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef](./type_defs.md#listinstanceprofilesrequestlistinstanceprofilespaginatetypedef) 
## ListJobsPaginator

Type annotations and code completion for `#!python session.client("devicefarm").get_paginator("list_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListJobs)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_devicefarm.paginator import ListJobsPaginator

session = Session()

session = get_session()
async with session.client("devicefarm") as client:  # (1)
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListJobsPaginator](./paginators.md#listjobspaginator)
3. item: [:material-code-braces: ListJobsResultTypeDef](./type_defs.md#listjobsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    arn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListJobsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListJobsResultTypeDef](./type_defs.md#listjobsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListJobsRequestListJobsPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestListJobsPaginateTypeDef](./type_defs.md#listjobsrequestlistjobspaginatetypedef) 
## ListNetworkProfilesPaginator

Type annotations and code completion for `#!python session.client("devicefarm").get_paginator("list_network_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListNetworkProfiles)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_devicefarm.paginator import ListNetworkProfilesPaginator

session = Session()

session = get_session()
async with session.client("devicefarm") as client:  # (1)
    paginator: ListNetworkProfilesPaginator = client.get_paginator("list_network_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListNetworkProfilesResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListNetworkProfilesPaginator](./paginators.md#listnetworkprofilespaginator)
3. item: [:material-code-braces: ListNetworkProfilesResultTypeDef](./type_defs.md#listnetworkprofilesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListNetworkProfilesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    arn: str,
    type: NetworkProfileTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListNetworkProfilesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: NetworkProfileTypeType](./literals.md#networkprofiletypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListNetworkProfilesResultTypeDef](./type_defs.md#listnetworkprofilesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef](./type_defs.md#listnetworkprofilesrequestlistnetworkprofilespaginatetypedef) 
## ListOfferingPromotionsPaginator

Type annotations and code completion for `#!python session.client("devicefarm").get_paginator("list_offering_promotions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferingPromotions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_devicefarm.paginator import ListOfferingPromotionsPaginator

session = Session()

session = get_session()
async with session.client("devicefarm") as client:  # (1)
    paginator: ListOfferingPromotionsPaginator = client.get_paginator("list_offering_promotions")  # (2)
    async for item in paginator.paginate(...):
        item: ListOfferingPromotionsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListOfferingPromotionsPaginator](./paginators.md#listofferingpromotionspaginator)
3. item: [:material-code-braces: ListOfferingPromotionsResultTypeDef](./type_defs.md#listofferingpromotionsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListOfferingPromotionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListOfferingPromotionsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOfferingPromotionsResultTypeDef](./type_defs.md#listofferingpromotionsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef](./type_defs.md#listofferingpromotionsrequestlistofferingpromotionspaginatetypedef) 
## ListOfferingTransactionsPaginator

Type annotations and code completion for `#!python session.client("devicefarm").get_paginator("list_offering_transactions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferingTransactions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_devicefarm.paginator import ListOfferingTransactionsPaginator

session = Session()

session = get_session()
async with session.client("devicefarm") as client:  # (1)
    paginator: ListOfferingTransactionsPaginator = client.get_paginator("list_offering_transactions")  # (2)
    async for item in paginator.paginate(...):
        item: ListOfferingTransactionsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListOfferingTransactionsPaginator](./paginators.md#listofferingtransactionspaginator)
3. item: [:material-code-braces: ListOfferingTransactionsResultTypeDef](./type_defs.md#listofferingtransactionsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListOfferingTransactionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListOfferingTransactionsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOfferingTransactionsResultTypeDef](./type_defs.md#listofferingtransactionsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef](./type_defs.md#listofferingtransactionsrequestlistofferingtransactionspaginatetypedef) 
## ListOfferingsPaginator

Type annotations and code completion for `#!python session.client("devicefarm").get_paginator("list_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferings)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_devicefarm.paginator import ListOfferingsPaginator

session = Session()

session = get_session()
async with session.client("devicefarm") as client:  # (1)
    paginator: ListOfferingsPaginator = client.get_paginator("list_offerings")  # (2)
    async for item in paginator.paginate(...):
        item: ListOfferingsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListOfferingsPaginator](./paginators.md#listofferingspaginator)
3. item: [:material-code-braces: ListOfferingsResultTypeDef](./type_defs.md#listofferingsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListOfferingsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListOfferingsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOfferingsResultTypeDef](./type_defs.md#listofferingsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListOfferingsRequestListOfferingsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOfferingsRequestListOfferingsPaginateTypeDef](./type_defs.md#listofferingsrequestlistofferingspaginatetypedef) 
## ListProjectsPaginator

Type annotations and code completion for `#!python session.client("devicefarm").get_paginator("list_projects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListProjects)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_devicefarm.paginator import ListProjectsPaginator

session = Session()

session = get_session()
async with session.client("devicefarm") as client:  # (1)
    paginator: ListProjectsPaginator = client.get_paginator("list_projects")  # (2)
    async for item in paginator.paginate(...):
        item: ListProjectsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListProjectsPaginator](./paginators.md#listprojectspaginator)
3. item: [:material-code-braces: ListProjectsResultTypeDef](./type_defs.md#listprojectsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListProjectsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    arn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListProjectsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProjectsResultTypeDef](./type_defs.md#listprojectsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListProjectsRequestListProjectsPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProjectsRequestListProjectsPaginateTypeDef](./type_defs.md#listprojectsrequestlistprojectspaginatetypedef) 
## ListRemoteAccessSessionsPaginator

Type annotations and code completion for `#!python session.client("devicefarm").get_paginator("list_remote_access_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListRemoteAccessSessions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_devicefarm.paginator import ListRemoteAccessSessionsPaginator

session = Session()

session = get_session()
async with session.client("devicefarm") as client:  # (1)
    paginator: ListRemoteAccessSessionsPaginator = client.get_paginator("list_remote_access_sessions")  # (2)
    async for item in paginator.paginate(...):
        item: ListRemoteAccessSessionsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListRemoteAccessSessionsPaginator](./paginators.md#listremoteaccesssessionspaginator)
3. item: [:material-code-braces: ListRemoteAccessSessionsResultTypeDef](./type_defs.md#listremoteaccesssessionsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListRemoteAccessSessionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    arn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRemoteAccessSessionsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRemoteAccessSessionsResultTypeDef](./type_defs.md#listremoteaccesssessionsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef](./type_defs.md#listremoteaccesssessionsrequestlistremoteaccesssessionspaginatetypedef) 
## ListRunsPaginator

Type annotations and code completion for `#!python session.client("devicefarm").get_paginator("list_runs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListRuns)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_devicefarm.paginator import ListRunsPaginator

session = Session()

session = get_session()
async with session.client("devicefarm") as client:  # (1)
    paginator: ListRunsPaginator = client.get_paginator("list_runs")  # (2)
    async for item in paginator.paginate(...):
        item: ListRunsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListRunsPaginator](./paginators.md#listrunspaginator)
3. item: [:material-code-braces: ListRunsResultTypeDef](./type_defs.md#listrunsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListRunsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    arn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRunsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRunsResultTypeDef](./type_defs.md#listrunsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListRunsRequestListRunsPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRunsRequestListRunsPaginateTypeDef](./type_defs.md#listrunsrequestlistrunspaginatetypedef) 
## ListSamplesPaginator

Type annotations and code completion for `#!python session.client("devicefarm").get_paginator("list_samples")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListSamples)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_devicefarm.paginator import ListSamplesPaginator

session = Session()

session = get_session()
async with session.client("devicefarm") as client:  # (1)
    paginator: ListSamplesPaginator = client.get_paginator("list_samples")  # (2)
    async for item in paginator.paginate(...):
        item: ListSamplesResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListSamplesPaginator](./paginators.md#listsamplespaginator)
3. item: [:material-code-braces: ListSamplesResultTypeDef](./type_defs.md#listsamplesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListSamplesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    arn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSamplesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSamplesResultTypeDef](./type_defs.md#listsamplesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListSamplesRequestListSamplesPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSamplesRequestListSamplesPaginateTypeDef](./type_defs.md#listsamplesrequestlistsamplespaginatetypedef) 
## ListSuitesPaginator

Type annotations and code completion for `#!python session.client("devicefarm").get_paginator("list_suites")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListSuites)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_devicefarm.paginator import ListSuitesPaginator

session = Session()

session = get_session()
async with session.client("devicefarm") as client:  # (1)
    paginator: ListSuitesPaginator = client.get_paginator("list_suites")  # (2)
    async for item in paginator.paginate(...):
        item: ListSuitesResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListSuitesPaginator](./paginators.md#listsuitespaginator)
3. item: [:material-code-braces: ListSuitesResultTypeDef](./type_defs.md#listsuitesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListSuitesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    arn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSuitesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSuitesResultTypeDef](./type_defs.md#listsuitesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListSuitesRequestListSuitesPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSuitesRequestListSuitesPaginateTypeDef](./type_defs.md#listsuitesrequestlistsuitespaginatetypedef) 
## ListTestsPaginator

Type annotations and code completion for `#!python session.client("devicefarm").get_paginator("list_tests")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListTests)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_devicefarm.paginator import ListTestsPaginator

session = Session()

session = get_session()
async with session.client("devicefarm") as client:  # (1)
    paginator: ListTestsPaginator = client.get_paginator("list_tests")  # (2)
    async for item in paginator.paginate(...):
        item: ListTestsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListTestsPaginator](./paginators.md#listtestspaginator)
3. item: [:material-code-braces: ListTestsResultTypeDef](./type_defs.md#listtestsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListTestsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    arn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTestsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTestsResultTypeDef](./type_defs.md#listtestsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListTestsRequestListTestsPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTestsRequestListTestsPaginateTypeDef](./type_defs.md#listtestsrequestlisttestspaginatetypedef) 
## ListUniqueProblemsPaginator

Type annotations and code completion for `#!python session.client("devicefarm").get_paginator("list_unique_problems")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListUniqueProblems)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_devicefarm.paginator import ListUniqueProblemsPaginator

session = Session()

session = get_session()
async with session.client("devicefarm") as client:  # (1)
    paginator: ListUniqueProblemsPaginator = client.get_paginator("list_unique_problems")  # (2)
    async for item in paginator.paginate(...):
        item: ListUniqueProblemsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListUniqueProblemsPaginator](./paginators.md#listuniqueproblemspaginator)
3. item: [:material-code-braces: ListUniqueProblemsResultTypeDef](./type_defs.md#listuniqueproblemsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListUniqueProblemsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    arn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListUniqueProblemsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUniqueProblemsResultTypeDef](./type_defs.md#listuniqueproblemsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef](./type_defs.md#listuniqueproblemsrequestlistuniqueproblemspaginatetypedef) 
## ListUploadsPaginator

Type annotations and code completion for `#!python session.client("devicefarm").get_paginator("list_uploads")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListUploads)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_devicefarm.paginator import ListUploadsPaginator

session = Session()

session = get_session()
async with session.client("devicefarm") as client:  # (1)
    paginator: ListUploadsPaginator = client.get_paginator("list_uploads")  # (2)
    async for item in paginator.paginate(...):
        item: ListUploadsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListUploadsPaginator](./paginators.md#listuploadspaginator)
3. item: [:material-code-braces: ListUploadsResultTypeDef](./type_defs.md#listuploadsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListUploadsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    arn: str,
    type: UploadTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListUploadsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: UploadTypeType](./literals.md#uploadtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListUploadsResultTypeDef](./type_defs.md#listuploadsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListUploadsRequestListUploadsPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUploadsRequestListUploadsPaginateTypeDef](./type_defs.md#listuploadsrequestlistuploadspaginatetypedef) 
## ListVPCEConfigurationsPaginator

Type annotations and code completion for `#!python session.client("devicefarm").get_paginator("list_vpce_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListVPCEConfigurations)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_devicefarm.paginator import ListVPCEConfigurationsPaginator

session = Session()

session = get_session()
async with session.client("devicefarm") as client:  # (1)
    paginator: ListVPCEConfigurationsPaginator = client.get_paginator("list_vpce_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListVPCEConfigurationsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListVPCEConfigurationsPaginator](./paginators.md#listvpceconfigurationspaginator)
3. item: [:material-code-braces: ListVPCEConfigurationsResultTypeDef](./type_defs.md#listvpceconfigurationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListVPCEConfigurationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListVPCEConfigurationsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListVPCEConfigurationsResultTypeDef](./type_defs.md#listvpceconfigurationsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef](./type_defs.md#listvpceconfigurationsrequestlistvpceconfigurationspaginatetypedef) 
