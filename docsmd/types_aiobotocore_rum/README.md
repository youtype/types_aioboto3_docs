# CloudWatchRUM module

> [Index](../README.md) > CloudWatchRUM


!!! note ""

    Auto-generated documentation for [CloudWatchRUM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
    type annotations stubs module [types-aiobotocore-rum](https://pypi.org/project/types-aiobotocore-rum/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `CloudWatchRUM`.

### From PyPI with pip

Install `types-aioboto3` for `CloudWatchRUM` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[rum]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[rum]'


# standalone installation
python -m pip install types-aiobotocore-rum
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-rum
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CloudWatchRUMClient

Type annotations and code completion for  `#!python session.client("rum")` as [CloudWatchRUMClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_rum.client import CloudWatchRUMClient


session = Session()
async with session.client("rum") as client:
    client: CloudWatchRUMClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("rum").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_rum.paginator import GetAppMonitorDataPaginator

def get_get_app_monitor_data_paginator() -> GetAppMonitorDataPaginator:
    return client.get_paginator("get_app_monitor_data"))
```

- [GetAppMonitorDataPaginator](./paginators.md#getappmonitordatapaginator)
- [ListAppMonitorsPaginator](./paginators.md#listappmonitorspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_rum.literals import GetAppMonitorDataPaginatorName

def get_value() -> GetAppMonitorDataPaginatorName:
    return "get_app_monitor_data"
```

- [GetAppMonitorDataPaginatorName](./literals.md#getappmonitordatapaginatorname)
- [ListAppMonitorsPaginatorName](./literals.md#listappmonitorspaginatorname)
- [StateEnumType](./literals.md#stateenumtype)
- [TelemetryType](./literals.md#telemetrytype)
- [CloudWatchRUMServiceName](./literals.md#cloudwatchrumservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_rum.type_defs import AppMonitorConfigurationTypeDef

def get_value() -> AppMonitorConfigurationTypeDef:
    return {
        "AllowCookies": ...,
    }
```

- [AppMonitorConfigurationTypeDef](./type_defs.md#appmonitorconfigurationtypedef)
- [AppMonitorDetailsTypeDef](./type_defs.md#appmonitordetailstypedef)
- [AppMonitorSummaryTypeDef](./type_defs.md#appmonitorsummarytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CwLogTypeDef](./type_defs.md#cwlogtypedef)
- [DeleteAppMonitorRequestRequestTypeDef](./type_defs.md#deleteappmonitorrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [QueryFilterTypeDef](./type_defs.md#queryfiltertypedef)
- [TimeRangeTypeDef](./type_defs.md#timerangetypedef)
- [GetAppMonitorRequestRequestTypeDef](./type_defs.md#getappmonitorrequestrequesttypedef)
- [ListAppMonitorsRequestRequestTypeDef](./type_defs.md#listappmonitorsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [RumEventTypeDef](./type_defs.md#rumeventtypedef)
- [UserDetailsTypeDef](./type_defs.md#userdetailstypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [CreateAppMonitorRequestRequestTypeDef](./type_defs.md#createappmonitorrequestrequesttypedef)
- [UpdateAppMonitorRequestRequestTypeDef](./type_defs.md#updateappmonitorrequestrequesttypedef)
- [CreateAppMonitorResponseTypeDef](./type_defs.md#createappmonitorresponsetypedef)
- [GetAppMonitorDataResponseTypeDef](./type_defs.md#getappmonitordataresponsetypedef)
- [ListAppMonitorsResponseTypeDef](./type_defs.md#listappmonitorsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [DataStorageTypeDef](./type_defs.md#datastoragetypedef)
- [ListAppMonitorsRequestListAppMonitorsPaginateTypeDef](./type_defs.md#listappmonitorsrequestlistappmonitorspaginatetypedef)
- [GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef](./type_defs.md#getappmonitordatarequestgetappmonitordatapaginatetypedef)
- [GetAppMonitorDataRequestRequestTypeDef](./type_defs.md#getappmonitordatarequestrequesttypedef)
- [PutRumEventsRequestRequestTypeDef](./type_defs.md#putrumeventsrequestrequesttypedef)
- [AppMonitorTypeDef](./type_defs.md#appmonitortypedef)
- [GetAppMonitorResponseTypeDef](./type_defs.md#getappmonitorresponsetypedef)

