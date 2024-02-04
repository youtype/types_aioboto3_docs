# ControlTower module

> [Index](../README.md) > ControlTower


!!! note ""

    Auto-generated documentation for [ControlTower](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
    type annotations stubs module [types-aiobotocore-controltower](https://pypi.org/project/types-aiobotocore-controltower/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `ControlTower` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[controltower]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[controltower]'


# standalone installation
python -m pip install types-aiobotocore-controltower
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-controltower
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ControlTowerClient

Type annotations and code completion for  `#!python session.client("controltower")` as [ControlTowerClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client)

```python
# ControlTowerClient usage example

from aioboto3.session import Session

from types_aiobotocore_controltower.client import ControlTowerClient


session = Session()
async with session.client("controltower") as client:
    client: ControlTowerClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("controltower").get_paginator("...")`.

```python
# ListEnabledControlsPaginator usage example

from types_aiobotocore_controltower.paginator import ListEnabledControlsPaginator

def get_list_enabled_controls_paginator() -> ListEnabledControlsPaginator:
    return client.get_paginator("list_enabled_controls"))
```

- [ListEnabledControlsPaginator](./paginators.md#listenabledcontrolspaginator)
- [ListLandingZonesPaginator](./paginators.md#listlandingzonespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ControlOperationStatusType usage example

from types_aiobotocore_controltower.literals import ControlOperationStatusType

def get_value() -> ControlOperationStatusType:
    return "FAILED"
```

- [ControlOperationStatusType](./literals.md#controloperationstatustype)
- [ControlOperationTypeType](./literals.md#controloperationtypetype)
- [DriftStatusType](./literals.md#driftstatustype)
- [EnablementStatusType](./literals.md#enablementstatustype)
- [LandingZoneDriftStatusType](./literals.md#landingzonedriftstatustype)
- [LandingZoneOperationStatusType](./literals.md#landingzoneoperationstatustype)
- [LandingZoneOperationTypeType](./literals.md#landingzoneoperationtypetype)
- [LandingZoneStatusType](./literals.md#landingzonestatustype)
- [ListEnabledControlsPaginatorName](./literals.md#listenabledcontrolspaginatorname)
- [ListLandingZonesPaginatorName](./literals.md#listlandingzonespaginatorname)
- [ControlTowerServiceName](./literals.md#controltowerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ControlOperationTypeDef](./type_defs.md#controloperationtypedef)
- [CreateLandingZoneInputRequestTypeDef](./type_defs.md#createlandingzoneinputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteLandingZoneInputRequestTypeDef](./type_defs.md#deletelandingzoneinputrequesttypedef)
- [DisableControlInputRequestTypeDef](./type_defs.md#disablecontrolinputrequesttypedef)
- [DriftStatusSummaryTypeDef](./type_defs.md#driftstatussummarytypedef)
- [EnabledControlParameterTypeDef](./type_defs.md#enabledcontrolparametertypedef)
- [EnabledControlParameterSummaryTypeDef](./type_defs.md#enabledcontrolparametersummarytypedef)
- [EnablementStatusSummaryTypeDef](./type_defs.md#enablementstatussummarytypedef)
- [RegionTypeDef](./type_defs.md#regiontypedef)
- [GetControlOperationInputRequestTypeDef](./type_defs.md#getcontroloperationinputrequesttypedef)
- [GetEnabledControlInputRequestTypeDef](./type_defs.md#getenabledcontrolinputrequesttypedef)
- [GetLandingZoneInputRequestTypeDef](./type_defs.md#getlandingzoneinputrequesttypedef)
- [GetLandingZoneOperationInputRequestTypeDef](./type_defs.md#getlandingzoneoperationinputrequesttypedef)
- [LandingZoneOperationDetailTypeDef](./type_defs.md#landingzoneoperationdetailtypedef)
- [LandingZoneDriftStatusSummaryTypeDef](./type_defs.md#landingzonedriftstatussummarytypedef)
- [LandingZoneSummaryTypeDef](./type_defs.md#landingzonesummarytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListEnabledControlsInputRequestTypeDef](./type_defs.md#listenabledcontrolsinputrequesttypedef)
- [ListLandingZonesInputRequestTypeDef](./type_defs.md#listlandingzonesinputrequesttypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [ResetLandingZoneInputRequestTypeDef](./type_defs.md#resetlandingzoneinputrequesttypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [UpdateLandingZoneInputRequestTypeDef](./type_defs.md#updatelandingzoneinputrequesttypedef)
- [CreateLandingZoneOutputTypeDef](./type_defs.md#createlandingzoneoutputtypedef)
- [DeleteLandingZoneOutputTypeDef](./type_defs.md#deletelandingzoneoutputtypedef)
- [DisableControlOutputTypeDef](./type_defs.md#disablecontroloutputtypedef)
- [EnableControlOutputTypeDef](./type_defs.md#enablecontroloutputtypedef)
- [GetControlOperationOutputTypeDef](./type_defs.md#getcontroloperationoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [ResetLandingZoneOutputTypeDef](./type_defs.md#resetlandingzoneoutputtypedef)
- [UpdateEnabledControlOutputTypeDef](./type_defs.md#updateenabledcontroloutputtypedef)
- [UpdateLandingZoneOutputTypeDef](./type_defs.md#updatelandingzoneoutputtypedef)
- [EnableControlInputRequestTypeDef](./type_defs.md#enablecontrolinputrequesttypedef)
- [UpdateEnabledControlInputRequestTypeDef](./type_defs.md#updateenabledcontrolinputrequesttypedef)
- [EnabledControlSummaryTypeDef](./type_defs.md#enabledcontrolsummarytypedef)
- [EnabledControlDetailsTypeDef](./type_defs.md#enabledcontroldetailstypedef)
- [GetLandingZoneOperationOutputTypeDef](./type_defs.md#getlandingzoneoperationoutputtypedef)
- [LandingZoneDetailTypeDef](./type_defs.md#landingzonedetailtypedef)
- [ListLandingZonesOutputTypeDef](./type_defs.md#listlandingzonesoutputtypedef)
- [ListEnabledControlsInputListEnabledControlsPaginateTypeDef](./type_defs.md#listenabledcontrolsinputlistenabledcontrolspaginatetypedef)
- [ListLandingZonesInputListLandingZonesPaginateTypeDef](./type_defs.md#listlandingzonesinputlistlandingzonespaginatetypedef)
- [ListEnabledControlsOutputTypeDef](./type_defs.md#listenabledcontrolsoutputtypedef)
- [GetEnabledControlOutputTypeDef](./type_defs.md#getenabledcontroloutputtypedef)
- [GetLandingZoneOutputTypeDef](./type_defs.md#getlandingzoneoutputtypedef)

