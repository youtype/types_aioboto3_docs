# BedrockRuntimeClient

> [Index](../README.md) > [BedrockRuntime](./README.md) > BedrockRuntimeClient

!!! note ""

    Auto-generated documentation for [BedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#bedrockruntime)
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
        client.exceptions.ConflictException,
        client.exceptions.InternalServerException,
        client.exceptions.ModelErrorException,
        client.exceptions.ModelNotReadyException,
        client.exceptions.ModelStreamErrorException,
        client.exceptions.ModelTimeoutException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ServiceUnavailableException,
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



Type annotations and code completion for `#!python session.client("bedrock-runtime").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("bedrock-runtime").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client)

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


### apply\_guardrail

The action to apply a guardrail.

Type annotations and code completion for `#!python session.client("bedrock-runtime").apply_guardrail` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client)

```python
# apply_guardrail method definition

await def apply_guardrail(
    self,
    *,
    guardrailIdentifier: str,
    guardrailVersion: str,
    source: GuardrailContentSourceType,  # (1)
    content: Sequence[GuardrailContentBlockTypeDef],  # (2)
) -> ApplyGuardrailResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: GuardrailContentSourceType](./literals.md#guardrailcontentsourcetype) 
2. See [:material-code-braces: GuardrailContentBlockTypeDef](./type_defs.md#guardrailcontentblocktypedef) 
3. See [:material-code-braces: ApplyGuardrailResponseTypeDef](./type_defs.md#applyguardrailresponsetypedef) 


```python
# apply_guardrail method usage example with argument unpacking

kwargs: ApplyGuardrailRequestRequestTypeDef = {  # (1)
    "guardrailIdentifier": ...,
    "guardrailVersion": ...,
    "source": ...,
    "content": ...,
}

parent.apply_guardrail(**kwargs)
```

1. See [:material-code-braces: ApplyGuardrailRequestRequestTypeDef](./type_defs.md#applyguardrailrequestrequesttypedef) 

### converse

Sends messages to the specified Amazon Bedrock model.

Type annotations and code completion for `#!python session.client("bedrock-runtime").converse` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client)

```python
# converse method definition

await def converse(
    self,
    *,
    modelId: str,
    messages: Sequence[MessageUnionTypeDef] = ...,  # (1)
    system: Sequence[SystemContentBlockTypeDef] = ...,  # (2)
    inferenceConfig: InferenceConfigurationTypeDef = ...,  # (3)
    toolConfig: ToolConfigurationTypeDef = ...,  # (4)
    guardrailConfig: GuardrailConfigurationTypeDef = ...,  # (5)
    additionalModelRequestFields: Mapping[str, Any] = ...,
    promptVariables: Mapping[str, PromptVariableValuesTypeDef] = ...,  # (6)
    additionalModelResponseFieldPaths: Sequence[str] = ...,
    requestMetadata: Mapping[str, str] = ...,
    performanceConfig: PerformanceConfigurationTypeDef = ...,  # (7)
) -> ConverseResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) [:material-code-braces: MessageOutputTypeDef](./type_defs.md#messageoutputtypedef) 
2. See [:material-code-braces: SystemContentBlockTypeDef](./type_defs.md#systemcontentblocktypedef) 
3. See [:material-code-braces: InferenceConfigurationTypeDef](./type_defs.md#inferenceconfigurationtypedef) 
4. See [:material-code-braces: ToolConfigurationTypeDef](./type_defs.md#toolconfigurationtypedef) 
5. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef) 
6. See [:material-code-braces: PromptVariableValuesTypeDef](./type_defs.md#promptvariablevaluestypedef) 
7. See [:material-code-braces: PerformanceConfigurationTypeDef](./type_defs.md#performanceconfigurationtypedef) 
8. See [:material-code-braces: ConverseResponseTypeDef](./type_defs.md#converseresponsetypedef) 


```python
# converse method usage example with argument unpacking

kwargs: ConverseRequestRequestTypeDef = {  # (1)
    "modelId": ...,
}

parent.converse(**kwargs)
```

1. See [:material-code-braces: ConverseRequestRequestTypeDef](./type_defs.md#converserequestrequesttypedef) 

### converse\_stream

Sends messages to the specified Amazon Bedrock model and returns the response
in a stream.

Type annotations and code completion for `#!python session.client("bedrock-runtime").converse_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client)

```python
# converse_stream method definition

await def converse_stream(
    self,
    *,
    modelId: str,
    messages: Sequence[MessageTypeDef] = ...,  # (1)
    system: Sequence[SystemContentBlockTypeDef] = ...,  # (2)
    inferenceConfig: InferenceConfigurationTypeDef = ...,  # (3)
    toolConfig: ToolConfigurationTypeDef = ...,  # (4)
    guardrailConfig: GuardrailStreamConfigurationTypeDef = ...,  # (5)
    additionalModelRequestFields: Mapping[str, Any] = ...,
    promptVariables: Mapping[str, PromptVariableValuesTypeDef] = ...,  # (6)
    additionalModelResponseFieldPaths: Sequence[str] = ...,
    requestMetadata: Mapping[str, str] = ...,
    performanceConfig: PerformanceConfigurationTypeDef = ...,  # (7)
) -> ConverseStreamResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
2. See [:material-code-braces: SystemContentBlockTypeDef](./type_defs.md#systemcontentblocktypedef) 
3. See [:material-code-braces: InferenceConfigurationTypeDef](./type_defs.md#inferenceconfigurationtypedef) 
4. See [:material-code-braces: ToolConfigurationTypeDef](./type_defs.md#toolconfigurationtypedef) 
5. See [:material-code-braces: GuardrailStreamConfigurationTypeDef](./type_defs.md#guardrailstreamconfigurationtypedef) 
6. See [:material-code-braces: PromptVariableValuesTypeDef](./type_defs.md#promptvariablevaluestypedef) 
7. See [:material-code-braces: PerformanceConfigurationTypeDef](./type_defs.md#performanceconfigurationtypedef) 
8. See [:material-code-braces: ConverseStreamResponseTypeDef](./type_defs.md#conversestreamresponsetypedef) 


```python
# converse_stream method usage example with argument unpacking

kwargs: ConverseStreamRequestRequestTypeDef = {  # (1)
    "modelId": ...,
}

parent.converse_stream(**kwargs)
```

1. See [:material-code-braces: ConverseStreamRequestRequestTypeDef](./type_defs.md#conversestreamrequestrequesttypedef) 

### get\_async\_invoke

Retrieve information about an asynchronous invocation.

Type annotations and code completion for `#!python session.client("bedrock-runtime").get_async_invoke` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client)

```python
# get_async_invoke method definition

await def get_async_invoke(
    self,
    *,
    invocationArn: str,
) -> GetAsyncInvokeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAsyncInvokeResponseTypeDef](./type_defs.md#getasyncinvokeresponsetypedef) 


```python
# get_async_invoke method usage example with argument unpacking

kwargs: GetAsyncInvokeRequestRequestTypeDef = {  # (1)
    "invocationArn": ...,
}

parent.get_async_invoke(**kwargs)
```

1. See [:material-code-braces: GetAsyncInvokeRequestRequestTypeDef](./type_defs.md#getasyncinvokerequestrequesttypedef) 

### invoke\_model

Invokes the specified Amazon Bedrock model to run inference using the prompt
and inference parameters provided in the request body.

Type annotations and code completion for `#!python session.client("bedrock-runtime").invoke_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client)

```python
# invoke_model method definition

await def invoke_model(
    self,
    *,
    modelId: str,
    body: BlobTypeDef = ...,
    contentType: str = ...,
    accept: str = ...,
    trace: TraceType = ...,  # (1)
    guardrailIdentifier: str = ...,
    guardrailVersion: str = ...,
    performanceConfigLatency: PerformanceConfigLatencyType = ...,  # (2)
) -> InvokeModelResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: TraceType](./literals.md#tracetype) 
2. See [:material-code-brackets: PerformanceConfigLatencyType](./literals.md#performanceconfiglatencytype) 
3. See [:material-code-braces: InvokeModelResponseTypeDef](./type_defs.md#invokemodelresponsetypedef) 


```python
# invoke_model method usage example with argument unpacking

kwargs: InvokeModelRequestRequestTypeDef = {  # (1)
    "modelId": ...,
}

parent.invoke_model(**kwargs)
```

1. See [:material-code-braces: InvokeModelRequestRequestTypeDef](./type_defs.md#invokemodelrequestrequesttypedef) 

### invoke\_model\_with\_response\_stream

Invoke the specified Amazon Bedrock model to run inference using the prompt and
inference parameters provided in the request body.

Type annotations and code completion for `#!python session.client("bedrock-runtime").invoke_model_with_response_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client)

```python
# invoke_model_with_response_stream method definition

await def invoke_model_with_response_stream(
    self,
    *,
    modelId: str,
    body: BlobTypeDef = ...,
    contentType: str = ...,
    accept: str = ...,
    trace: TraceType = ...,  # (1)
    guardrailIdentifier: str = ...,
    guardrailVersion: str = ...,
    performanceConfigLatency: PerformanceConfigLatencyType = ...,  # (2)
) -> InvokeModelWithResponseStreamResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: TraceType](./literals.md#tracetype) 
2. See [:material-code-brackets: PerformanceConfigLatencyType](./literals.md#performanceconfiglatencytype) 
3. See [:material-code-braces: InvokeModelWithResponseStreamResponseTypeDef](./type_defs.md#invokemodelwithresponsestreamresponsetypedef) 


```python
# invoke_model_with_response_stream method usage example with argument unpacking

kwargs: InvokeModelWithResponseStreamRequestRequestTypeDef = {  # (1)
    "modelId": ...,
}

parent.invoke_model_with_response_stream(**kwargs)
```

1. See [:material-code-braces: InvokeModelWithResponseStreamRequestRequestTypeDef](./type_defs.md#invokemodelwithresponsestreamrequestrequesttypedef) 

### list\_async\_invokes

Lists asynchronous invocations.

Type annotations and code completion for `#!python session.client("bedrock-runtime").list_async_invokes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client)

```python
# list_async_invokes method definition

await def list_async_invokes(
    self,
    *,
    submitTimeAfter: TimestampTypeDef = ...,
    submitTimeBefore: TimestampTypeDef = ...,
    statusEquals: AsyncInvokeStatusType = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
    sortBy: SortAsyncInvocationByType = ...,  # (2)
    sortOrder: SortOrderType = ...,  # (3)
) -> ListAsyncInvokesResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: AsyncInvokeStatusType](./literals.md#asyncinvokestatustype) 
2. See [:material-code-brackets: SortAsyncInvocationByType](./literals.md#sortasyncinvocationbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListAsyncInvokesResponseTypeDef](./type_defs.md#listasyncinvokesresponsetypedef) 


```python
# list_async_invokes method usage example with argument unpacking

kwargs: ListAsyncInvokesRequestRequestTypeDef = {  # (1)
    "submitTimeAfter": ...,
}

parent.list_async_invokes(**kwargs)
```

1. See [:material-code-braces: ListAsyncInvokesRequestRequestTypeDef](./type_defs.md#listasyncinvokesrequestrequesttypedef) 

### start\_async\_invoke

Starts an asynchronous invocation.

Type annotations and code completion for `#!python session.client("bedrock-runtime").start_async_invoke` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client)

```python
# start_async_invoke method definition

await def start_async_invoke(
    self,
    *,
    modelId: str,
    modelInput: Mapping[str, Any],
    outputDataConfig: AsyncInvokeOutputDataConfigTypeDef,  # (1)
    clientRequestToken: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> StartAsyncInvokeResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AsyncInvokeOutputDataConfigTypeDef](./type_defs.md#asyncinvokeoutputdataconfigtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: StartAsyncInvokeResponseTypeDef](./type_defs.md#startasyncinvokeresponsetypedef) 


```python
# start_async_invoke method usage example with argument unpacking

kwargs: StartAsyncInvokeRequestRequestTypeDef = {  # (1)
    "modelId": ...,
    "modelInput": ...,
    "outputDataConfig": ...,
}

parent.start_async_invoke(**kwargs)
```

1. See [:material-code-braces: StartAsyncInvokeRequestRequestTypeDef](./type_defs.md#startasyncinvokerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("bedrock-runtime").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("bedrock-runtime").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.client("bedrock-runtime").get_paginator` method with overloads.

- `client.get_paginator("list_async_invokes")` -> [ListAsyncInvokesPaginator](./paginators.md#listasyncinvokespaginator)


