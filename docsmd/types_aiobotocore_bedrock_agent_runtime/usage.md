# Examples

> [Index](../README.md) > [AgentsforBedrockRuntime](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AgentsforBedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#agentsforbedrockruntime)
    type annotations stubs module [types-aiobotocore-bedrock-agent-runtime](https://pypi.org/project/types-aiobotocore-bedrock-agent-runtime/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[bedrock-agent-runtime]` package installed.

Write your `AgentsforBedrockRuntime` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# AgentsforBedrockRuntimeClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("bedrock-agent-runtime") as client:  # (1)
    result = await client.generate_query()  # (2)
```

1. client: [AgentsforBedrockRuntimeClient](./client.md)
2. result: [:material-code-braces: GenerateQueryResponseTypeDef](./type_defs.md#generatequeryresponsetypedef)



#### Paginator usage example

```python
# GetAgentMemoryPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("bedrock-agent-runtime") as client:  # (1)
    paginator = client.get_paginator("get_agent_memory")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AgentsforBedrockRuntimeClient](./client.md)
2. paginator: [GetAgentMemoryPaginator](./paginators.md#getagentmemorypaginator)
3. item: [:material-code-braces: GetAgentMemoryResponseTypeDef](./type_defs.md#getagentmemoryresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[bedrock-agent-runtime]`
or a standalone `types_aiobotocore_bedrock_agent_runtime` package, you have to explicitly specify
`client: AgentsforBedrockRuntimeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# AgentsforBedrockRuntimeClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_bedrock_agent_runtime.client import AgentsforBedrockRuntimeClient
from types_aiobotocore_bedrock_agent_runtime.type_defs import GenerateQueryResponseTypeDef
from types_aiobotocore_bedrock_agent_runtime.type_defs import GenerateQueryRequestTypeDef


session = Session()

client: AgentsforBedrockRuntimeClient
async with session.client("bedrock-agent-runtime") as client:  # (1)
    kwargs: GenerateQueryRequestTypeDef = {...}  # (2)
    result: GenerateQueryResponseTypeDef = await client.generate_query(**kwargs)  # (3)
```

1. client: [AgentsforBedrockRuntimeClient](./client.md)
2. kwargs: [:material-code-braces: GenerateQueryRequestTypeDef](./type_defs.md#generatequeryrequesttypedef)
3. result: [:material-code-braces: GenerateQueryResponseTypeDef](./type_defs.md#generatequeryresponsetypedef)



#### Paginator usage example

```python
# GetAgentMemoryPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_bedrock_agent_runtime.client import AgentsforBedrockRuntimeClient
from types_aiobotocore_bedrock_agent_runtime.paginator import GetAgentMemoryPaginator
from types_aiobotocore_bedrock_agent_runtime.type_defs import GetAgentMemoryResponseTypeDef


session = Session()

client: AgentsforBedrockRuntimeClient
async with session.client("bedrock-agent-runtime") as client:  # (1)
    paginator: GetAgentMemoryPaginator = client.get_paginator("get_agent_memory")  # (2)
    async for item in paginator.paginate(...):
        item: GetAgentMemoryResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockRuntimeClient](./client.md)
2. paginator: [GetAgentMemoryPaginator](./paginators.md#getagentmemorypaginator)
3. item: [:material-code-braces: GetAgentMemoryResponseTypeDef](./type_defs.md#getagentmemoryresponsetypedef)




