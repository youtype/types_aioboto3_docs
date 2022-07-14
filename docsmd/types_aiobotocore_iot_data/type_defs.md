# Typed dictionaries

> [Index](../README.md) > [IoTDataPlane](./README.md) > Typed dictionaries

!!! note ""

    Auto-generated documentation for [IoTDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane)
    type annotations stubs module [types-aiobotocore-iot-data](https://pypi.org/project/types-aiobotocore-iot-data/).

## DeleteThingShadowRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_iot_data.type_defs import DeleteThingShadowRequestRequestTypeDef

def get_value() -> DeleteThingShadowRequestRequestTypeDef:
    return {
        "thingName": ...,
    }
```

```python title="Definition"
class DeleteThingShadowRequestRequestTypeDef(TypedDict):
    thingName: str,
    shadowName: NotRequired[str],
```

## ResponseMetadataTypeDef

```python title="Usage Example"
from types_aiobotocore_iot_data.type_defs import ResponseMetadataTypeDef

def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
        "HostId": ...,
        "HTTPStatusCode": ...,
        "HTTPHeaders": ...,
        "RetryAttempts": ...,
    }
```

```python title="Definition"
class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## GetRetainedMessageRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_iot_data.type_defs import GetRetainedMessageRequestRequestTypeDef

def get_value() -> GetRetainedMessageRequestRequestTypeDef:
    return {
        "topic": ...,
    }
```

```python title="Definition"
class GetRetainedMessageRequestRequestTypeDef(TypedDict):
    topic: str,
```

## GetThingShadowRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_iot_data.type_defs import GetThingShadowRequestRequestTypeDef

def get_value() -> GetThingShadowRequestRequestTypeDef:
    return {
        "thingName": ...,
    }
```

```python title="Definition"
class GetThingShadowRequestRequestTypeDef(TypedDict):
    thingName: str,
    shadowName: NotRequired[str],
```

## ListNamedShadowsForThingRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_iot_data.type_defs import ListNamedShadowsForThingRequestRequestTypeDef

def get_value() -> ListNamedShadowsForThingRequestRequestTypeDef:
    return {
        "thingName": ...,
    }
```

```python title="Definition"
class ListNamedShadowsForThingRequestRequestTypeDef(TypedDict):
    thingName: str,
    nextToken: NotRequired[str],
    pageSize: NotRequired[int],
```

## PaginatorConfigTypeDef

```python title="Usage Example"
from types_aiobotocore_iot_data.type_defs import PaginatorConfigTypeDef

def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }
```

```python title="Definition"
class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListRetainedMessagesRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_iot_data.type_defs import ListRetainedMessagesRequestRequestTypeDef

def get_value() -> ListRetainedMessagesRequestRequestTypeDef:
    return {
        "nextToken": ...,
    }
```

```python title="Definition"
class ListRetainedMessagesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## RetainedMessageSummaryTypeDef

```python title="Usage Example"
from types_aiobotocore_iot_data.type_defs import RetainedMessageSummaryTypeDef

def get_value() -> RetainedMessageSummaryTypeDef:
    return {
        "topic": ...,
    }
```

```python title="Definition"
class RetainedMessageSummaryTypeDef(TypedDict):
    topic: NotRequired[str],
    payloadSize: NotRequired[int],
    qos: NotRequired[int],
    lastModifiedTime: NotRequired[int],
```

## PublishRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_iot_data.type_defs import PublishRequestRequestTypeDef

def get_value() -> PublishRequestRequestTypeDef:
    return {
        "topic": ...,
    }
```

```python title="Definition"
class PublishRequestRequestTypeDef(TypedDict):
    topic: str,
    qos: NotRequired[int],
    retain: NotRequired[bool],
    payload: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
```

## UpdateThingShadowRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_iot_data.type_defs import UpdateThingShadowRequestRequestTypeDef

def get_value() -> UpdateThingShadowRequestRequestTypeDef:
    return {
        "thingName": ...,
        "payload": ...,
    }
```

```python title="Definition"
class UpdateThingShadowRequestRequestTypeDef(TypedDict):
    thingName: str,
    payload: Union[str, bytes, IO[Any], StreamingBody],
    shadowName: NotRequired[str],
```

## DeleteThingShadowResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_iot_data.type_defs import DeleteThingShadowResponseTypeDef

def get_value() -> DeleteThingShadowResponseTypeDef:
    return {
        "payload": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DeleteThingShadowResponseTypeDef(TypedDict):
    payload: StreamingBody,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python title="Usage Example"
from types_aiobotocore_iot_data.type_defs import EmptyResponseMetadataTypeDef

def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRetainedMessageResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_iot_data.type_defs import GetRetainedMessageResponseTypeDef

def get_value() -> GetRetainedMessageResponseTypeDef:
    return {
        "topic": ...,
        "payload": ...,
        "qos": ...,
        "lastModifiedTime": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetRetainedMessageResponseTypeDef(TypedDict):
    topic: str,
    payload: bytes,
    qos: int,
    lastModifiedTime: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetThingShadowResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_iot_data.type_defs import GetThingShadowResponseTypeDef

def get_value() -> GetThingShadowResponseTypeDef:
    return {
        "payload": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetThingShadowResponseTypeDef(TypedDict):
    payload: StreamingBody,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNamedShadowsForThingResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_iot_data.type_defs import ListNamedShadowsForThingResponseTypeDef

def get_value() -> ListNamedShadowsForThingResponseTypeDef:
    return {
        "results": ...,
        "nextToken": ...,
        "timestamp": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListNamedShadowsForThingResponseTypeDef(TypedDict):
    results: List[str],
    nextToken: str,
    timestamp: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateThingShadowResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_iot_data.type_defs import UpdateThingShadowResponseTypeDef

def get_value() -> UpdateThingShadowResponseTypeDef:
    return {
        "payload": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class UpdateThingShadowResponseTypeDef(TypedDict):
    payload: StreamingBody,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef

```python title="Usage Example"
from types_aiobotocore_iot_data.type_defs import ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef

def get_value() -> ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }
```

```python title="Definition"
class ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRetainedMessagesResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_iot_data.type_defs import ListRetainedMessagesResponseTypeDef

def get_value() -> ListRetainedMessagesResponseTypeDef:
    return {
        "retainedTopics": ...,
        "nextToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListRetainedMessagesResponseTypeDef(TypedDict):
    retainedTopics: List[RetainedMessageSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RetainedMessageSummaryTypeDef](./type_defs.md#retainedmessagesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
