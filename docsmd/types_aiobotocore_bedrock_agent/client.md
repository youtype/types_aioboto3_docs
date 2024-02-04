# AgentsforBedrockClient

> [Index](../README.md) > [AgentsforBedrock](./README.md) > AgentsforBedrockClient

!!! note ""

    Auto-generated documentation for [AgentsforBedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
    type annotations stubs module [types-aiobotocore-bedrock-agent](https://pypi.org/project/types-aiobotocore-bedrock-agent/).

## AgentsforBedrockClient

Type annotations and code completion for `#!python session.client("bedrock-agent")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client)

```python
# AgentsforBedrockClient usage example

from aioboto3.session import Session
from types_aiobotocore_bedrock_agent.client import AgentsforBedrockClient

session = Session()
async with session.client("bedrock-agent") as client:
    client: AgentsforBedrockClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("bedrock-agent").exceptions` structure.

```python
# AgentsforBedrockClient.exceptions usage example

async with session.client("bedrock-agent") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# AgentsforBedrockClient.exceptions type checking example

from types_aiobotocore_bedrock_agent.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### associate\_agent\_knowledge\_base

Associate a Knowledge Base to an existing Amazon Bedrock Agent See also: [AWS
API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/AssociateAgentKnowledgeBase).

Type annotations and code completion for `#!python session.client("bedrock-agent").associate_agent_knowledge_base` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.associate_agent_knowledge_base)

```python
# associate_agent_knowledge_base method definition

await def associate_agent_knowledge_base(
    self,
    *,
    agentId: str,
    agentVersion: str,
    knowledgeBaseId: str,
    description: str,
    knowledgeBaseState: KnowledgeBaseStateType = ...,  # (1)
) -> AssociateAgentKnowledgeBaseResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: KnowledgeBaseStateType](./literals.md#knowledgebasestatetype) 
2. See [:material-code-braces: AssociateAgentKnowledgeBaseResponseTypeDef](./type_defs.md#associateagentknowledgebaseresponsetypedef) 


```python
# associate_agent_knowledge_base method usage example with argument unpacking

kwargs: AssociateAgentKnowledgeBaseRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentVersion": ...,
    "knowledgeBaseId": ...,
    "description": ...,
}

parent.associate_agent_knowledge_base(**kwargs)
```

1. See [:material-code-braces: AssociateAgentKnowledgeBaseRequestRequestTypeDef](./type_defs.md#associateagentknowledgebaserequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.client("bedrock-agent").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.can_paginate)

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

Type annotations and code completion for `#!python session.client("bedrock-agent").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_agent

Creates an Amazon Bedrock Agent See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/CreateAgent).

Type annotations and code completion for `#!python session.client("bedrock-agent").create_agent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_agent)

```python
# create_agent method definition

