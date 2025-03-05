# SsmSap module

> [Index](../README.md) > SsmSap


!!! note ""

    Auto-generated documentation for [SsmSap](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#ssmsap)
    type annotations stubs module [types-aiobotocore-ssm-sap](https://pypi.org/project/types-aiobotocore-ssm-sap/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==14.1.0' mypy-boto3-builder`
1. Select `aioboto3` AWS SDK.
1. Add `SsmSap` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `SsmSap` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[ssm-sap]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[ssm-sap]'

# standalone installation
python -m pip install types-aiobotocore-ssm-sap
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-ssm-sap
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SsmSapClient

Type annotations and code completion for  `#!python session.client("ssm-sap")` as [SsmSapClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# SsmSapClient usage example

from aioboto3.session import Session

from types_aiobotocore_ssm_sap.client import SsmSapClient


session = Session()
async with session.client("ssm-sap") as client:
    client: SsmSapClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("ssm-sap").get_paginator("...")`.

```python
# ListApplicationsPaginator usage example

from types_aiobotocore_ssm_sap.paginator import ListApplicationsPaginator

def get_list_applications_paginator() -> ListApplicationsPaginator:
    return client.get_paginator("list_applications"))
```

- [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
- [ListComponentsPaginator](./paginators.md#listcomponentspaginator)
- [ListDatabasesPaginator](./paginators.md#listdatabasespaginator)
- [ListOperationEventsPaginator](./paginators.md#listoperationeventspaginator)
- [ListOperationsPaginator](./paginators.md#listoperationspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AllocationTypeType usage example

from types_aiobotocore_ssm_sap.literals import AllocationTypeType

def get_value() -> AllocationTypeType:
    return "ELASTIC_IP"
```

- [AllocationTypeType](./literals.md#allocationtypetype)
- [ApplicationDiscoveryStatusType](./literals.md#applicationdiscoverystatustype)
- [ApplicationStatusType](./literals.md#applicationstatustype)
- [ApplicationTypeType](./literals.md#applicationtypetype)
- [BackintModeType](./literals.md#backintmodetype)
- [ClusterStatusType](./literals.md#clusterstatustype)
- [ComponentStatusType](./literals.md#componentstatustype)
- [ComponentTypeType](./literals.md#componenttypetype)
- [ConnectedEntityTypeType](./literals.md#connectedentitytypetype)
- [CredentialTypeType](./literals.md#credentialtypetype)
- [DatabaseConnectionMethodType](./literals.md#databaseconnectionmethodtype)
- [DatabaseStatusType](./literals.md#databasestatustype)
- [DatabaseTypeType](./literals.md#databasetypetype)
- [FilterOperatorType](./literals.md#filteroperatortype)
- [HostRoleType](./literals.md#hostroletype)
- [ListApplicationsPaginatorName](./literals.md#listapplicationspaginatorname)
- [ListComponentsPaginatorName](./literals.md#listcomponentspaginatorname)
- [ListDatabasesPaginatorName](./literals.md#listdatabasespaginatorname)
- [ListOperationEventsPaginatorName](./literals.md#listoperationeventspaginatorname)
- [ListOperationsPaginatorName](./literals.md#listoperationspaginatorname)
- [OperationEventStatusType](./literals.md#operationeventstatustype)
- [OperationModeType](./literals.md#operationmodetype)
- [OperationStatusType](./literals.md#operationstatustype)
- [PermissionActionTypeType](./literals.md#permissionactiontypetype)
- [ReplicationModeType](./literals.md#replicationmodetype)
- [SsmSapServiceName](./literals.md#ssmsapservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ApplicationCredentialTypeDef](./type_defs.md#applicationcredentialtypedef)
- [ApplicationSummaryTypeDef](./type_defs.md#applicationsummarytypedef)
- [ApplicationTypeDef](./type_defs.md#applicationtypedef)
- [IpAddressMemberTypeDef](./type_defs.md#ipaddressmembertypedef)
- [BackintConfigTypeDef](./type_defs.md#backintconfigtypedef)
- [ComponentInfoTypeDef](./type_defs.md#componentinfotypedef)
- [ComponentSummaryTypeDef](./type_defs.md#componentsummarytypedef)
- [DatabaseConnectionTypeDef](./type_defs.md#databaseconnectiontypedef)
- [HostTypeDef](./type_defs.md#hosttypedef)
- [ResilienceTypeDef](./type_defs.md#resiliencetypedef)
- [DatabaseSummaryTypeDef](./type_defs.md#databasesummarytypedef)
- [DeleteResourcePermissionInputTypeDef](./type_defs.md#deleteresourcepermissioninputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeregisterApplicationInputTypeDef](./type_defs.md#deregisterapplicationinputtypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [GetApplicationInputTypeDef](./type_defs.md#getapplicationinputtypedef)
- [GetComponentInputTypeDef](./type_defs.md#getcomponentinputtypedef)
- [GetDatabaseInputTypeDef](./type_defs.md#getdatabaseinputtypedef)
- [GetOperationInputTypeDef](./type_defs.md#getoperationinputtypedef)
- [OperationTypeDef](./type_defs.md#operationtypedef)
- [GetResourcePermissionInputTypeDef](./type_defs.md#getresourcepermissioninputtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListComponentsInputTypeDef](./type_defs.md#listcomponentsinputtypedef)
- [ListDatabasesInputTypeDef](./type_defs.md#listdatabasesinputtypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [ResourceTypeDef](./type_defs.md#resourcetypedef)
- [PutResourcePermissionInputTypeDef](./type_defs.md#putresourcepermissioninputtypedef)
- [StartApplicationInputTypeDef](./type_defs.md#startapplicationinputtypedef)
- [StartApplicationRefreshInputTypeDef](./type_defs.md#startapplicationrefreshinputtypedef)
- [StopApplicationInputTypeDef](./type_defs.md#stopapplicationinputtypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [DatabaseTypeDef](./type_defs.md#databasetypedef)
- [AssociatedHostTypeDef](./type_defs.md#associatedhosttypedef)
- [UpdateApplicationSettingsInputTypeDef](./type_defs.md#updateapplicationsettingsinputtypedef)
- [RegisterApplicationInputTypeDef](./type_defs.md#registerapplicationinputtypedef)
- [DeleteResourcePermissionOutputTypeDef](./type_defs.md#deleteresourcepermissionoutputtypedef)
- [GetApplicationOutputTypeDef](./type_defs.md#getapplicationoutputtypedef)
- [GetResourcePermissionOutputTypeDef](./type_defs.md#getresourcepermissionoutputtypedef)
- [ListApplicationsOutputTypeDef](./type_defs.md#listapplicationsoutputtypedef)
- [ListComponentsOutputTypeDef](./type_defs.md#listcomponentsoutputtypedef)
- [ListDatabasesOutputTypeDef](./type_defs.md#listdatabasesoutputtypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PutResourcePermissionOutputTypeDef](./type_defs.md#putresourcepermissionoutputtypedef)
- [RegisterApplicationOutputTypeDef](./type_defs.md#registerapplicationoutputtypedef)
- [StartApplicationOutputTypeDef](./type_defs.md#startapplicationoutputtypedef)
- [StartApplicationRefreshOutputTypeDef](./type_defs.md#startapplicationrefreshoutputtypedef)
- [StopApplicationOutputTypeDef](./type_defs.md#stopapplicationoutputtypedef)
- [UpdateApplicationSettingsOutputTypeDef](./type_defs.md#updateapplicationsettingsoutputtypedef)
- [ListApplicationsInputTypeDef](./type_defs.md#listapplicationsinputtypedef)
- [ListOperationEventsInputTypeDef](./type_defs.md#listoperationeventsinputtypedef)
- [ListOperationsInputTypeDef](./type_defs.md#listoperationsinputtypedef)
- [GetOperationOutputTypeDef](./type_defs.md#getoperationoutputtypedef)
- [ListOperationsOutputTypeDef](./type_defs.md#listoperationsoutputtypedef)
- [ListApplicationsInputPaginateTypeDef](./type_defs.md#listapplicationsinputpaginatetypedef)
- [ListComponentsInputPaginateTypeDef](./type_defs.md#listcomponentsinputpaginatetypedef)
- [ListDatabasesInputPaginateTypeDef](./type_defs.md#listdatabasesinputpaginatetypedef)
- [ListOperationEventsInputPaginateTypeDef](./type_defs.md#listoperationeventsinputpaginatetypedef)
- [ListOperationsInputPaginateTypeDef](./type_defs.md#listoperationsinputpaginatetypedef)
- [OperationEventTypeDef](./type_defs.md#operationeventtypedef)
- [GetDatabaseOutputTypeDef](./type_defs.md#getdatabaseoutputtypedef)
- [ComponentTypeDef](./type_defs.md#componenttypedef)
- [ListOperationEventsOutputTypeDef](./type_defs.md#listoperationeventsoutputtypedef)
- [GetComponentOutputTypeDef](./type_defs.md#getcomponentoutputtypedef)

