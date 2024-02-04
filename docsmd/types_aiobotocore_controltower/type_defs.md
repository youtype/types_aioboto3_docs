# Type definitions

> [Index](../README.md) > [ControlTower](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ControlTower](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
    type annotations stubs module [types-aiobotocore-controltower](https://pypi.org/project/types-aiobotocore-controltower/).



## ControlOperationTypeDef

```python
# ControlOperationTypeDef definition

class ControlOperationTypeDef(TypedDict):
    endTime: NotRequired[datetime],
    operationType: NotRequired[ControlOperationTypeType],  # (1)
    startTime: NotRequired[datetime],
    status: NotRequired[ControlOperationStatusType],  # (2)
    statusMessage: NotRequired[str],
```

1. See [:material-code-brackets: ControlOperationTypeType](./literals.md#controloperationtypetype) 
2. See [:material-code-brackets: ControlOperationStatusType](./literals.md#controloperationstatustype) 
## CreateLandingZoneInputRequestTypeDef

```python
# CreateLandingZoneInputRequestTypeDef definition

class CreateLandingZoneInputRequestTypeDef(TypedDict):
    manifest: Mapping[str, Any],
    version: str,
    tags: NotRequired[Mapping[str, str]],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## DeleteLandingZoneInputRequestTypeDef

```python
# DeleteLandingZoneInputRequestTypeDef definition

class DeleteLandingZoneInputRequestTypeDef(TypedDict):
    landingZoneIdentifier: str,
```

## DisableControlInputRequestTypeDef

```python
# DisableControlInputRequestTypeDef definition

class DisableControlInputRequestTypeDef(TypedDict):
    controlIdentifier: str,
    targetIdentifier: str,
```

## DriftStatusSummaryTypeDef

```python
# DriftStatusSummaryTypeDef definition

class DriftStatusSummaryTypeDef(TypedDict):
    driftStatus: NotRequired[DriftStatusType],  # (1)
```

1. See [:material-code-brackets: DriftStatusType](./literals.md#driftstatustype) 
## EnabledControlParameterTypeDef

```python
# EnabledControlParameterTypeDef definition

class EnabledControlParameterTypeDef(TypedDict):
    key: str,
    value: Mapping[str, Any],
```

## EnabledControlParameterSummaryTypeDef

```python
# EnabledControlParameterSummaryTypeDef definition

class EnabledControlParameterSummaryTypeDef(TypedDict):
    key: str,
    value: Dict[str, Any],
```

## EnablementStatusSummaryTypeDef

```python
# EnablementStatusSummaryTypeDef definition

class EnablementStatusSummaryTypeDef(TypedDict):
    lastOperationIdentifier: NotRequired[str],
    status: NotRequired[EnablementStatusType],  # (1)
```

1. See [:material-code-brackets: EnablementStatusType](./literals.md#enablementstatustype) 
## RegionTypeDef

```python
# RegionTypeDef definition

class RegionTypeDef(TypedDict):
    name: NotRequired[str],
```

## GetControlOperationInputRequestTypeDef

```python
# GetControlOperationInputRequestTypeDef definition

class GetControlOperationInputRequestTypeDef(TypedDict):
    operationIdentifier: str,
```

## GetEnabledControlInputRequestTypeDef

```python
# GetEnabledControlInputRequestTypeDef definition

class GetEnabledControlInputRequestTypeDef(TypedDict):
    enabledControlIdentifier: str,
```

## GetLandingZoneInputRequestTypeDef

```python
# GetLandingZoneInputRequestTypeDef definition

class GetLandingZoneInputRequestTypeDef(TypedDict):
    landingZoneIdentifier: str,
```

## GetLandingZoneOperationInputRequestTypeDef

```python
# GetLandingZoneOperationInputRequestTypeDef definition

class GetLandingZoneOperationInputRequestTypeDef(TypedDict):
    operationIdentifier: str,
```

## LandingZoneOperationDetailTypeDef

```python
# LandingZoneOperationDetailTypeDef definition

class LandingZoneOperationDetailTypeDef(TypedDict):
    endTime: NotRequired[datetime],
    operationType: NotRequired[LandingZoneOperationTypeType],  # (1)
    startTime: NotRequired[datetime],
    status: NotRequired[LandingZoneOperationStatusType],  # (2)
    statusMessage: NotRequired[str],
```

1. See [:material-code-brackets: LandingZoneOperationTypeType](./literals.md#landingzoneoperationtypetype) 
2. See [:material-code-brackets: LandingZoneOperationStatusType](./literals.md#landingzoneoperationstatustype) 
## LandingZoneDriftStatusSummaryTypeDef

```python
# LandingZoneDriftStatusSummaryTypeDef definition

class LandingZoneDriftStatusSummaryTypeDef(TypedDict):
    status: NotRequired[LandingZoneDriftStatusType],  # (1)
```

1. See [:material-code-brackets: LandingZoneDriftStatusType](./literals.md#landingzonedriftstatustype) 
## LandingZoneSummaryTypeDef

```python
# LandingZoneSummaryTypeDef definition

class LandingZoneSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListEnabledControlsInputRequestTypeDef

```python
# ListEnabledControlsInputRequestTypeDef definition

class ListEnabledControlsInputRequestTypeDef(TypedDict):
    targetIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListLandingZonesInputRequestTypeDef

```python
# ListLandingZonesInputRequestTypeDef definition

class ListLandingZonesInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ResetLandingZoneInputRequestTypeDef

```python
# ResetLandingZoneInputRequestTypeDef definition

class ResetLandingZoneInputRequestTypeDef(TypedDict):
    landingZoneIdentifier: str,
```

## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateLandingZoneInputRequestTypeDef

```python
# UpdateLandingZoneInputRequestTypeDef definition

class UpdateLandingZoneInputRequestTypeDef(TypedDict):
    landingZoneIdentifier: str,
    manifest: Mapping[str, Any],
    version: str,
```

## CreateLandingZoneOutputTypeDef

```python
# CreateLandingZoneOutputTypeDef definition

class CreateLandingZoneOutputTypeDef(TypedDict):
    arn: str,
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteLandingZoneOutputTypeDef

```python
# DeleteLandingZoneOutputTypeDef definition

class DeleteLandingZoneOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisableControlOutputTypeDef

```python
# DisableControlOutputTypeDef definition

class DisableControlOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableControlOutputTypeDef

```python
# EnableControlOutputTypeDef definition

class EnableControlOutputTypeDef(TypedDict):
    arn: str,
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetControlOperationOutputTypeDef

```python
# GetControlOperationOutputTypeDef definition

class GetControlOperationOutputTypeDef(TypedDict):
    controlOperation: ControlOperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ControlOperationTypeDef](./type_defs.md#controloperationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResetLandingZoneOutputTypeDef

```python
# ResetLandingZoneOutputTypeDef definition

class ResetLandingZoneOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEnabledControlOutputTypeDef

```python
# UpdateEnabledControlOutputTypeDef definition

class UpdateEnabledControlOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateLandingZoneOutputTypeDef

```python
# UpdateLandingZoneOutputTypeDef definition

class UpdateLandingZoneOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableControlInputRequestTypeDef

```python
# EnableControlInputRequestTypeDef definition

class EnableControlInputRequestTypeDef(TypedDict):
    controlIdentifier: str,
    targetIdentifier: str,
    parameters: NotRequired[Sequence[EnabledControlParameterTypeDef]],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: EnabledControlParameterTypeDef](./type_defs.md#enabledcontrolparametertypedef) 
## UpdateEnabledControlInputRequestTypeDef

```python
# UpdateEnabledControlInputRequestTypeDef definition

class UpdateEnabledControlInputRequestTypeDef(TypedDict):
    enabledControlIdentifier: str,
    parameters: Sequence[EnabledControlParameterTypeDef],  # (1)
```

1. See [:material-code-braces: EnabledControlParameterTypeDef](./type_defs.md#enabledcontrolparametertypedef) 
## EnabledControlSummaryTypeDef

```python
# EnabledControlSummaryTypeDef definition

class EnabledControlSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    controlIdentifier: NotRequired[str],
    driftStatusSummary: NotRequired[DriftStatusSummaryTypeDef],  # (1)
    statusSummary: NotRequired[EnablementStatusSummaryTypeDef],  # (2)
    targetIdentifier: NotRequired[str],
```

1. See [:material-code-braces: DriftStatusSummaryTypeDef](./type_defs.md#driftstatussummarytypedef) 
2. See [:material-code-braces: EnablementStatusSummaryTypeDef](./type_defs.md#enablementstatussummarytypedef) 
## EnabledControlDetailsTypeDef

```python
# EnabledControlDetailsTypeDef definition

class EnabledControlDetailsTypeDef(TypedDict):
    arn: NotRequired[str],
    controlIdentifier: NotRequired[str],
    driftStatusSummary: NotRequired[DriftStatusSummaryTypeDef],  # (1)
    parameters: NotRequired[List[EnabledControlParameterSummaryTypeDef]],  # (2)
    statusSummary: NotRequired[EnablementStatusSummaryTypeDef],  # (3)
    targetIdentifier: NotRequired[str],
    targetRegions: NotRequired[List[RegionTypeDef]],  # (4)
```

1. See [:material-code-braces: DriftStatusSummaryTypeDef](./type_defs.md#driftstatussummarytypedef) 
2. See [:material-code-braces: EnabledControlParameterSummaryTypeDef](./type_defs.md#enabledcontrolparametersummarytypedef) 
3. See [:material-code-braces: EnablementStatusSummaryTypeDef](./type_defs.md#enablementstatussummarytypedef) 
4. See [:material-code-braces: RegionTypeDef](./type_defs.md#regiontypedef) 
## GetLandingZoneOperationOutputTypeDef

```python
# GetLandingZoneOperationOutputTypeDef definition

class GetLandingZoneOperationOutputTypeDef(TypedDict):
    operationDetails: LandingZoneOperationDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LandingZoneOperationDetailTypeDef](./type_defs.md#landingzoneoperationdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LandingZoneDetailTypeDef

```python
# LandingZoneDetailTypeDef definition

class LandingZoneDetailTypeDef(TypedDict):
    manifest: Dict[str, Any],
    version: str,
    arn: NotRequired[str],
    driftStatus: NotRequired[LandingZoneDriftStatusSummaryTypeDef],  # (1)
    latestAvailableVersion: NotRequired[str],
    status: NotRequired[LandingZoneStatusType],  # (2)
```

1. See [:material-code-braces: LandingZoneDriftStatusSummaryTypeDef](./type_defs.md#landingzonedriftstatussummarytypedef) 
2. See [:material-code-brackets: LandingZoneStatusType](./literals.md#landingzonestatustype) 
## ListLandingZonesOutputTypeDef

```python
# ListLandingZonesOutputTypeDef definition

class ListLandingZonesOutputTypeDef(TypedDict):
    landingZones: List[LandingZoneSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LandingZoneSummaryTypeDef](./type_defs.md#landingzonesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnabledControlsInputListEnabledControlsPaginateTypeDef

```python
# ListEnabledControlsInputListEnabledControlsPaginateTypeDef definition

class ListEnabledControlsInputListEnabledControlsPaginateTypeDef(TypedDict):
    targetIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLandingZonesInputListLandingZonesPaginateTypeDef

```python
# ListLandingZonesInputListLandingZonesPaginateTypeDef definition

class ListLandingZonesInputListLandingZonesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnabledControlsOutputTypeDef

```python
# ListEnabledControlsOutputTypeDef definition

class ListEnabledControlsOutputTypeDef(TypedDict):
    enabledControls: List[EnabledControlSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnabledControlSummaryTypeDef](./type_defs.md#enabledcontrolsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEnabledControlOutputTypeDef

```python
# GetEnabledControlOutputTypeDef definition

class GetEnabledControlOutputTypeDef(TypedDict):
    enabledControlDetails: EnabledControlDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnabledControlDetailsTypeDef](./type_defs.md#enabledcontroldetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLandingZoneOutputTypeDef

```python
# GetLandingZoneOutputTypeDef definition

class GetLandingZoneOutputTypeDef(TypedDict):
    landingZone: LandingZoneDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LandingZoneDetailTypeDef](./type_defs.md#landingzonedetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