await def create_agent(
    self,
    *,
    agentName: str,
    agentResourceRoleArn: str,
    clientToken: str = ...,
    instruction: str = ...,
    foundationModel: str = ...,
    description: str = ...,
    idleSessionTTLInSeconds: int = ...,
    customerEncryptionKeyArn: str = ...,
    tags: Mapping[str, str] = ...,
    promptOverrideConfiguration: PromptOverrideConfigurationTypeDef = ...,  # (1)
) -> CreateAgentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PromptOverrideConfigurationTypeDef](./type_defs.md#promptoverrideconfigurationtypedef) 
2. See [:material-code-braces: CreateAgentResponseTypeDef](./type_defs.md#createagentresponsetypedef) 


```python
# create_agent method usage example with argument unpacking

kwargs: CreateAgentRequestRequestTypeDef = {  # (1)
    "agentName": ...,
    "agentResourceRoleArn": ...,
}

parent.create_agent(**kwargs)
```

1. See [:material-code-braces: CreateAgentRequestRequestTypeDef](./type_defs.md#createagentrequestrequesttypedef) 

### create\_agent\_action\_group

Creates an Action Group for existing Amazon Bedrock Agent See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/CreateAgentActionGroup).

Type annotations and code completion for `#!python session.client("bedrock-agent").create_agent_action_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_agent_action_group)

```python
# create_agent_action_group method definition

await def create_agent_action_group(
    self,
    *,
    agentId: str,
    agentVersion: str,
    actionGroupName: str,
    clientToken: str = ...,
    description: str = ...,
    parentActionGroupSignature: ActionGroupSignatureType = ...,  # (1)
    actionGroupExecutor: ActionGroupExecutorTypeDef = ...,  # (2)
    apiSchema: APISchemaTypeDef = ...,  # (3)
    actionGroupState: ActionGroupStateType = ...,  # (4)
) -> CreateAgentActionGroupResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: ActionGroupSignatureType](./literals.md#actiongroupsignaturetype) 
2. See [:material-code-braces: ActionGroupExecutorTypeDef](./type_defs.md#actiongroupexecutortypedef) 
3. See [:material-code-braces: APISchemaTypeDef](./type_defs.md#apischematypedef) 
4. See [:material-code-brackets: ActionGroupStateType](./literals.md#actiongroupstatetype) 
5. See [:material-code-braces: CreateAgentActionGroupResponseTypeDef](./type_defs.md#createagentactiongroupresponsetypedef) 


```python
# create_agent_action_group method usage example with argument unpacking

kwargs: CreateAgentActionGroupRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentVersion": ...,
    "actionGroupName": ...,
}

parent.create_agent_action_group(**kwargs)
```

1. See [:material-code-braces: CreateAgentActionGroupRequestRequestTypeDef](./type_defs.md#createagentactiongrouprequestrequesttypedef) 

### create\_agent\_alias

Creates an Alias for an existing Amazon Bedrock Agent See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/CreateAgentAlias).

Type annotations and code completion for `#!python session.client("bedrock-agent").create_agent_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_agent_alias)

```python
# create_agent_alias method definition

await def create_agent_alias(
    self,
    *,
    agentId: str,
    agentAliasName: str,
    clientToken: str = ...,
    description: str = ...,
    routingConfiguration: Sequence[AgentAliasRoutingConfigurationListItemTypeDef] = ...,  # (1)
    tags: Mapping[str, str] = ...,
) -> CreateAgentAliasResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AgentAliasRoutingConfigurationListItemTypeDef](./type_defs.md#agentaliasroutingconfigurationlistitemtypedef) 
2. See [:material-code-braces: CreateAgentAliasResponseTypeDef](./type_defs.md#createagentaliasresponsetypedef) 


```python
# create_agent_alias method usage example with argument unpacking

kwargs: CreateAgentAliasRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentAliasName": ...,
}

parent.create_agent_alias(**kwargs)
```

1. See [:material-code-braces: CreateAgentAliasRequestRequestTypeDef](./type_defs.md#createagentaliasrequestrequesttypedef) 

### create\_data\_source

Create a new data source See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/CreateDataSource).

Type annotations and code completion for `#!python session.client("bedrock-agent").create_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_data_source)

```python
# create_data_source method definition

await def create_data_source(
    self,
    *,
    knowledgeBaseId: str,
    name: str,
    dataSourceConfiguration: DataSourceConfigurationTypeDef,  # (1)
    clientToken: str = ...,
    description: str = ...,
    serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,  # (2)
    vectorIngestionConfiguration: VectorIngestionConfigurationTypeDef = ...,  # (3)
) -> CreateDataSourceResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef) 
2. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
3. See [:material-code-braces: VectorIngestionConfigurationTypeDef](./type_defs.md#vectoringestionconfigurationtypedef) 
4. See [:material-code-braces: CreateDataSourceResponseTypeDef](./type_defs.md#createdatasourceresponsetypedef) 


```python
# create_data_source method usage example with argument unpacking

kwargs: CreateDataSourceRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "name": ...,
    "dataSourceConfiguration": ...,
}

parent.create_data_source(**kwargs)
```

1. See [:material-code-braces: CreateDataSourceRequestRequestTypeDef](./type_defs.md#createdatasourcerequestrequesttypedef) 

### create\_knowledge\_base

Create a new knowledge base See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/CreateKnowledgeBase).

Type annotations and code completion for `#!python session.client("bedrock-agent").create_knowledge_base` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_knowledge_base)

```python
# create_knowledge_base method definition

await def create_knowledge_base(
    self,
    *,
    name: str,
    roleArn: str,
    knowledgeBaseConfiguration: KnowledgeBaseConfigurationTypeDef,  # (1)
    storageConfiguration: StorageConfigurationTypeDef,  # (2)
    clientToken: str = ...,
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateKnowledgeBaseResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: KnowledgeBaseConfigurationTypeDef](./type_defs.md#knowledgebaseconfigurationtypedef) 
2. See [:material-code-braces: StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef) 
3. See [:material-code-braces: CreateKnowledgeBaseResponseTypeDef](./type_defs.md#createknowledgebaseresponsetypedef) 


```python
# create_knowledge_base method usage example with argument unpacking

kwargs: CreateKnowledgeBaseRequestRequestTypeDef = {  # (1)
    "name": ...,
    "roleArn": ...,
    "knowledgeBaseConfiguration": ...,
    "storageConfiguration": ...,
}

parent.create_knowledge_base(**kwargs)
```

1. See [:material-code-braces: CreateKnowledgeBaseRequestRequestTypeDef](./type_defs.md#createknowledgebaserequestrequesttypedef) 

### delete\_agent

Deletes an Agent for existing Amazon Bedrock Agent See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/DeleteAgent).

Type annotations and code completion for `#!python session.client("bedrock-agent").delete_agent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.delete_agent)

```python
# delete_agent method definition

await def delete_agent(
    self,
    *,
    agentId: str,
    skipResourceInUseCheck: bool = ...,
) -> DeleteAgentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteAgentResponseTypeDef](./type_defs.md#deleteagentresponsetypedef) 


```python
# delete_agent method usage example with argument unpacking

kwargs: DeleteAgentRequestRequestTypeDef = {  # (1)
    "agentId": ...,
}

parent.delete_agent(**kwargs)
```

1. See [:material-code-braces: DeleteAgentRequestRequestTypeDef](./type_defs.md#deleteagentrequestrequesttypedef) 

### delete\_agent\_action\_group

Deletes an Action Group for existing Amazon Bedrock Agent.

Type annotations and code completion for `#!python session.client("bedrock-agent").delete_agent_action_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.delete_agent_action_group)

```python
# delete_agent_action_group method definition

await def delete_agent_action_group(
    self,
    *,
    agentId: str,
    agentVersion: str,
    actionGroupId: str,
    skipResourceInUseCheck: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_agent_action_group method usage example with argument unpacking

kwargs: DeleteAgentActionGroupRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentVersion": ...,
    "actionGroupId": ...,
}

parent.delete_agent_action_group(**kwargs)
```

1. See [:material-code-braces: DeleteAgentActionGroupRequestRequestTypeDef](./type_defs.md#deleteagentactiongrouprequestrequesttypedef) 

### delete\_agent\_alias

Deletes an Alias for a Amazon Bedrock Agent See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/DeleteAgentAlias).

Type annotations and code completion for `#!python session.client("bedrock-agent").delete_agent_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.delete_agent_alias)

```python
# delete_agent_alias method definition

await def delete_agent_alias(
    self,
    *,
    agentId: str,
    agentAliasId: str,
) -> DeleteAgentAliasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteAgentAliasResponseTypeDef](./type_defs.md#deleteagentaliasresponsetypedef) 


```python
# delete_agent_alias method usage example with argument unpacking

kwargs: DeleteAgentAliasRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentAliasId": ...,
}

parent.delete_agent_alias(**kwargs)
```

1. See [:material-code-braces: DeleteAgentAliasRequestRequestTypeDef](./type_defs.md#deleteagentaliasrequestrequesttypedef) 

### delete\_agent\_version

Deletes an Agent version for existing Amazon Bedrock Agent See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/DeleteAgentVersion).

Type annotations and code completion for `#!python session.client("bedrock-agent").delete_agent_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.delete_agent_version)

```python
# delete_agent_version method definition

await def delete_agent_version(
    self,
    *,
    agentId: str,
    agentVersion: str,
    skipResourceInUseCheck: bool = ...,
) -> DeleteAgentVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteAgentVersionResponseTypeDef](./type_defs.md#deleteagentversionresponsetypedef) 


```python
# delete_agent_version method usage example with argument unpacking

kwargs: DeleteAgentVersionRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentVersion": ...,
}

parent.delete_agent_version(**kwargs)
```

1. See [:material-code-braces: DeleteAgentVersionRequestRequestTypeDef](./type_defs.md#deleteagentversionrequestrequesttypedef) 

### delete\_data\_source

Delete an existing data source See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/DeleteDataSource).

Type annotations and code completion for `#!python session.client("bedrock-agent").delete_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.delete_data_source)

```python
# delete_data_source method definition

await def delete_data_source(
    self,
    *,
    knowledgeBaseId: str,
    dataSourceId: str,
) -> DeleteDataSourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDataSourceResponseTypeDef](./type_defs.md#deletedatasourceresponsetypedef) 


```python
# delete_data_source method usage example with argument unpacking

kwargs: DeleteDataSourceRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "dataSourceId": ...,
}

parent.delete_data_source(**kwargs)
```

1. See [:material-code-braces: DeleteDataSourceRequestRequestTypeDef](./type_defs.md#deletedatasourcerequestrequesttypedef) 

### delete\_knowledge\_base

Delete an existing knowledge base See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/DeleteKnowledgeBase).

Type annotations and code completion for `#!python session.client("bedrock-agent").delete_knowledge_base` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.delete_knowledge_base)

```python
# delete_knowledge_base method definition

await def delete_knowledge_base(
    self,
    *,
    knowledgeBaseId: str,
) -> DeleteKnowledgeBaseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteKnowledgeBaseResponseTypeDef](./type_defs.md#deleteknowledgebaseresponsetypedef) 


```python
# delete_knowledge_base method usage example with argument unpacking

kwargs: DeleteKnowledgeBaseRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
}

parent.delete_knowledge_base(**kwargs)
```

1. See [:material-code-braces: DeleteKnowledgeBaseRequestRequestTypeDef](./type_defs.md#deleteknowledgebaserequestrequesttypedef) 

### disassociate\_agent\_knowledge\_base

Disassociate an existing Knowledge Base from an Amazon Bedrock Agent See also:
[AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/DisassociateAgentKnowledgeBase).

Type annotations and code completion for `#!python session.client("bedrock-agent").disassociate_agent_knowledge_base` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.disassociate_agent_knowledge_base)

```python
# disassociate_agent_knowledge_base method definition

await def disassociate_agent_knowledge_base(
    self,
    *,
    agentId: str,
    agentVersion: str,
    knowledgeBaseId: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_agent_knowledge_base method usage example with argument unpacking

kwargs: DisassociateAgentKnowledgeBaseRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentVersion": ...,
    "knowledgeBaseId": ...,
}

parent.disassociate_agent_knowledge_base(**kwargs)
```

1. See [:material-code-braces: DisassociateAgentKnowledgeBaseRequestRequestTypeDef](./type_defs.md#disassociateagentknowledgebaserequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.client("bedrock-agent").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.generate_presigned_url)

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


### get\_agent

Gets an Agent for existing Amazon Bedrock Agent See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/GetAgent).

Type annotations and code completion for `#!python session.client("bedrock-agent").get_agent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.get_agent)

```python
# get_agent method definition

await def get_agent(
    self,
    *,
    agentId: str,
) -> GetAgentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAgentResponseTypeDef](./type_defs.md#getagentresponsetypedef) 


```python
# get_agent method usage example with argument unpacking

kwargs: GetAgentRequestRequestTypeDef = {  # (1)
    "agentId": ...,
}

parent.get_agent(**kwargs)
```

1. See [:material-code-braces: GetAgentRequestRequestTypeDef](./type_defs.md#getagentrequestrequesttypedef) 

### get\_agent\_action\_group

Gets an Action Group for existing Amazon Bedrock Agent Version See also: [AWS
API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/GetAgentActionGroup).

Type annotations and code completion for `#!python session.client("bedrock-agent").get_agent_action_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.get_agent_action_group)

```python
# get_agent_action_group method definition

await def get_agent_action_group(
    self,
    *,
    agentId: str,
    agentVersion: str,
    actionGroupId: str,
) -> GetAgentActionGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAgentActionGroupResponseTypeDef](./type_defs.md#getagentactiongroupresponsetypedef) 


```python
# get_agent_action_group method usage example with argument unpacking

kwargs: GetAgentActionGroupRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentVersion": ...,
    "actionGroupId": ...,
}

parent.get_agent_action_group(**kwargs)
```

1. See [:material-code-braces: GetAgentActionGroupRequestRequestTypeDef](./type_defs.md#getagentactiongrouprequestrequesttypedef) 

### get\_agent\_alias

Describes an Alias for a Amazon Bedrock Agent See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/GetAgentAlias).

Type annotations and code completion for `#!python session.client("bedrock-agent").get_agent_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.get_agent_alias)

```python
# get_agent_alias method definition

await def get_agent_alias(
    self,
    *,
    agentId: str,
    agentAliasId: str,
) -> GetAgentAliasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAgentAliasResponseTypeDef](./type_defs.md#getagentaliasresponsetypedef) 


```python
# get_agent_alias method usage example with argument unpacking

kwargs: GetAgentAliasRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentAliasId": ...,
}

parent.get_agent_alias(**kwargs)
```

1. See [:material-code-braces: GetAgentAliasRequestRequestTypeDef](./type_defs.md#getagentaliasrequestrequesttypedef) 

### get\_agent\_knowledge\_base

Gets a knowledge base associated to an existing Amazon Bedrock Agent Version
See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/GetAgentKnowledgeBase).

Type annotations and code completion for `#!python session.client("bedrock-agent").get_agent_knowledge_base` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.get_agent_knowledge_base)

```python
# get_agent_knowledge_base method definition

await def get_agent_knowledge_base(
    self,
    *,
    agentId: str,
    agentVersion: str,
    knowledgeBaseId: str,
) -> GetAgentKnowledgeBaseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAgentKnowledgeBaseResponseTypeDef](./type_defs.md#getagentknowledgebaseresponsetypedef) 


```python
# get_agent_knowledge_base method usage example with argument unpacking

kwargs: GetAgentKnowledgeBaseRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentVersion": ...,
    "knowledgeBaseId": ...,
}

parent.get_agent_knowledge_base(**kwargs)
```

1. See [:material-code-braces: GetAgentKnowledgeBaseRequestRequestTypeDef](./type_defs.md#getagentknowledgebaserequestrequesttypedef) 

### get\_agent\_version

Gets an Agent version for existing Amazon Bedrock Agent See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/GetAgentVersion).

Type annotations and code completion for `#!python session.client("bedrock-agent").get_agent_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.get_agent_version)

```python
# get_agent_version method definition

await def get_agent_version(
    self,
    *,
    agentId: str,
    agentVersion: str,
) -> GetAgentVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAgentVersionResponseTypeDef](./type_defs.md#getagentversionresponsetypedef) 


```python
# get_agent_version method usage example with argument unpacking

kwargs: GetAgentVersionRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentVersion": ...,
}

parent.get_agent_version(**kwargs)
```

1. See [:material-code-braces: GetAgentVersionRequestRequestTypeDef](./type_defs.md#getagentversionrequestrequesttypedef) 

### get\_data\_source

Get an existing data source See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/GetDataSource).

Type annotations and code completion for `#!python session.client("bedrock-agent").get_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.get_data_source)

```python
# get_data_source method definition

await def get_data_source(
    self,
    *,
    knowledgeBaseId: str,
    dataSourceId: str,
) -> GetDataSourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataSourceResponseTypeDef](./type_defs.md#getdatasourceresponsetypedef) 


```python
# get_data_source method usage example with argument unpacking

kwargs: GetDataSourceRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "dataSourceId": ...,
}

parent.get_data_source(**kwargs)
```

1. See [:material-code-braces: GetDataSourceRequestRequestTypeDef](./type_defs.md#getdatasourcerequestrequesttypedef) 

### get\_ingestion\_job

Get an ingestion job See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/GetIngestionJob).

Type annotations and code completion for `#!python session.client("bedrock-agent").get_ingestion_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.get_ingestion_job)

```python
# get_ingestion_job method definition

await def get_ingestion_job(
    self,
    *,
    knowledgeBaseId: str,
    dataSourceId: str,
    ingestionJobId: str,
) -> GetIngestionJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIngestionJobResponseTypeDef](./type_defs.md#getingestionjobresponsetypedef) 


```python
# get_ingestion_job method usage example with argument unpacking

kwargs: GetIngestionJobRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "dataSourceId": ...,
    "ingestionJobId": ...,
}

parent.get_ingestion_job(**kwargs)
```

1. See [:material-code-braces: GetIngestionJobRequestRequestTypeDef](./type_defs.md#getingestionjobrequestrequesttypedef) 

### get\_knowledge\_base

Get an existing knowledge base See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/GetKnowledgeBase).

Type annotations and code completion for `#!python session.client("bedrock-agent").get_knowledge_base` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.get_knowledge_base)

```python
# get_knowledge_base method definition

await def get_knowledge_base(
    self,
    *,
    knowledgeBaseId: str,
) -> GetKnowledgeBaseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetKnowledgeBaseResponseTypeDef](./type_defs.md#getknowledgebaseresponsetypedef) 


```python
# get_knowledge_base method usage example with argument unpacking

kwargs: GetKnowledgeBaseRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
}

