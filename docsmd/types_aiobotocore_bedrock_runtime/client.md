# BedrockRuntimeClient

> [Index](../README.md) > [BedrockRuntime](./README.md) > BedrockRuntimeClient

!!! note ""

    Auto-generated documentation for [BedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime)
    type annotations stubs module [types-aiobotocore-bedrock-runtime](https://pypi.org/project/types-aiobotocore-bedrock-runtime/).

## BedrockRuntimeClient

Type annotations and code completion for `#!python session.client("bedrock-runtime")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client)

```python
# BedrockRuntimeClient usage example

from aioboto3.session import Session
from types_aiobotocore_bedrock_runtime.client import BedrockRuntimeClient

session = Session()
async with session.client("bedrock-runtime") as client:
    client: BedrockRuntimeClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("bedrock-runtime").exceptions` structure.

```python
# BedrockRuntimeClient.exceptions usage example

async with session.client("bedrock-runtime") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.InternalServerException,
        client.exceptions.ModelErrorException,
        client.exceptions.ModelNotReadyException,
        client.exceptions.ModelStreamErrorException,
        client.exceptions.ModelTimeoutException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# BedrockRuntimeClient.exceptions type checking example

from types_aiobotocore_bedrock_runtime.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.client("bedrock-runtime").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.client("bedrock-runtime").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.client("bedrock-runtime").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client.generate_presigned_url)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### invoke\_model

Invokes the specified Bedrock model to run inference using the input provided
in the request
body.

Type annotations and code completion for `#!python session.client("bedrock-runtime").invoke_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client.invoke_model)

```python
# invoke_model method definition

await def invoke_model(
    self,
    *,
    body: Union[str, bytes, IO[Any], StreamingBody],
    modelId: str,
    contentType: str = ...,
    accept: str = ...,
) -> InvokeModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: InvokeModelResponseTypeDef](./type_defs.md#invokemodelresponsetypedef) 


```python
# invoke_model method usage example with argument unpacking

kwargs: InvokeModelRequestRequestTypeDef = {  # (1)
    "body": ...,
    "modelId": ...,
}

parent.invoke_model(**kwargs)
```

1. See [:material-code-braces: InvokeModelRequestRequestTypeDef](./type_defs.md#invokemodelrequestrequesttypedef) 

### invoke\_model\_with\_response\_stream

Invoke the specified Bedrock model to run inference using the input provided.

Type annotations and code completion for `#!python session.client("bedrock-runtime").invoke_model_with_response_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client.invoke_model_with_response_stream)

```python
# invoke_model_with_response_stream method definition

await def invoke_model_with_response_stream(
    self,
    *,
    body: Union[str, bytes, IO[Any], StreamingBody],
    modelId: str,
    contentType: str = ...,
    accept: str = ...,
) -> InvokeModelWithResponseStreamResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: InvokeModelWithResponseStreamResponseTypeDef](./type_defs.md#invokemodelwithresponsestreamresponsetypedef) 


```python
# invoke_model_with_response_stream method usage example with argument unpacking

kwargs: InvokeModelWithResponseStreamRequestRequestTypeDef = {  # (1)
    "body": ...,
    "modelId": ...,
}

parent.invoke_model_with_response_stream(**kwargs)
```

1. See [:material-code-braces: InvokeModelWithResponseStreamRequestRequestTypeDef](./type_defs.md#invokemodelwithresponsestreamrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("bedrock-runtime").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> BedrockRuntimeClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("bedrock-runtime").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





