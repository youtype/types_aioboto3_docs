# Examples

> [Index](../README.md) > [BedrockRuntime](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [BedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#bedrockruntime)
    type annotations stubs module [types-aiobotocore-bedrock-runtime](https://pypi.org/project/types-aiobotocore-bedrock-runtime/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[bedrock-runtime]` package installed.

Write your `BedrockRuntime` code as usual,
type checking and code completion should work out of the box.



```python
# BedrockRuntimeClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("bedrock-runtime") as client:  # (1)
    result = await client.apply_guardrail()  # (2)
```

1. client: [BedrockRuntimeClient](./client.md)
2. result: [:material-code-braces: ApplyGuardrailResponseTypeDef](./type_defs.md#applyguardrailresponsetypedef) 



```python
# ListAsyncInvokesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("bedrock-runtime") as client:  # (1)
    paginator = client.get_paginator("list_async_invokes")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [BedrockRuntimeClient](./client.md)
2. paginator: [ListAsyncInvokesPaginator](./paginators.md#listasyncinvokespaginator)
3. item: [:material-code-braces: ListAsyncInvokesResponseTypeDef](./type_defs.md#listasyncinvokesresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[bedrock-runtime]`
or a standalone `types_aiobotocore_bedrock_runtime` package, you have to explicitly specify
`client: BedrockRuntimeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# BedrockRuntimeClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_bedrock_runtime.client import BedrockRuntimeClient
from types_aiobotocore_bedrock_runtime.type_defs import ApplyGuardrailResponseTypeDef
from types_aiobotocore_bedrock_runtime.type_defs import ApplyGuardrailRequestRequestTypeDef


session = Session()

client: BedrockRuntimeClient
async with session.client("bedrock-runtime") as client:  # (1)
    kwargs: ApplyGuardrailRequestRequestTypeDef = {...}  # (2)
    result: ApplyGuardrailResponseTypeDef = await client.apply_guardrail(**kwargs)  # (3)
```

1. client: [BedrockRuntimeClient](./client.md)
2. kwargs: [:material-code-braces: ApplyGuardrailRequestRequestTypeDef](./type_defs.md#applyguardrailrequestrequesttypedef) 
3. result: [:material-code-braces: ApplyGuardrailResponseTypeDef](./type_defs.md#applyguardrailresponsetypedef) 



```python
# ListAsyncInvokesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_bedrock_runtime.client import BedrockRuntimeClient
from types_aiobotocore_bedrock_runtime.paginator import ListAsyncInvokesPaginator
from types_aiobotocore_bedrock_runtime.type_defs import ListAsyncInvokesResponseTypeDef


session = Session()

client: BedrockRuntimeClient
async with session.client("bedrock-runtime") as client:  # (1)
    paginator: ListAsyncInvokesPaginator = client.get_paginator("list_async_invokes")  # (2)
    async for item in paginator.paginate(...):
        item: ListAsyncInvokesResponseTypeDef
        print(item)  # (3)
```

1. client: [BedrockRuntimeClient](./client.md)
2. paginator: [ListAsyncInvokesPaginator](./paginators.md#listasyncinvokespaginator)
3. item: [:material-code-braces: ListAsyncInvokesResponseTypeDef](./type_defs.md#listasyncinvokesresponsetypedef) 



