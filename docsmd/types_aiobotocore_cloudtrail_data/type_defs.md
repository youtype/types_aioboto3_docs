# Type definitions

> [Index](../README.md) > [CloudTrailDataService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CloudTrailDataService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#cloudtraildataservice)
    type annotations stubs module [types-aiobotocore-cloudtrail-data](https://pypi.org/project/types-aiobotocore-cloudtrail-data/).



## AuditEventResultEntryTypeDef

```python
# AuditEventResultEntryTypeDef definition

class AuditEventResultEntryTypeDef(TypedDict):
    eventID: str,
    id: str,
```

## AuditEventTypeDef

```python
# AuditEventTypeDef definition

class AuditEventTypeDef(TypedDict):
    eventData: str,
    id: str,
    eventDataChecksum: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## ResultErrorEntryTypeDef

```python
# ResultErrorEntryTypeDef definition

class ResultErrorEntryTypeDef(TypedDict):
    errorCode: str,
    errorMessage: str,
    id: str,
```

## PutAuditEventsRequestRequestTypeDef

```python
# PutAuditEventsRequestRequestTypeDef definition

class PutAuditEventsRequestRequestTypeDef(TypedDict):
    auditEvents: Sequence[AuditEventTypeDef],  # (1)
    channelArn: str,
    externalId: NotRequired[str],
```

1. See [:material-code-braces: AuditEventTypeDef](./type_defs.md#auditeventtypedef) 
## PutAuditEventsResponseTypeDef

```python
# PutAuditEventsResponseTypeDef definition

class PutAuditEventsResponseTypeDef(TypedDict):
    failed: list[ResultErrorEntryTypeDef],  # (1)
    successful: list[AuditEventResultEntryTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ResultErrorEntryTypeDef](./type_defs.md#resulterrorentrytypedef) 
2. See [:material-code-braces: AuditEventResultEntryTypeDef](./type_defs.md#auditeventresultentrytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 