parent.get_knowledge_base(**kwargs)
```

1. See [:material-code-braces: GetKnowledgeBaseRequestRequestTypeDef](./type_defs.md#getknowledgebaserequestrequesttypedef) 

### list\_agent\_action\_groups

Lists an Action Group for existing Amazon Bedrock Agent Version See also: [AWS
API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/ListAgentActionGroups).

Type annotations and code completion for `#!python session.client("bedrock-agent").list_agent_action_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.list_agent_action_groups)

```python
# list_agent_action_groups method definition

await def list_agent_action_groups(
    self,
    *,
    agentId: str,
    agentVersion: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAgentActionGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAgentActionGroupsResponseTypeDef](./type_defs.md#listagentactiongroupsresponsetypedef) 


```python
# list_agent_action_groups method usage example with argument unpacking

kwargs: ListAgentActionGroupsRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentVersion": ...,
}

parent.list_agent_action_groups(**kwargs)
```

1. See [:material-code-braces: ListAgentActionGroupsRequestRequestTypeDef](./type_defs.md#listagentactiongroupsrequestrequesttypedef) 

### list\_agent\_aliases

Lists all the Aliases for an Amazon Bedrock Agent See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/ListAgentAliases).

Type annotations and code completion for `#!python session.client("bedrock-agent").list_agent_aliases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.list_agent_aliases)

