# Typed dictionaries

> [Index](../README.md) > [ApiGatewayManagementApi](./README.md) > Typed dictionaries

!!! note ""

    Auto-generated documentation for [ApiGatewayManagementApi](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
    type annotations stubs module [types-aiobotocore-apigatewaymanagementapi](https://pypi.org/project/types-aiobotocore-apigatewaymanagementapi/).

## DeleteConnectionRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_apigatewaymanagementapi.type_defs import DeleteConnectionRequestRequestTypeDef

def get_value() -> DeleteConnectionRequestRequestTypeDef:
    return {
        "ConnectionId": ...,
    }
```

```python title="Definition"
class DeleteConnectionRequestRequestTypeDef(TypedDict):
    ConnectionId: str,
```

## ResponseMetadataTypeDef

```python title="Usage Example"
from types_aiobotocore_apigatewaymanagementapi.type_defs import ResponseMetadataTypeDef

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

## GetConnectionRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_apigatewaymanagementapi.type_defs import GetConnectionRequestRequestTypeDef

def get_value() -> GetConnectionRequestRequestTypeDef:
    return {
        "ConnectionId": ...,
    }
```

```python title="Definition"
class GetConnectionRequestRequestTypeDef(TypedDict):
    ConnectionId: str,
```

## IdentityTypeDef

```python title="Usage Example"
from types_aiobotocore_apigatewaymanagementapi.type_defs import IdentityTypeDef

def get_value() -> IdentityTypeDef:
    return {
        "SourceIp": ...,
        "UserAgent": ...,
    }
```

```python title="Definition"
class IdentityTypeDef(TypedDict):
    SourceIp: str,
    UserAgent: str,
```

## PostToConnectionRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_apigatewaymanagementapi.type_defs import PostToConnectionRequestRequestTypeDef

def get_value() -> PostToConnectionRequestRequestTypeDef:
    return {
        "Data": ...,
        "ConnectionId": ...,
    }
```

```python title="Definition"
class PostToConnectionRequestRequestTypeDef(TypedDict):
    Data: Union[str, bytes, IO[Any], StreamingBody],
    ConnectionId: str,
```

## EmptyResponseMetadataTypeDef

```python title="Usage Example"
from types_aiobotocore_apigatewaymanagementapi.type_defs import EmptyResponseMetadataTypeDef

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
## GetConnectionResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_apigatewaymanagementapi.type_defs import GetConnectionResponseTypeDef

def get_value() -> GetConnectionResponseTypeDef:
    return {
        "ConnectedAt": ...,
        "Identity": ...,
        "LastActiveAt": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetConnectionResponseTypeDef(TypedDict):
    ConnectedAt: datetime,
    Identity: IdentityTypeDef,  # (1)
    LastActiveAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
