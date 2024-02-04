# Type definitions

> [Index](../README.md) > [BedrockRuntime](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [BedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime)
    type annotations stubs module [types-aiobotocore-bedrock-runtime](https://pypi.org/project/types-aiobotocore-bedrock-runtime/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```




## InternalServerExceptionTypeDef

```python
# InternalServerExceptionTypeDef definition

class InternalServerExceptionTypeDef(TypedDict):
    message: NotRequired[str],
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

## ModelStreamErrorExceptionTypeDef

```python
# ModelStreamErrorExceptionTypeDef definition

class ModelStreamErrorExceptionTypeDef(TypedDict):
    message: NotRequired[str],
    originalStatusCode: NotRequired[int],
    originalMessage: NotRequired[str],
```

## ModelTimeoutExceptionTypeDef

```python
# ModelTimeoutExceptionTypeDef definition

class ModelTimeoutExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## PayloadPartTypeDef

```python
# PayloadPartTypeDef definition

class PayloadPartTypeDef(TypedDict):
    bytes: NotRequired[bytes],
```

## ThrottlingExceptionTypeDef

```python
# ThrottlingExceptionTypeDef definition

class ThrottlingExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## ValidationExceptionTypeDef

```python
# ValidationExceptionTypeDef definition

class ValidationExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## InvokeModelRequestRequestTypeDef

```python
# InvokeModelRequestRequestTypeDef definition

class InvokeModelRequestRequestTypeDef(TypedDict):
    body: Union[str, bytes, IO[Any], StreamingBody],
    modelId: str,
    contentType: NotRequired[str],
    accept: NotRequired[str],
```

## InvokeModelWithResponseStreamRequestRequestTypeDef

```python
# InvokeModelWithResponseStreamRequestRequestTypeDef definition

class InvokeModelWithResponseStreamRequestRequestTypeDef(TypedDict):
    body: Union[str, bytes, IO[Any], StreamingBody],
    modelId: str,
    contentType: NotRequired[str],
    accept: NotRequired[str],
```

## InvokeModelResponseTypeDef

```python
# InvokeModelResponseTypeDef definition

class InvokeModelResponseTypeDef(TypedDict):
    body: StreamingBody,
    contentType: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResponseStreamTypeDef

```python
# ResponseStreamTypeDef definition

class ResponseStreamTypeDef(TypedDict):
    chunk: NotRequired[PayloadPartTypeDef],  # (1)
    internalServerException: NotRequired[InternalServerExceptionTypeDef],  # (2)
    modelStreamErrorException: NotRequired[ModelStreamErrorExceptionTypeDef],  # (3)
    validationException: NotRequired[ValidationExceptionTypeDef],  # (4)
    throttlingException: NotRequired[ThrottlingExceptionTypeDef],  # (5)
    modelTimeoutException: NotRequired[ModelTimeoutExceptionTypeDef],  # (6)
```

1. See [:material-code-braces: PayloadPartTypeDef](./type_defs.md#payloadparttypedef) 
2. See [:material-code-braces: InternalServerExceptionTypeDef](./type_defs.md#internalserverexceptiontypedef) 
3. See [:material-code-braces: ModelStreamErrorExceptionTypeDef](./type_defs.md#modelstreamerrorexceptiontypedef) 
4. See [:material-code-braces: ValidationExceptionTypeDef](./type_defs.md#validationexceptiontypedef) 
5. See [:material-code-braces: ThrottlingExceptionTypeDef](./type_defs.md#throttlingexceptiontypedef) 
6. See [:material-code-braces: ModelTimeoutExceptionTypeDef](./type_defs.md#modeltimeoutexceptiontypedef) 
## InvokeModelWithResponseStreamResponseTypeDef

```python
# InvokeModelWithResponseStreamResponseTypeDef definition

class InvokeModelWithResponseStreamResponseTypeDef(TypedDict):
    body: AioEventStream[ResponseStreamTypeDef],  # (1)
    contentType: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResponseStreamTypeDef](./type_defs.md#responsestreamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