```python
# list_agent_aliases method definition

await def list_agent_aliases(
    self,
    *,
    agentId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAgentAliasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAgentAliasesResponseTypeDef](./type_defs.md#listagentaliasesresponsetypedef) 


```python
# list_agent_aliases method usage example with argument unpacking

kwargs: ListAgentAliasesRequestRequestTypeDef = {  # (1)
    "agentId": ...,
}

parent.list_agent_aliases(**kwargs)
```

1. See [:material-code-braces: ListAgentAliasesRequestRequestTypeDef](./type_defs.md#listagentaliasesrequestrequesttypedef) 

### list\_agent\_knowledge\_bases

List of Knowledge Bases associated to an existing Amazon Bedrock Agent Version
See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/ListAgentKnowledgeBases).

Type annotations and code completion for `#!python session.client("bedrock-agent").list_agent_knowledge_bases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.list_agent_knowledge_bases)

```python
# list_agent_knowledge_bases method definition

await def list_agent_knowledge_bases(
    self,
    *,
    agentId: str,
    agentVersion: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAgentKnowledgeBasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAgentKnowledgeBasesResponseTypeDef](./type_defs.md#listagentknowledgebasesresponsetypedef) 


```python
# list_agent_knowledge_bases method usage example with argument unpacking

kwargs: ListAgentKnowledgeBasesRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentVersion": ...,
}

