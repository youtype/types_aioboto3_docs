# WorkSpacesThinClient module

> [Index](../README.md) > WorkSpacesThinClient


!!! note ""

    Auto-generated documentation for [WorkSpacesThinClient](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#workspacesthinclient)
    type annotations stubs module [types-aiobotocore-workspaces-thin-client](https://pypi.org/project/types-aiobotocore-workspaces-thin-client/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `WorkSpacesThinClient` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `WorkSpacesThinClient` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[workspaces-thin-client]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[workspaces-thin-client]'

# standalone installation
python -m pip install types-aiobotocore-workspaces-thin-client
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-workspaces-thin-client
```

## Usage

Code samples can be found in [Examples](./usage.md).

## WorkSpacesThinClientClient

Type annotations and code completion for  `#!python session.client("workspaces-thin-client")` as [WorkSpacesThinClientClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient.Client)

```python
# WorkSpacesThinClientClient usage example

from aioboto3.session import Session

from types_aiobotocore_workspaces_thin_client.client import WorkSpacesThinClientClient


session = Session()
async with session.client("workspaces-thin-client") as client:
    client: WorkSpacesThinClientClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("workspaces-thin-client").get_paginator("...")`.

```python
# ListDevicesPaginator usage example

from types_aiobotocore_workspaces_thin_client.paginator import ListDevicesPaginator

def get_list_devices_paginator() -> ListDevicesPaginator:
    return client.get_paginator("list_devices"))
```

- [ListDevicesPaginator](./paginators.md#listdevicespaginator)
- [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)
- [ListSoftwareSetsPaginator](./paginators.md#listsoftwaresetspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ApplyTimeOfType usage example

from types_aiobotocore_workspaces_thin_client.literals import ApplyTimeOfType

def get_value() -> ApplyTimeOfType:
    return "DEVICE"
```

- [ApplyTimeOfType](./literals.md#applytimeoftype)
- [DayOfWeekType](./literals.md#dayofweektype)
- [DesktopTypeType](./literals.md#desktoptypetype)
- [DeviceSoftwareSetComplianceStatusType](./literals.md#devicesoftwaresetcompliancestatustype)
- [DeviceStatusType](./literals.md#devicestatustype)
- [EnvironmentSoftwareSetComplianceStatusType](./literals.md#environmentsoftwaresetcompliancestatustype)
- [ListDevicesPaginatorName](./literals.md#listdevicespaginatorname)
- [ListEnvironmentsPaginatorName](./literals.md#listenvironmentspaginatorname)
- [ListSoftwareSetsPaginatorName](./literals.md#listsoftwaresetspaginatorname)
- [MaintenanceWindowTypeType](./literals.md#maintenancewindowtypetype)
- [SoftwareSetUpdateModeType](./literals.md#softwaresetupdatemodetype)
- [SoftwareSetUpdateScheduleType](./literals.md#softwaresetupdatescheduletype)
- [SoftwareSetUpdateStatusType](./literals.md#softwaresetupdatestatustype)
- [SoftwareSetValidationStatusType](./literals.md#softwaresetvalidationstatustype)
- [TargetDeviceStatusType](./literals.md#targetdevicestatustype)
- [WorkSpacesThinClientServiceName](./literals.md#workspacesthinclientservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [MaintenanceWindowTypeDef](./type_defs.md#maintenancewindowtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteDeviceRequestRequestTypeDef](./type_defs.md#deletedevicerequestrequesttypedef)
- [DeleteEnvironmentRequestRequestTypeDef](./type_defs.md#deleteenvironmentrequestrequesttypedef)
- [DeregisterDeviceRequestRequestTypeDef](./type_defs.md#deregisterdevicerequestrequesttypedef)
- [DeviceSummaryTypeDef](./type_defs.md#devicesummarytypedef)
- [DeviceTypeDef](./type_defs.md#devicetypedef)
- [MaintenanceWindowOutputTypeDef](./type_defs.md#maintenancewindowoutputtypedef)
- [GetDeviceRequestRequestTypeDef](./type_defs.md#getdevicerequestrequesttypedef)
- [GetEnvironmentRequestRequestTypeDef](./type_defs.md#getenvironmentrequestrequesttypedef)
- [GetSoftwareSetRequestRequestTypeDef](./type_defs.md#getsoftwaresetrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListDevicesRequestRequestTypeDef](./type_defs.md#listdevicesrequestrequesttypedef)
- [ListEnvironmentsRequestRequestTypeDef](./type_defs.md#listenvironmentsrequestrequesttypedef)
- [ListSoftwareSetsRequestRequestTypeDef](./type_defs.md#listsoftwaresetsrequestrequesttypedef)
- [SoftwareSetSummaryTypeDef](./type_defs.md#softwaresetsummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [SoftwareTypeDef](./type_defs.md#softwaretypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateDeviceRequestRequestTypeDef](./type_defs.md#updatedevicerequestrequesttypedef)
- [UpdateSoftwareSetRequestRequestTypeDef](./type_defs.md#updatesoftwaresetrequestrequesttypedef)
- [CreateEnvironmentRequestRequestTypeDef](./type_defs.md#createenvironmentrequestrequesttypedef)
- [UpdateEnvironmentRequestRequestTypeDef](./type_defs.md#updateenvironmentrequestrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ListDevicesResponseTypeDef](./type_defs.md#listdevicesresponsetypedef)
- [UpdateDeviceResponseTypeDef](./type_defs.md#updatedeviceresponsetypedef)
- [GetDeviceResponseTypeDef](./type_defs.md#getdeviceresponsetypedef)
- [EnvironmentSummaryTypeDef](./type_defs.md#environmentsummarytypedef)
- [EnvironmentTypeDef](./type_defs.md#environmenttypedef)
- [ListDevicesRequestPaginateTypeDef](./type_defs.md#listdevicesrequestpaginatetypedef)
- [ListEnvironmentsRequestPaginateTypeDef](./type_defs.md#listenvironmentsrequestpaginatetypedef)
- [ListSoftwareSetsRequestPaginateTypeDef](./type_defs.md#listsoftwaresetsrequestpaginatetypedef)
- [ListSoftwareSetsResponseTypeDef](./type_defs.md#listsoftwaresetsresponsetypedef)
- [SoftwareSetTypeDef](./type_defs.md#softwaresettypedef)
- [CreateEnvironmentResponseTypeDef](./type_defs.md#createenvironmentresponsetypedef)
- [ListEnvironmentsResponseTypeDef](./type_defs.md#listenvironmentsresponsetypedef)
- [UpdateEnvironmentResponseTypeDef](./type_defs.md#updateenvironmentresponsetypedef)
- [GetEnvironmentResponseTypeDef](./type_defs.md#getenvironmentresponsetypedef)
- [GetSoftwareSetResponseTypeDef](./type_defs.md#getsoftwaresetresponsetypedef)
