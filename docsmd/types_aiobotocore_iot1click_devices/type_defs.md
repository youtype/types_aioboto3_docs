# Type definitions

> [Index](../README.md) > [IoT1ClickDevicesService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [IoT1ClickDevicesService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#iot1clickdevicesservice)
    type annotations stubs module [types-aiobotocore-iot1click-devices](https://pypi.org/project/types-aiobotocore-iot1click-devices/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## ClaimDevicesByClaimCodeRequestRequestTypeDef

```python
# ClaimDevicesByClaimCodeRequestRequestTypeDef definition

class ClaimDevicesByClaimCodeRequestRequestTypeDef(TypedDict):
    ClaimCode: str,
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

## DescribeDeviceRequestRequestTypeDef

```python
# DescribeDeviceRequestRequestTypeDef definition

class DescribeDeviceRequestRequestTypeDef(TypedDict):
    DeviceId: str,
```

## DeviceDescriptionTypeDef

```python
# DeviceDescriptionTypeDef definition

class DeviceDescriptionTypeDef(TypedDict):
    Arn: NotRequired[str],
    Attributes: NotRequired[dict[str, str]],
    DeviceId: NotRequired[str],
    Enabled: NotRequired[bool],
    RemainingLife: NotRequired[float],
    Type: NotRequired[str],
    Tags: NotRequired[dict[str, str]],
```

## DeviceTypeDef

```python
# DeviceTypeDef definition

class DeviceTypeDef(TypedDict):
    Attributes: NotRequired[dict[str, Any]],
    DeviceId: NotRequired[str],
    Type: NotRequired[str],
```

## DeviceMethodTypeDef

```python
# DeviceMethodTypeDef definition

class DeviceMethodTypeDef(TypedDict):
    DeviceType: NotRequired[str],
    MethodName: NotRequired[str],
```

## FinalizeDeviceClaimRequestRequestTypeDef

```python
# FinalizeDeviceClaimRequestRequestTypeDef definition

class FinalizeDeviceClaimRequestRequestTypeDef(TypedDict):
    DeviceId: str,
    Tags: NotRequired[Mapping[str, str]],
```

## GetDeviceMethodsRequestRequestTypeDef

```python
# GetDeviceMethodsRequestRequestTypeDef definition

class GetDeviceMethodsRequestRequestTypeDef(TypedDict):
    DeviceId: str,
```

## InitiateDeviceClaimRequestRequestTypeDef

```python
# InitiateDeviceClaimRequestRequestTypeDef definition

class InitiateDeviceClaimRequestRequestTypeDef(TypedDict):
    DeviceId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListDevicesRequestRequestTypeDef

```python
# ListDevicesRequestRequestTypeDef definition

class ListDevicesRequestRequestTypeDef(TypedDict):
    DeviceType: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UnclaimDeviceRequestRequestTypeDef

```python
# UnclaimDeviceRequestRequestTypeDef definition

class UnclaimDeviceRequestRequestTypeDef(TypedDict):
    DeviceId: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateDeviceStateRequestRequestTypeDef

```python
# UpdateDeviceStateRequestRequestTypeDef definition

class UpdateDeviceStateRequestRequestTypeDef(TypedDict):
    DeviceId: str,
    Enabled: NotRequired[bool],
```

## ClaimDevicesByClaimCodeResponseTypeDef

```python
# ClaimDevicesByClaimCodeResponseTypeDef definition

class ClaimDevicesByClaimCodeResponseTypeDef(TypedDict):
    ClaimCode: str,
    Total: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FinalizeDeviceClaimResponseTypeDef

```python
# FinalizeDeviceClaimResponseTypeDef definition

class FinalizeDeviceClaimResponseTypeDef(TypedDict):
    State: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InitiateDeviceClaimResponseTypeDef

```python
# InitiateDeviceClaimResponseTypeDef definition

class InitiateDeviceClaimResponseTypeDef(TypedDict):
    State: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InvokeDeviceMethodResponseTypeDef

```python
# InvokeDeviceMethodResponseTypeDef definition

class InvokeDeviceMethodResponseTypeDef(TypedDict):
    DeviceMethodResponse: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UnclaimDeviceResponseTypeDef

```python
# UnclaimDeviceResponseTypeDef definition

class UnclaimDeviceResponseTypeDef(TypedDict):
    State: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDeviceResponseTypeDef

```python
# DescribeDeviceResponseTypeDef definition

class DescribeDeviceResponseTypeDef(TypedDict):
    DeviceDescription: DeviceDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeviceDescriptionTypeDef](./type_defs.md#devicedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDevicesResponseTypeDef

```python
# ListDevicesResponseTypeDef definition

class ListDevicesResponseTypeDef(TypedDict):
    Devices: list[DeviceDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DeviceDescriptionTypeDef](./type_defs.md#devicedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeviceEventTypeDef

```python
# DeviceEventTypeDef definition

class DeviceEventTypeDef(TypedDict):
    Device: NotRequired[DeviceTypeDef],  # (1)
    StdEvent: NotRequired[str],
```

1. See [:material-code-braces: DeviceTypeDef](./type_defs.md#devicetypedef) 
## GetDeviceMethodsResponseTypeDef

```python
# GetDeviceMethodsResponseTypeDef definition

class GetDeviceMethodsResponseTypeDef(TypedDict):
    DeviceMethods: list[DeviceMethodTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeviceMethodTypeDef](./type_defs.md#devicemethodtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InvokeDeviceMethodRequestRequestTypeDef

```python
# InvokeDeviceMethodRequestRequestTypeDef definition

class InvokeDeviceMethodRequestRequestTypeDef(TypedDict):
    DeviceId: str,
    DeviceMethod: NotRequired[DeviceMethodTypeDef],  # (1)
    DeviceMethodParameters: NotRequired[str],
```

1. See [:material-code-braces: DeviceMethodTypeDef](./type_defs.md#devicemethodtypedef) 
## ListDevicesRequestPaginateTypeDef

```python
# ListDevicesRequestPaginateTypeDef definition

class ListDevicesRequestPaginateTypeDef(TypedDict):
    DeviceType: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDeviceEventsRequestPaginateTypeDef

```python
# ListDeviceEventsRequestPaginateTypeDef definition

class ListDeviceEventsRequestPaginateTypeDef(TypedDict):
    DeviceId: str,
    FromTimeStamp: TimestampTypeDef,
    ToTimeStamp: TimestampTypeDef,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDeviceEventsRequestRequestTypeDef

```python
# ListDeviceEventsRequestRequestTypeDef definition

class ListDeviceEventsRequestRequestTypeDef(TypedDict):
    DeviceId: str,
    FromTimeStamp: TimestampTypeDef,
    ToTimeStamp: TimestampTypeDef,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListDeviceEventsResponseTypeDef

```python
# ListDeviceEventsResponseTypeDef definition

class ListDeviceEventsResponseTypeDef(TypedDict):
    Events: list[DeviceEventTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DeviceEventTypeDef](./type_defs.md#deviceeventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 