parent.list_agent_knowledge_bases(**kwargs)
```

1. See [:material-code-braces: ListAgentKnowledgeBasesRequestRequestTypeDef](./type_defs.md#listagentknowledgebasesrequestrequesttypedef) 

### list\_agent\_versions

Lists Agent Versions See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/ListAgentVersions).

Type annotations and code completion for `#!python session.client("bedrock-agent").list_agent_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.list_agent_versions)

```python
# list_agent_versions method definition

await def list_agent_versions(
    self,
    *,
    agentId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAgentVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAgentVersionsResponseTypeDef](./type_defs.md#listagentversionsresponsetypedef) 


```python
# list_agent_versions method usage example with argument unpacking

kwargs: ListAgentVersionsRequestRequestTypeDef = {  # (1)
    "agentId": ...,
}

parent.list_agent_versions(**kwargs)
```

1. See [:material-code-braces: ListAgentVersionsRequestRequestTypeDef](./type_defs.md#listagentversionsrequestrequesttypedef) 

### list\_agents

Lists Agents See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/ListAgents).

Type annotations and code completion for `#!python session.client("bedrock-agent").list_agents` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.list_agents)

```python
# list_agents method definition

await def list_agents(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAgentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAgentsResponseTypeDef](./type_defs.md#listagentsresponsetypedef) 


```python
# list_agents method usage example with argument unpacking

