# Examples

> [Index](../README.md) > [AgentsforBedrockRuntime](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AgentsforBedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime)
    type annotations stubs module [types-aiobotocore-bedrock-agent-runtime](https://pypi.org/project/types-aiobotocore-bedrock-agent-runtime/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[bedrock-agent-runtime]` package installed.

Write your `AgentsforBedrockRuntime` code as usual,
type checking and code completion should work out of the box.



```python
# AgentsforBedrockRuntimeClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("bedrock-agent-runtime") as client:  # (1)
    result = await client.invoke_agent()  # (2)
```

1. client: [AgentsforBedrockRuntimeClient](./client.md)
2. result: [:material-code-braces: InvokeAgentResponseTypeDef](./type_defs.md#invokeagentresponsetypedef) 



```python
# RetrievePaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("bedrock-agent-runtime") as client:  # (1)
    paginator = client.get_paginator("retrieve")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AgentsforBedrockRuntimeClient](./client.md)
2. paginator: [RetrievePaginator](./paginators.md#retrievepaginator)
3. item: [:material-code-braces: RetrieveResponseTypeDef](./type_defs.md#retrieveresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[bedrock-agent-runtime]`
or a standalone `types_aiobotocore_bedrock_agent_runtime` package, you have to explicitly specify
`client: AgentsforBedrockRuntimeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# AgentsforBedrockRuntimeClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_bedrock_agent_runtime.client import AgentsforBedrockRuntimeClient
from types_aiobotocore_bedrock_agent_runtime.type_defs import InvokeAgentResponseTypeDef
from types_aiobotocore_bedrock_agent_runtime.type_defs import InvokeAgentRequestRequestTypeDef


session = Session()

client: AgentsforBedrockRuntimeClient
async with session.client("bedrock-agent-runtime") as client:  # (1)
    kwargs: InvokeAgentRequestRequestTypeDef = {...}  # (2)
    result: InvokeAgentResponseTypeDef = await client.invoke_agent(**kwargs)  # (3)
```

1. client: [AgentsforBedrockRuntimeClient](./client.md)
2. kwargs: [:material-code-braces: InvokeAgentRequestRequestTypeDef](./type_defs.md#invokeagentrequestrequesttypedef) 
3. result: [:material-code-braces: InvokeAgentResponseTypeDef](./type_defs.md#invokeagentresponsetypedef) 



```python
# RetrievePaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_bedrock_agent_runtime.client import AgentsforBedrockRuntimeClient
from types_aiobotocore_bedrock_agent_runtime.paginator import RetrievePaginator
from types_aiobotocore_bedrock_agent_runtime.type_defs import RetrieveResponseTypeDef


session = Session()

client: AgentsforBedrockRuntimeClient
async with session.client("bedrock-agent-runtime") as client:  # (1)
    paginator: RetrievePaginator = client.get_paginator("retrieve")  # (2)
    async for item in paginator.paginate(...):
        item: RetrieveResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockRuntimeClient](./client.md)
2. paginator: [RetrievePaginator](./paginators.md#retrievepaginator)
3. item: [:material-code-braces: RetrieveResponseTypeDef](./type_defs.md#retrieveresponsetypedef) 




