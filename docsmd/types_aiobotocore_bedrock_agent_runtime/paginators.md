# Paginators

> [Index](../README.md) > [AgentsforBedrockRuntime](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [AgentsforBedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#agentsforbedrockruntime)
    type annotations stubs module [types-aiobotocore-bedrock-agent-runtime](https://pypi.org/project/types-aiobotocore-bedrock-agent-runtime/).

## GetAgentMemoryPaginator

Type annotations and code completion for `#!python session.client("bedrock-agent-runtime").get_paginator("get_agent_memory")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime/paginator/GetAgentMemory.html#AgentsforBedrockRuntime.Paginator.GetAgentMemory)

```python
# GetAgentMemoryPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_bedrock_agent_runtime.paginator import GetAgentMemoryPaginator

session = Session()

session = get_session()
async with session.client("bedrock-agent-runtime") as client:  # (1)
    paginator: GetAgentMemoryPaginator = client.get_paginator("get_agent_memory")  # (2)
    async for item in paginator.paginate(...):
        item: GetAgentMemoryResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockRuntimeClient](./client.md)
2. paginator: [GetAgentMemoryPaginator](./paginators.md#getagentmemorypaginator)
3. item: `AioPageIterator[GetAgentMemoryResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetAgentMemoryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    agentAliasId: str,
    agentId: str,
    memoryId: str,
    memoryType: MemoryTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[GetAgentMemoryResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: MemoryTypeType](./literals.md#memorytypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[GetAgentMemoryResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetAgentMemoryRequestPaginateTypeDef = {  # (1)
    "agentAliasId": ...,
    "agentId": ...,
    "memoryId": ...,
    "memoryType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetAgentMemoryRequestPaginateTypeDef](./type_defs.md#getagentmemoryrequestpaginatetypedef)
## RerankPaginator

Type annotations and code completion for `#!python session.client("bedrock-agent-runtime").get_paginator("rerank")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime/paginator/Rerank.html#AgentsforBedrockRuntime.Paginator.Rerank)

```python
# RerankPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_bedrock_agent_runtime.paginator import RerankPaginator

session = Session()

session = get_session()
async with session.client("bedrock-agent-runtime") as client:  # (1)
    paginator: RerankPaginator = client.get_paginator("rerank")  # (2)
    async for item in paginator.paginate(...):
        item: RerankResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockRuntimeClient](./client.md)
2. paginator: [RerankPaginator](./paginators.md#rerankpaginator)
3. item: `AioPageIterator[RerankResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python RerankPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    queries: Sequence[RerankQueryTypeDef],  # (1)
    rerankingConfiguration: RerankingConfigurationTypeDef,  # (2)
    sources: Sequence[RerankSourceTypeDef],  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[RerankResponseTypeDef]:  # (5)
    ...
```

1. See `Sequence[RerankQueryTypeDef]`
2. See [:material-code-braces: RerankingConfigurationTypeDef](./type_defs.md#rerankingconfigurationtypedef)
3. See `Sequence[RerankSourceTypeDef]`
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[RerankResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: RerankRequestPaginateTypeDef = {  # (1)
    "queries": ...,
    "rerankingConfiguration": ...,
    "sources": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: RerankRequestPaginateTypeDef](./type_defs.md#rerankrequestpaginatetypedef)
## RetrievePaginator

Type annotations and code completion for `#!python session.client("bedrock-agent-runtime").get_paginator("retrieve")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime/paginator/Retrieve.html#AgentsforBedrockRuntime.Paginator.Retrieve)

```python
# RetrievePaginator usage example

from aioboto3.session import Session

from types_aiobotocore_bedrock_agent_runtime.paginator import RetrievePaginator

session = Session()

session = get_session()
async with session.client("bedrock-agent-runtime") as client:  # (1)
    paginator: RetrievePaginator = client.get_paginator("retrieve")  # (2)
    async for item in paginator.paginate(...):
        item: RetrieveResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockRuntimeClient](./client.md)
2. paginator: [RetrievePaginator](./paginators.md#retrievepaginator)
3. item: `AioPageIterator[RetrieveResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python RetrievePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    knowledgeBaseId: str,
    retrievalQuery: KnowledgeBaseQueryTypeDef,  # (1)
    guardrailConfiguration: GuardrailConfigurationTypeDef = ...,  # (2)
    retrievalConfiguration: KnowledgeBaseRetrievalConfigurationPaginatorTypeDef = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[RetrieveResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: KnowledgeBaseQueryTypeDef](./type_defs.md#knowledgebasequerytypedef)
2. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef)
3. See [:material-code-braces: KnowledgeBaseRetrievalConfigurationPaginatorTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationpaginatortypedef)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[RetrieveResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: RetrieveRequestPaginateTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "retrievalQuery": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: RetrieveRequestPaginateTypeDef](./type_defs.md#retrieverequestpaginatetypedef)