kwargs: ListAgentsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_agents(**kwargs)
```

1. See [:material-code-braces: ListAgentsRequestRequestTypeDef](./type_defs.md#listagentsrequestrequesttypedef) 

### list\_data\_sources

List data sources See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/ListDataSources).

Type annotations and code completion for `#!python session.client("bedrock-agent").list_data_sources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.list_data_sources)

```python
# list_data_sources method definition

await def list_data_sources(
    self,
    *,
    knowledgeBaseId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListDataSourcesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDataSourcesResponseTypeDef](./type_defs.md#listdatasourcesresponsetypedef) 


```python
# list_data_sources method usage example with argument unpacking

kwargs: ListDataSourcesRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
}

parent.list_data_sources(**kwargs)
```

1. See [:material-code-braces: ListDataSourcesRequestRequestTypeDef](./type_defs.md#listdatasourcesrequestrequesttypedef) 

### list\_ingestion\_jobs

List ingestion jobs See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/ListIngestionJobs).

Type annotations and code completion for `#!python session.client("bedrock-agent").list_ingestion_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.list_ingestion_jobs)

```python
# list_ingestion_jobs method definition

await def list_ingestion_jobs(
    self,
    *,
    knowledgeBaseId: str,
    dataSourceId: str,
    filters: Sequence[IngestionJobFilterTypeDef] = ...,  # (1)
    sortBy: IngestionJobSortByTypeDef = ...,  # (2)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListIngestionJobsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: IngestionJobFilterTypeDef](./type_defs.md#ingestionjobfiltertypedef) 
2. See [:material-code-braces: IngestionJobSortByTypeDef](./type_defs.md#ingestionjobsortbytypedef) 
3. See [:material-code-braces: ListIngestionJobsResponseTypeDef](./type_defs.md#listingestionjobsresponsetypedef) 


```python
# list_ingestion_jobs method usage example with argument unpacking

kwargs: ListIngestionJobsRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "dataSourceId": ...,
}

parent.list_ingestion_jobs(**kwargs)
```

1. See [:material-code-braces: ListIngestionJobsRequestRequestTypeDef](./type_defs.md#listingestionjobsrequestrequesttypedef) 

### list\_knowledge\_bases

List Knowledge Bases See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/ListKnowledgeBases).

Type annotations and code completion for `#!python session.client("bedrock-agent").list_knowledge_bases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.list_knowledge_bases)

```python
# list_knowledge_bases method definition

await def list_knowledge_bases(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListKnowledgeBasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListKnowledgeBasesResponseTypeDef](./type_defs.md#listknowledgebasesresponsetypedef) 


```python
# list_knowledge_bases method usage example with argument unpacking

kwargs: ListKnowledgeBasesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_knowledge_bases(**kwargs)
```

1. See [:material-code-braces: ListKnowledgeBasesRequestRequestTypeDef](./type_defs.md#listknowledgebasesrequestrequesttypedef) 

### list\_tags\_for\_resource

List tags for a resource See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/ListTagsForResource).

Type annotations and code completion for `#!python session.client("bedrock-agent").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### prepare\_agent

Prepares an existing Amazon Bedrock Agent to receive runtime requests See also:
[AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/PrepareAgent).

Type annotations and code completion for `#!python session.client("bedrock-agent").prepare_agent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.prepare_agent)

```python
# prepare_agent method definition

await def prepare_agent(
    self,
    *,
    agentId: str,
) -> PrepareAgentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PrepareAgentResponseTypeDef](./type_defs.md#prepareagentresponsetypedef) 


```python
# prepare_agent method usage example with argument unpacking

kwargs: PrepareAgentRequestRequestTypeDef = {  # (1)
    "agentId": ...,
}

parent.prepare_agent(**kwargs)
```

1. See [:material-code-braces: PrepareAgentRequestRequestTypeDef](./type_defs.md#prepareagentrequestrequesttypedef) 

### start\_ingestion\_job

Start a new ingestion job See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/StartIngestionJob).

Type annotations and code completion for `#!python session.client("bedrock-agent").start_ingestion_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.start_ingestion_job)

```python
# start_ingestion_job method definition

await def start_ingestion_job(
    self,
    *,
    knowledgeBaseId: str,
    dataSourceId: str,
    clientToken: str = ...,
    description: str = ...,
) -> StartIngestionJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartIngestionJobResponseTypeDef](./type_defs.md#startingestionjobresponsetypedef) 


```python
# start_ingestion_job method usage example with argument unpacking

kwargs: StartIngestionJobRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "dataSourceId": ...,
}

parent.start_ingestion_job(**kwargs)
```

1. See [:material-code-braces: StartIngestionJobRequestRequestTypeDef](./type_defs.md#startingestionjobrequestrequesttypedef) 

### tag\_resource

Tag a resource See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/TagResource).

Type annotations and code completion for `#!python session.client("bedrock-agent").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Untag a resource See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/UntagResource).

Type annotations and code completion for `#!python session.client("bedrock-agent").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_agent

Updates an existing Amazon Bedrock Agent See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/UpdateAgent).

