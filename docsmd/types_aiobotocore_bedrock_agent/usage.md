# Examples

> [Index](../README.md) > [AgentsforBedrock](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AgentsforBedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#agentsforbedrock)
    type annotations stubs module [types-aiobotocore-bedrock-agent](https://pypi.org/project/types-aiobotocore-bedrock-agent/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[bedrock-agent]` package installed.

Write your `AgentsforBedrock` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# AgentsforBedrockClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("bedrock-agent") as client:  # (1)
    result = await client.associate_agent_collaborator()  # (2)
```

1. client: [AgentsforBedrockClient](./client.md)
2. result: [:material-code-braces: AssociateAgentCollaboratorResponseTypeDef](./type_defs.md#associateagentcollaboratorresponsetypedef)



#### Paginator usage example

```python
# ListAgentActionGroupsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("bedrock-agent") as client:  # (1)
    paginator = client.get_paginator("list_agent_action_groups")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AgentsforBedrockClient](./client.md)
2. paginator: [ListAgentActionGroupsPaginator](./paginators.md#listagentactiongroupspaginator)
3. item: [:material-code-braces: ListAgentActionGroupsResponseTypeDef](./type_defs.md#listagentactiongroupsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[bedrock-agent]`
or a standalone `types_aiobotocore_bedrock_agent` package, you have to explicitly specify
`client: AgentsforBedrockClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# AgentsforBedrockClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_bedrock_agent.client import AgentsforBedrockClient
from types_aiobotocore_bedrock_agent.type_defs import AssociateAgentCollaboratorResponseTypeDef
from types_aiobotocore_bedrock_agent.type_defs import AssociateAgentCollaboratorRequestTypeDef


session = Session()

client: AgentsforBedrockClient
async with session.client("bedrock-agent") as client:  # (1)
    kwargs: AssociateAgentCollaboratorRequestTypeDef = {...}  # (2)
    result: AssociateAgentCollaboratorResponseTypeDef = await client.associate_agent_collaborator(**kwargs)  # (3)
```

1. client: [AgentsforBedrockClient](./client.md)
2. kwargs: [:material-code-braces: AssociateAgentCollaboratorRequestTypeDef](./type_defs.md#associateagentcollaboratorrequesttypedef)
3. result: [:material-code-braces: AssociateAgentCollaboratorResponseTypeDef](./type_defs.md#associateagentcollaboratorresponsetypedef)



#### Paginator usage example

```python
# ListAgentActionGroupsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_bedrock_agent.client import AgentsforBedrockClient
from types_aiobotocore_bedrock_agent.paginator import ListAgentActionGroupsPaginator
from types_aiobotocore_bedrock_agent.type_defs import ListAgentActionGroupsResponseTypeDef


session = Session()

client: AgentsforBedrockClient
async with session.client("bedrock-agent") as client:  # (1)
    paginator: ListAgentActionGroupsPaginator = client.get_paginator("list_agent_action_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListAgentActionGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockClient](./client.md)
2. paginator: [ListAgentActionGroupsPaginator](./paginators.md#listagentactiongroupspaginator)
3. item: [:material-code-braces: ListAgentActionGroupsResponseTypeDef](./type_defs.md#listagentactiongroupsresponsetypedef)




