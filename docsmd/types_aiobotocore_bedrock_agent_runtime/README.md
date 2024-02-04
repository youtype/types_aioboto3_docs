# AgentsforBedrockRuntime module

> [Index](../README.md) > AgentsforBedrockRuntime


!!! note ""

    Auto-generated documentation for [AgentsforBedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime)
    type annotations stubs module [types-aiobotocore-bedrock-agent-runtime](https://pypi.org/project/types-aiobotocore-bedrock-agent-runtime/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `AgentsforBedrockRuntime` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[bedrock-agent-runtime]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[bedrock-agent-runtime]'


# standalone installation
python -m pip install types-aiobotocore-bedrock-agent-runtime
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-bedrock-agent-runtime
```

## Usage

Code samples can be found in [Examples](./usage.md).

## AgentsforBedrockRuntimeClient

Type annotations and code completion for  `#!python session.client("bedrock-agent-runtime")` as [AgentsforBedrockRuntimeClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime.Client)

```python
# AgentsforBedrockRuntimeClient usage example

from aioboto3.session import Session

from types_aiobotocore_bedrock_agent_runtime.client import AgentsforBedrockRuntimeClient


session = Session()
async with session.client("bedrock-agent-runtime") as client:
    client: AgentsforBedrockRuntimeClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("bedrock-agent-runtime").get_paginator("...")`.

```python
# RetrievePaginator usage example

from types_aiobotocore_bedrock_agent_runtime.paginator import RetrievePaginator

def get_retrieve_paginator() -> RetrievePaginator:
    return client.get_paginator("retrieve"))
```

- [RetrievePaginator](./paginators.md#retrievepaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# CreationModeType usage example

from types_aiobotocore_bedrock_agent_runtime.literals import CreationModeType

def get_value() -> CreationModeType:
    return "DEFAULT"
```

- [CreationModeType](./literals.md#creationmodetype)
- [InvocationTypeType](./literals.md#invocationtypetype)
- [PromptTypeType](./literals.md#prompttypetype)
- [RetrievalResultLocationTypeType](./literals.md#retrievalresultlocationtypetype)
- [RetrieveAndGenerateTypeType](./literals.md#retrieveandgeneratetypetype)
- [RetrievePaginatorName](./literals.md#retrievepaginatorname)
- [SourceType](./literals.md#sourcetype)
- [TypeType](./literals.md#typetype)
- [AgentsforBedrockRuntimeServiceName](./literals.md#agentsforbedrockruntimeservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccessDeniedExceptionTypeDef](./type_defs.md#accessdeniedexceptiontypedef)
- [ParameterTypeDef](./type_defs.md#parametertypedef)
- [ActionGroupInvocationOutputTypeDef](./type_defs.md#actiongroupinvocationoutputtypedef)
- [BadGatewayExceptionTypeDef](./type_defs.md#badgatewayexceptiontypedef)
- [ConflictExceptionTypeDef](./type_defs.md#conflictexceptiontypedef)
- [DependencyFailedExceptionTypeDef](./type_defs.md#dependencyfailedexceptiontypedef)
- [FailureTraceTypeDef](./type_defs.md#failuretracetypedef)
- [FinalResponseTypeDef](./type_defs.md#finalresponsetypedef)
- [InferenceConfigurationTypeDef](./type_defs.md#inferenceconfigurationtypedef)
- [InternalServerExceptionTypeDef](./type_defs.md#internalserverexceptiontypedef)
- [KnowledgeBaseLookupInputTypeDef](./type_defs.md#knowledgebaselookupinputtypedef)
- [SessionStateTypeDef](./type_defs.md#sessionstatetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [KnowledgeBaseQueryTypeDef](./type_defs.md#knowledgebasequerytypedef)
- [KnowledgeBaseVectorSearchConfigurationTypeDef](./type_defs.md#knowledgebasevectorsearchconfigurationtypedef)
- [RetrievalResultContentTypeDef](./type_defs.md#retrievalresultcontenttypedef)
- [KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef](./type_defs.md#knowledgebaseretrieveandgenerateconfigurationtypedef)
- [RepromptResponseTypeDef](./type_defs.md#repromptresponsetypedef)
- [RationaleTypeDef](./type_defs.md#rationaletypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [PostProcessingParsedResponseTypeDef](./type_defs.md#postprocessingparsedresponsetypedef)
- [PreProcessingParsedResponseTypeDef](./type_defs.md#preprocessingparsedresponsetypedef)
- [ResourceNotFoundExceptionTypeDef](./type_defs.md#resourcenotfoundexceptiontypedef)
- [ServiceQuotaExceededExceptionTypeDef](./type_defs.md#servicequotaexceededexceptiontypedef)
- [ThrottlingExceptionTypeDef](./type_defs.md#throttlingexceptiontypedef)
- [ValidationExceptionTypeDef](./type_defs.md#validationexceptiontypedef)
- [RetrievalResultS3LocationTypeDef](./type_defs.md#retrievalresults3locationtypedef)
- [RetrieveAndGenerateInputTypeDef](./type_defs.md#retrieveandgenerateinputtypedef)
- [RetrieveAndGenerateOutputTypeDef](./type_defs.md#retrieveandgenerateoutputtypedef)
- [RetrieveAndGenerateSessionConfigurationTypeDef](./type_defs.md#retrieveandgeneratesessionconfigurationtypedef)
- [SpanTypeDef](./type_defs.md#spantypedef)
- [RequestBodyTypeDef](./type_defs.md#requestbodytypedef)
- [ModelInvocationInputTypeDef](./type_defs.md#modelinvocationinputtypedef)
- [InvokeAgentRequestRequestTypeDef](./type_defs.md#invokeagentrequestrequesttypedef)
- [KnowledgeBaseRetrievalConfigurationTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationtypedef)
- [RetrieveAndGenerateConfigurationTypeDef](./type_defs.md#retrieveandgenerateconfigurationtypedef)
- [PostProcessingModelInvocationOutputTypeDef](./type_defs.md#postprocessingmodelinvocationoutputtypedef)
- [PreProcessingModelInvocationOutputTypeDef](./type_defs.md#preprocessingmodelinvocationoutputtypedef)
- [RetrievalResultLocationTypeDef](./type_defs.md#retrievalresultlocationtypedef)
- [TextResponsePartTypeDef](./type_defs.md#textresponseparttypedef)
- [ActionGroupInvocationInputTypeDef](./type_defs.md#actiongroupinvocationinputtypedef)
- [RetrieveRequestRequestTypeDef](./type_defs.md#retrieverequestrequesttypedef)
- [RetrieveRequestRetrievePaginateTypeDef](./type_defs.md#retrieverequestretrievepaginatetypedef)
- [RetrieveAndGenerateRequestRequestTypeDef](./type_defs.md#retrieveandgeneraterequestrequesttypedef)
- [PostProcessingTraceTypeDef](./type_defs.md#postprocessingtracetypedef)
- [PreProcessingTraceTypeDef](./type_defs.md#preprocessingtracetypedef)
- [KnowledgeBaseRetrievalResultTypeDef](./type_defs.md#knowledgebaseretrievalresulttypedef)
- [RetrievedReferenceTypeDef](./type_defs.md#retrievedreferencetypedef)
- [GeneratedResponsePartTypeDef](./type_defs.md#generatedresponseparttypedef)
- [InvocationInputTypeDef](./type_defs.md#invocationinputtypedef)
- [RetrieveResponseTypeDef](./type_defs.md#retrieveresponsetypedef)
- [KnowledgeBaseLookupOutputTypeDef](./type_defs.md#knowledgebaselookupoutputtypedef)
- [CitationTypeDef](./type_defs.md#citationtypedef)
- [ObservationTypeDef](./type_defs.md#observationtypedef)
- [AttributionTypeDef](./type_defs.md#attributiontypedef)
- [RetrieveAndGenerateResponseTypeDef](./type_defs.md#retrieveandgenerateresponsetypedef)
- [OrchestrationTraceTypeDef](./type_defs.md#orchestrationtracetypedef)
- [PayloadPartTypeDef](./type_defs.md#payloadparttypedef)
- [TraceTypeDef](./type_defs.md#tracetypedef)
- [TracePartTypeDef](./type_defs.md#traceparttypedef)
- [ResponseStreamTypeDef](./type_defs.md#responsestreamtypedef)
- [InvokeAgentResponseTypeDef](./type_defs.md#invokeagentresponsetypedef)