Type annotations and code completion for `#!python session.client("bedrock-agent").update_agent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_agent)

```python
# update_agent method definition

await def update_agent(
    self,
    *,
    agentId: str,
    agentName: str,
    agentResourceRoleArn: str,
    instruction: str = ...,
    foundationModel: str = ...,
    description: str = ...,
    idleSessionTTLInSeconds: int = ...,
    customerEncryptionKeyArn: str = ...,
    promptOverrideConfiguration: PromptOverrideConfigurationTypeDef = ...,  # (1)
) -> UpdateAgentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PromptOverrideConfigurationTypeDef](./type_defs.md#promptoverrideconfigurationtypedef) 
2. See [:material-code-braces: UpdateAgentResponseTypeDef](./type_defs.md#updateagentresponsetypedef) 


```python
# update_agent method usage example with argument unpacking

kwargs: UpdateAgentRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentName": ...,
    "agentResourceRoleArn": ...,
}

parent.update_agent(**kwargs)
```

1. See [:material-code-braces: UpdateAgentRequestRequestTypeDef](./type_defs.md#updateagentrequestrequesttypedef) 

### update\_agent\_action\_group

Updates an existing Action Group for Amazon Bedrock Agent See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/UpdateAgentActionGroup).

Type annotations and code completion for `#!python session.client("bedrock-agent").update_agent_action_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_agent_action_group)

```python
# update_agent_action_group method definition

await def update_agent_action_group(
    self,
    *,
    agentId: str,
    agentVersion: str,
    actionGroupId: str,
    actionGroupName: str,
    description: str = ...,
    parentActionGroupSignature: ActionGroupSignatureType = ...,  # (1)
    actionGroupExecutor: ActionGroupExecutorTypeDef = ...,  # (2)
    actionGroupState: ActionGroupStateType = ...,  # (3)
    apiSchema: APISchemaTypeDef = ...,  # (4)
) -> UpdateAgentActionGroupResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: ActionGroupSignatureType](./literals.md#actiongroupsignaturetype) 
2. See [:material-code-braces: ActionGroupExecutorTypeDef](./type_defs.md#actiongroupexecutortypedef) 
3. See [:material-code-brackets: ActionGroupStateType](./literals.md#actiongroupstatetype) 
4. See [:material-code-braces: APISchemaTypeDef](./type_defs.md#apischematypedef) 
5. See [:material-code-braces: UpdateAgentActionGroupResponseTypeDef](./type_defs.md#updateagentactiongroupresponsetypedef) 


```python
# update_agent_action_group method usage example with argument unpacking

kwargs: UpdateAgentActionGroupRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentVersion": ...,
    "actionGroupId": ...,
    "actionGroupName": ...,
}

parent.update_agent_action_group(**kwargs)
```

1. See [:material-code-braces: UpdateAgentActionGroupRequestRequestTypeDef](./type_defs.md#updateagentactiongrouprequestrequesttypedef) 

### update\_agent\_alias

Updates an existing Alias for an Amazon Bedrock Agent See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/UpdateAgentAlias).

Type annotations and code completion for `#!python session.client("bedrock-agent").update_agent_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_agent_alias)

```python
# update_agent_alias method definition

await def update_agent_alias(
    self,
    *,
    agentId: str,
    agentAliasId: str,
    agentAliasName: str,
    description: str = ...,
    routingConfiguration: Sequence[AgentAliasRoutingConfigurationListItemTypeDef] = ...,  # (1)
) -> UpdateAgentAliasResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AgentAliasRoutingConfigurationListItemTypeDef](./type_defs.md#agentaliasroutingconfigurationlistitemtypedef) 
2. See [:material-code-braces: UpdateAgentAliasResponseTypeDef](./type_defs.md#updateagentaliasresponsetypedef) 


```python
# update_agent_alias method usage example with argument unpacking

kwargs: UpdateAgentAliasRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentAliasId": ...,
    "agentAliasName": ...,
}

parent.update_agent_alias(**kwargs)
```

1. See [:material-code-braces: UpdateAgentAliasRequestRequestTypeDef](./type_defs.md#updateagentaliasrequestrequesttypedef) 

### update\_agent\_knowledge\_base

Updates an existing Knowledge Base associated to an Amazon Bedrock Agent See
also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/UpdateAgentKnowledgeBase).

Type annotations and code completion for `#!python session.client("bedrock-agent").update_agent_knowledge_base` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_agent_knowledge_base)

```python
# update_agent_knowledge_base method definition

await def update_agent_knowledge_base(
    self,
    *,
    agentId: str,
    agentVersion: str,
    knowledgeBaseId: str,
    description: str = ...,
    knowledgeBaseState: KnowledgeBaseStateType = ...,  # (1)
) -> UpdateAgentKnowledgeBaseResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: KnowledgeBaseStateType](./literals.md#knowledgebasestatetype) 
2. See [:material-code-braces: UpdateAgentKnowledgeBaseResponseTypeDef](./type_defs.md#updateagentknowledgebaseresponsetypedef) 


```python
# update_agent_knowledge_base method usage example with argument unpacking

kwargs: UpdateAgentKnowledgeBaseRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentVersion": ...,
    "knowledgeBaseId": ...,
}

parent.update_agent_knowledge_base(**kwargs)
```

1. See [:material-code-braces: UpdateAgentKnowledgeBaseRequestRequestTypeDef](./type_defs.md#updateagentknowledgebaserequestrequesttypedef) 

### update\_data\_source

Update an existing data source See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/UpdateDataSource).

Type annotations and code completion for `#!python session.client("bedrock-agent").update_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_data_source)

```python
# update_data_source method definition

await def update_data_source(
    self,
    *,
    knowledgeBaseId: str,
    dataSourceId: str,
    name: str,
    dataSourceConfiguration: DataSourceConfigurationTypeDef,  # (1)
    description: str = ...,
    serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,  # (2)
    vectorIngestionConfiguration: VectorIngestionConfigurationTypeDef = ...,  # (3)
) -> UpdateDataSourceResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef) 
2. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
3. See [:material-code-braces: VectorIngestionConfigurationTypeDef](./type_defs.md#vectoringestionconfigurationtypedef) 
4. See [:material-code-braces: UpdateDataSourceResponseTypeDef](./type_defs.md#updatedatasourceresponsetypedef) 


```python
# update_data_source method usage example with argument unpacking

kwargs: UpdateDataSourceRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "dataSourceId": ...,
    "name": ...,
    "dataSourceConfiguration": ...,
}

parent.update_data_source(**kwargs)
```

1. See [:material-code-braces: UpdateDataSourceRequestRequestTypeDef](./type_defs.md#updatedatasourcerequestrequesttypedef) 

### update\_knowledge\_base

Update an existing knowledge base See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/bedrock-agent-2023-06-05/UpdateKnowledgeBase).

Type annotations and code completion for `#!python session.client("bedrock-agent").update_knowledge_base` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_knowledge_base)

```python
# update_knowledge_base method definition

await def update_knowledge_base(
    self,
    *,
    knowledgeBaseId: str,
    name: str,
    roleArn: str,
    knowledgeBaseConfiguration: KnowledgeBaseConfigurationTypeDef,  # (1)
    storageConfiguration: StorageConfigurationTypeDef,  # (2)
    description: str = ...,
) -> UpdateKnowledgeBaseResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: KnowledgeBaseConfigurationTypeDef](./type_defs.md#knowledgebaseconfigurationtypedef) 
2. See [:material-code-braces: StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef) 
3. See [:material-code-braces: UpdateKnowledgeBaseResponseTypeDef](./type_defs.md#updateknowledgebaseresponsetypedef) 


```python
# update_knowledge_base method usage example with argument unpacking

kwargs: UpdateKnowledgeBaseRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "name": ...,
    "roleArn": ...,
    "knowledgeBaseConfiguration": ...,
    "storageConfiguration": ...,
}

parent.update_knowledge_base(**kwargs)
```

1. See [:material-code-braces: UpdateKnowledgeBaseRequestRequestTypeDef](./type_defs.md#updateknowledgebaserequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("bedrock-agent").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> AgentsforBedrockClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("bedrock-agent").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.__aexit__)

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




### get_paginator

Type annotations and code completion for `#!python session.client("bedrock-agent").get_paginator` method with overloads.

- `client.get_paginator("list_agent_action_groups")` -> [ListAgentActionGroupsPaginator](./paginators.md#listagentactiongroupspaginator)
- `client.get_paginator("list_agent_aliases")` -> [ListAgentAliasesPaginator](./paginators.md#listagentaliasespaginator)
- `client.get_paginator("list_agent_knowledge_bases")` -> [ListAgentKnowledgeBasesPaginator](./paginators.md#listagentknowledgebasespaginator)
- `client.get_paginator("list_agent_versions")` -> [ListAgentVersionsPaginator](./paginators.md#listagentversionspaginator)
- `client.get_paginator("list_agents")` -> [ListAgentsPaginator](./paginators.md#listagentspaginator)
- `client.get_paginator("list_data_sources")` -> [ListDataSourcesPaginator](./paginators.md#listdatasourcespaginator)
- `client.get_paginator("list_ingestion_jobs")` -> [ListIngestionJobsPaginator](./paginators.md#listingestionjobspaginator)
- `client.get_paginator("list_knowledge_bases")` -> [ListKnowledgeBasesPaginator](./paginators.md#listknowledgebasespaginator)



