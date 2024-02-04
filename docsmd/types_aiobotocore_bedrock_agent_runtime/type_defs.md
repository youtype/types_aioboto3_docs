# Type definitions

> [Index](../README.md) > [AgentsforBedrockRuntime](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AgentsforBedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime)
    type annotations stubs module [types-aiobotocore-bedrock-agent-runtime](https://pypi.org/project/types-aiobotocore-bedrock-agent-runtime/).



## AccessDeniedExceptionTypeDef

```python
# AccessDeniedExceptionTypeDef definition

class AccessDeniedExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## ParameterTypeDef

```python
# ParameterTypeDef definition

class ParameterTypeDef(TypedDict):
    name: NotRequired[str],
    type: NotRequired[str],
    value: NotRequired[str],
```

## ActionGroupInvocationOutputTypeDef

```python
# ActionGroupInvocationOutputTypeDef definition

class ActionGroupInvocationOutputTypeDef(TypedDict):
    text: NotRequired[str],
```

## BadGatewayExceptionTypeDef

```python
# BadGatewayExceptionTypeDef definition

class BadGatewayExceptionTypeDef(TypedDict):
    message: NotRequired[str],
    resourceName: NotRequired[str],
```

## ConflictExceptionTypeDef

```python
# ConflictExceptionTypeDef definition

class ConflictExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## DependencyFailedExceptionTypeDef

```python
# DependencyFailedExceptionTypeDef definition

class DependencyFailedExceptionTypeDef(TypedDict):
    message: NotRequired[str],
    resourceName: NotRequired[str],
```

## FailureTraceTypeDef

```python
# FailureTraceTypeDef definition

class FailureTraceTypeDef(TypedDict):
    traceId: NotRequired[str],
    failureReason: NotRequired[str],
```

## FinalResponseTypeDef

```python
# FinalResponseTypeDef definition

class FinalResponseTypeDef(TypedDict):
    text: NotRequired[str],
```

## InferenceConfigurationTypeDef

```python
# InferenceConfigurationTypeDef definition

class InferenceConfigurationTypeDef(TypedDict):
    temperature: NotRequired[float],
    topP: NotRequired[float],
    topK: NotRequired[int],
    maximumLength: NotRequired[int],
    stopSequences: NotRequired[List[str]],
```

## InternalServerExceptionTypeDef

```python
# InternalServerExceptionTypeDef definition

class InternalServerExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## KnowledgeBaseLookupInputTypeDef

```python
# KnowledgeBaseLookupInputTypeDef definition

class KnowledgeBaseLookupInputTypeDef(TypedDict):
    text: NotRequired[str],
    knowledgeBaseId: NotRequired[str],
```

## SessionStateTypeDef

```python
# SessionStateTypeDef definition

class SessionStateTypeDef(TypedDict):
    sessionAttributes: NotRequired[Mapping[str, str]],
    promptSessionAttributes: NotRequired[Mapping[str, str]],
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

## KnowledgeBaseQueryTypeDef

```python
# KnowledgeBaseQueryTypeDef definition

class KnowledgeBaseQueryTypeDef(TypedDict):
    text: str,
```

## KnowledgeBaseVectorSearchConfigurationTypeDef

```python
# KnowledgeBaseVectorSearchConfigurationTypeDef definition

class KnowledgeBaseVectorSearchConfigurationTypeDef(TypedDict):
    numberOfResults: int,
```

## RetrievalResultContentTypeDef

```python
# RetrievalResultContentTypeDef definition

class RetrievalResultContentTypeDef(TypedDict):
    text: str,
```

## KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef

```python
# KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef definition

class KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef(TypedDict):
    knowledgeBaseId: str,
    modelArn: str,
```

## RepromptResponseTypeDef

```python
# RepromptResponseTypeDef definition

class RepromptResponseTypeDef(TypedDict):
    text: NotRequired[str],
    source: NotRequired[SourceType],  # (1)
```

1. See [:material-code-brackets: SourceType](./literals.md#sourcetype) 
## RationaleTypeDef

```python
# RationaleTypeDef definition

class RationaleTypeDef(TypedDict):
    traceId: NotRequired[str],
    text: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## PostProcessingParsedResponseTypeDef

```python
# PostProcessingParsedResponseTypeDef definition

class PostProcessingParsedResponseTypeDef(TypedDict):
    text: NotRequired[str],
```

## PreProcessingParsedResponseTypeDef

```python
# PreProcessingParsedResponseTypeDef definition

class PreProcessingParsedResponseTypeDef(TypedDict):
    rationale: NotRequired[str],
    isValid: NotRequired[bool],
```

## ResourceNotFoundExceptionTypeDef

```python
# ResourceNotFoundExceptionTypeDef definition

class ResourceNotFoundExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## ServiceQuotaExceededExceptionTypeDef

```python
# ServiceQuotaExceededExceptionTypeDef definition

class ServiceQuotaExceededExceptionTypeDef(TypedDict):
    message: NotRequired[str],
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

## RetrievalResultS3LocationTypeDef

```python
# RetrievalResultS3LocationTypeDef definition

class RetrievalResultS3LocationTypeDef(TypedDict):
    uri: NotRequired[str],
```

## RetrieveAndGenerateInputTypeDef

```python
# RetrieveAndGenerateInputTypeDef definition

class RetrieveAndGenerateInputTypeDef(TypedDict):
    text: str,
```

## RetrieveAndGenerateOutputTypeDef

```python
# RetrieveAndGenerateOutputTypeDef definition

class RetrieveAndGenerateOutputTypeDef(TypedDict):
    text: str,
```

## RetrieveAndGenerateSessionConfigurationTypeDef

```python
# RetrieveAndGenerateSessionConfigurationTypeDef definition

class RetrieveAndGenerateSessionConfigurationTypeDef(TypedDict):
    kmsKeyArn: str,
```

## SpanTypeDef

```python
# SpanTypeDef definition

class SpanTypeDef(TypedDict):
    start: NotRequired[int],
    end: NotRequired[int],
```

## RequestBodyTypeDef

```python
# RequestBodyTypeDef definition

class RequestBodyTypeDef(TypedDict):
    content: NotRequired[Dict[str, List[ParameterTypeDef]]],  # (1)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
## ModelInvocationInputTypeDef

```python
# ModelInvocationInputTypeDef definition

class ModelInvocationInputTypeDef(TypedDict):
    traceId: NotRequired[str],
    text: NotRequired[str],
    type: NotRequired[PromptTypeType],  # (1)
    inferenceConfiguration: NotRequired[InferenceConfigurationTypeDef],  # (2)
    overrideLambda: NotRequired[str],
    promptCreationMode: NotRequired[CreationModeType],  # (3)
    parserMode: NotRequired[CreationModeType],  # (3)
```

1. See [:material-code-brackets: PromptTypeType](./literals.md#prompttypetype) 
2. See [:material-code-braces: InferenceConfigurationTypeDef](./type_defs.md#inferenceconfigurationtypedef) 
3. See [:material-code-brackets: CreationModeType](./literals.md#creationmodetype) 
4. See [:material-code-brackets: CreationModeType](./literals.md#creationmodetype) 
## InvokeAgentRequestRequestTypeDef

```python
# InvokeAgentRequestRequestTypeDef definition

class InvokeAgentRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentAliasId: str,
    sessionId: str,
    inputText: str,
    sessionState: NotRequired[SessionStateTypeDef],  # (1)
    endSession: NotRequired[bool],
    enableTrace: NotRequired[bool],
```

1. See [:material-code-braces: SessionStateTypeDef](./type_defs.md#sessionstatetypedef) 
## KnowledgeBaseRetrievalConfigurationTypeDef

```python
# KnowledgeBaseRetrievalConfigurationTypeDef definition

class KnowledgeBaseRetrievalConfigurationTypeDef(TypedDict):
    vectorSearchConfiguration: KnowledgeBaseVectorSearchConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: KnowledgeBaseVectorSearchConfigurationTypeDef](./type_defs.md#knowledgebasevectorsearchconfigurationtypedef) 
## RetrieveAndGenerateConfigurationTypeDef

```python
# RetrieveAndGenerateConfigurationTypeDef definition

class RetrieveAndGenerateConfigurationTypeDef(TypedDict):
    type: RetrieveAndGenerateTypeType,  # (1)
    knowledgeBaseConfiguration: NotRequired[KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: RetrieveAndGenerateTypeType](./literals.md#retrieveandgeneratetypetype) 
2. See [:material-code-braces: KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef](./type_defs.md#knowledgebaseretrieveandgenerateconfigurationtypedef) 
## PostProcessingModelInvocationOutputTypeDef

```python
# PostProcessingModelInvocationOutputTypeDef definition

class PostProcessingModelInvocationOutputTypeDef(TypedDict):
    traceId: NotRequired[str],
    parsedResponse: NotRequired[PostProcessingParsedResponseTypeDef],  # (1)
```

1. See [:material-code-braces: PostProcessingParsedResponseTypeDef](./type_defs.md#postprocessingparsedresponsetypedef) 
## PreProcessingModelInvocationOutputTypeDef

```python
# PreProcessingModelInvocationOutputTypeDef definition

class PreProcessingModelInvocationOutputTypeDef(TypedDict):
    traceId: NotRequired[str],
    parsedResponse: NotRequired[PreProcessingParsedResponseTypeDef],  # (1)
```

1. See [:material-code-braces: PreProcessingParsedResponseTypeDef](./type_defs.md#preprocessingparsedresponsetypedef) 
## RetrievalResultLocationTypeDef

```python
# RetrievalResultLocationTypeDef definition

class RetrievalResultLocationTypeDef(TypedDict):
    type: RetrievalResultLocationTypeType,  # (1)
    s3Location: NotRequired[RetrievalResultS3LocationTypeDef],  # (2)
```

1. See [:material-code-brackets: RetrievalResultLocationTypeType](./literals.md#retrievalresultlocationtypetype) 
2. See [:material-code-braces: RetrievalResultS3LocationTypeDef](./type_defs.md#retrievalresults3locationtypedef) 
## TextResponsePartTypeDef

```python
# TextResponsePartTypeDef definition

class TextResponsePartTypeDef(TypedDict):
    text: NotRequired[str],
    span: NotRequired[SpanTypeDef],  # (1)
```

1. See [:material-code-braces: SpanTypeDef](./type_defs.md#spantypedef) 
## ActionGroupInvocationInputTypeDef

```python
# ActionGroupInvocationInputTypeDef definition

class ActionGroupInvocationInputTypeDef(TypedDict):
    actionGroupName: NotRequired[str],
    verb: NotRequired[str],
    apiPath: NotRequired[str],
    parameters: NotRequired[List[ParameterTypeDef]],  # (1)
    requestBody: NotRequired[RequestBodyTypeDef],  # (2)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
2. See [:material-code-braces: RequestBodyTypeDef](./type_defs.md#requestbodytypedef) 
## RetrieveRequestRequestTypeDef

```python
# RetrieveRequestRequestTypeDef definition

class RetrieveRequestRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    retrievalQuery: KnowledgeBaseQueryTypeDef,  # (1)
    retrievalConfiguration: NotRequired[KnowledgeBaseRetrievalConfigurationTypeDef],  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: KnowledgeBaseQueryTypeDef](./type_defs.md#knowledgebasequerytypedef) 
2. See [:material-code-braces: KnowledgeBaseRetrievalConfigurationTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationtypedef) 
## RetrieveRequestRetrievePaginateTypeDef

```python
# RetrieveRequestRetrievePaginateTypeDef definition

class RetrieveRequestRetrievePaginateTypeDef(TypedDict):
    knowledgeBaseId: str,
    retrievalQuery: KnowledgeBaseQueryTypeDef,  # (1)
    retrievalConfiguration: NotRequired[KnowledgeBaseRetrievalConfigurationTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: KnowledgeBaseQueryTypeDef](./type_defs.md#knowledgebasequerytypedef) 
2. See [:material-code-braces: KnowledgeBaseRetrievalConfigurationTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationtypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## RetrieveAndGenerateRequestRequestTypeDef

```python
# RetrieveAndGenerateRequestRequestTypeDef definition

class RetrieveAndGenerateRequestRequestTypeDef(TypedDict):
    input: RetrieveAndGenerateInputTypeDef,  # (1)
    sessionId: NotRequired[str],
    retrieveAndGenerateConfiguration: NotRequired[RetrieveAndGenerateConfigurationTypeDef],  # (2)
    sessionConfiguration: NotRequired[RetrieveAndGenerateSessionConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: RetrieveAndGenerateInputTypeDef](./type_defs.md#retrieveandgenerateinputtypedef) 
2. See [:material-code-braces: RetrieveAndGenerateConfigurationTypeDef](./type_defs.md#retrieveandgenerateconfigurationtypedef) 
3. See [:material-code-braces: RetrieveAndGenerateSessionConfigurationTypeDef](./type_defs.md#retrieveandgeneratesessionconfigurationtypedef) 
## PostProcessingTraceTypeDef

```python
# PostProcessingTraceTypeDef definition

class PostProcessingTraceTypeDef(TypedDict):
    modelInvocationInput: NotRequired[ModelInvocationInputTypeDef],  # (1)
    modelInvocationOutput: NotRequired[PostProcessingModelInvocationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ModelInvocationInputTypeDef](./type_defs.md#modelinvocationinputtypedef) 
2. See [:material-code-braces: PostProcessingModelInvocationOutputTypeDef](./type_defs.md#postprocessingmodelinvocationoutputtypedef) 
## PreProcessingTraceTypeDef

```python
# PreProcessingTraceTypeDef definition

class PreProcessingTraceTypeDef(TypedDict):
    modelInvocationInput: NotRequired[ModelInvocationInputTypeDef],  # (1)
    modelInvocationOutput: NotRequired[PreProcessingModelInvocationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ModelInvocationInputTypeDef](./type_defs.md#modelinvocationinputtypedef) 
2. See [:material-code-braces: PreProcessingModelInvocationOutputTypeDef](./type_defs.md#preprocessingmodelinvocationoutputtypedef) 
## KnowledgeBaseRetrievalResultTypeDef

```python
# KnowledgeBaseRetrievalResultTypeDef definition

class KnowledgeBaseRetrievalResultTypeDef(TypedDict):
    content: RetrievalResultContentTypeDef,  # (1)
    location: NotRequired[RetrievalResultLocationTypeDef],  # (2)
    score: NotRequired[float],
```

1. See [:material-code-braces: RetrievalResultContentTypeDef](./type_defs.md#retrievalresultcontenttypedef) 
2. See [:material-code-braces: RetrievalResultLocationTypeDef](./type_defs.md#retrievalresultlocationtypedef) 
## RetrievedReferenceTypeDef

```python
# RetrievedReferenceTypeDef definition

class RetrievedReferenceTypeDef(TypedDict):
    content: NotRequired[RetrievalResultContentTypeDef],  # (1)
    location: NotRequired[RetrievalResultLocationTypeDef],  # (2)
```

1. See [:material-code-braces: RetrievalResultContentTypeDef](./type_defs.md#retrievalresultcontenttypedef) 
2. See [:material-code-braces: RetrievalResultLocationTypeDef](./type_defs.md#retrievalresultlocationtypedef) 
## GeneratedResponsePartTypeDef

```python
# GeneratedResponsePartTypeDef definition

class GeneratedResponsePartTypeDef(TypedDict):
    textResponsePart: NotRequired[TextResponsePartTypeDef],  # (1)
```

1. See [:material-code-braces: TextResponsePartTypeDef](./type_defs.md#textresponseparttypedef) 
## InvocationInputTypeDef

```python
# InvocationInputTypeDef definition

class InvocationInputTypeDef(TypedDict):
    traceId: NotRequired[str],
    invocationType: NotRequired[InvocationTypeType],  # (1)
    actionGroupInvocationInput: NotRequired[ActionGroupInvocationInputTypeDef],  # (2)
    knowledgeBaseLookupInput: NotRequired[KnowledgeBaseLookupInputTypeDef],  # (3)
```

1. See [:material-code-brackets: InvocationTypeType](./literals.md#invocationtypetype) 
2. See [:material-code-braces: ActionGroupInvocationInputTypeDef](./type_defs.md#actiongroupinvocationinputtypedef) 
3. See [:material-code-braces: KnowledgeBaseLookupInputTypeDef](./type_defs.md#knowledgebaselookupinputtypedef) 
## RetrieveResponseTypeDef

```python
# RetrieveResponseTypeDef definition

class RetrieveResponseTypeDef(TypedDict):
    retrievalResults: List[KnowledgeBaseRetrievalResultTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KnowledgeBaseRetrievalResultTypeDef](./type_defs.md#knowledgebaseretrievalresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## KnowledgeBaseLookupOutputTypeDef

```python
# KnowledgeBaseLookupOutputTypeDef definition

class KnowledgeBaseLookupOutputTypeDef(TypedDict):
    retrievedReferences: NotRequired[List[RetrievedReferenceTypeDef]],  # (1)
```

1. See [:material-code-braces: RetrievedReferenceTypeDef](./type_defs.md#retrievedreferencetypedef) 
## CitationTypeDef

```python
# CitationTypeDef definition

class CitationTypeDef(TypedDict):
    generatedResponsePart: NotRequired[GeneratedResponsePartTypeDef],  # (1)
    retrievedReferences: NotRequired[List[RetrievedReferenceTypeDef]],  # (2)
```

1. See [:material-code-braces: GeneratedResponsePartTypeDef](./type_defs.md#generatedresponseparttypedef) 
2. See [:material-code-braces: RetrievedReferenceTypeDef](./type_defs.md#retrievedreferencetypedef) 
## ObservationTypeDef

```python
# ObservationTypeDef definition

class ObservationTypeDef(TypedDict):
    traceId: NotRequired[str],
    type: NotRequired[TypeType],  # (1)
    actionGroupInvocationOutput: NotRequired[ActionGroupInvocationOutputTypeDef],  # (2)
    knowledgeBaseLookupOutput: NotRequired[KnowledgeBaseLookupOutputTypeDef],  # (3)
    finalResponse: NotRequired[FinalResponseTypeDef],  # (4)
    repromptResponse: NotRequired[RepromptResponseTypeDef],  # (5)
```

1. See [:material-code-brackets: TypeType](./literals.md#typetype) 
2. See [:material-code-braces: ActionGroupInvocationOutputTypeDef](./type_defs.md#actiongroupinvocationoutputtypedef) 
3. See [:material-code-braces: KnowledgeBaseLookupOutputTypeDef](./type_defs.md#knowledgebaselookupoutputtypedef) 
4. See [:material-code-braces: FinalResponseTypeDef](./type_defs.md#finalresponsetypedef) 
5. See [:material-code-braces: RepromptResponseTypeDef](./type_defs.md#repromptresponsetypedef) 
## AttributionTypeDef

```python
# AttributionTypeDef definition

class AttributionTypeDef(TypedDict):
    citations: NotRequired[List[CitationTypeDef]],  # (1)
```

1. See [:material-code-braces: CitationTypeDef](./type_defs.md#citationtypedef) 
## RetrieveAndGenerateResponseTypeDef

```python
# RetrieveAndGenerateResponseTypeDef definition

class RetrieveAndGenerateResponseTypeDef(TypedDict):
    sessionId: str,
    output: RetrieveAndGenerateOutputTypeDef,  # (1)
    citations: List[CitationTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RetrieveAndGenerateOutputTypeDef](./type_defs.md#retrieveandgenerateoutputtypedef) 
2. See [:material-code-braces: CitationTypeDef](./type_defs.md#citationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OrchestrationTraceTypeDef

```python
# OrchestrationTraceTypeDef definition

class OrchestrationTraceTypeDef(TypedDict):
    rationale: NotRequired[RationaleTypeDef],  # (1)
    invocationInput: NotRequired[InvocationInputTypeDef],  # (2)
    observation: NotRequired[ObservationTypeDef],  # (3)
    modelInvocationInput: NotRequired[ModelInvocationInputTypeDef],  # (4)
```

1. See [:material-code-braces: RationaleTypeDef](./type_defs.md#rationaletypedef) 
2. See [:material-code-braces: InvocationInputTypeDef](./type_defs.md#invocationinputtypedef) 
3. See [:material-code-braces: ObservationTypeDef](./type_defs.md#observationtypedef) 
4. See [:material-code-braces: ModelInvocationInputTypeDef](./type_defs.md#modelinvocationinputtypedef) 
## PayloadPartTypeDef

```python
# PayloadPartTypeDef definition

class PayloadPartTypeDef(TypedDict):
    bytes: NotRequired[bytes],
    attribution: NotRequired[AttributionTypeDef],  # (1)
```

1. See [:material-code-braces: AttributionTypeDef](./type_defs.md#attributiontypedef) 
## TraceTypeDef

```python
# TraceTypeDef definition

class TraceTypeDef(TypedDict):
    preProcessingTrace: NotRequired[PreProcessingTraceTypeDef],  # (1)
    orchestrationTrace: NotRequired[OrchestrationTraceTypeDef],  # (2)
    postProcessingTrace: NotRequired[PostProcessingTraceTypeDef],  # (3)
    failureTrace: NotRequired[FailureTraceTypeDef],  # (4)
```

1. See [:material-code-braces: PreProcessingTraceTypeDef](./type_defs.md#preprocessingtracetypedef) 
2. See [:material-code-braces: OrchestrationTraceTypeDef](./type_defs.md#orchestrationtracetypedef) 
3. See [:material-code-braces: PostProcessingTraceTypeDef](./type_defs.md#postprocessingtracetypedef) 
4. See [:material-code-braces: FailureTraceTypeDef](./type_defs.md#failuretracetypedef) 
## TracePartTypeDef

```python
# TracePartTypeDef definition

class TracePartTypeDef(TypedDict):
    agentId: NotRequired[str],
    agentAliasId: NotRequired[str],
    sessionId: NotRequired[str],
    trace: NotRequired[TraceTypeDef],  # (1)
```

1. See [:material-code-braces: TraceTypeDef](./type_defs.md#tracetypedef) 
## ResponseStreamTypeDef

```python
# ResponseStreamTypeDef definition

class ResponseStreamTypeDef(TypedDict):
    chunk: NotRequired[PayloadPartTypeDef],  # (1)
    trace: NotRequired[TracePartTypeDef],  # (2)
    internalServerException: NotRequired[InternalServerExceptionTypeDef],  # (3)
    validationException: NotRequired[ValidationExceptionTypeDef],  # (4)
    resourceNotFoundException: NotRequired[ResourceNotFoundExceptionTypeDef],  # (5)
    serviceQuotaExceededException: NotRequired[ServiceQuotaExceededExceptionTypeDef],  # (6)
    throttlingException: NotRequired[ThrottlingExceptionTypeDef],  # (7)
    accessDeniedException: NotRequired[AccessDeniedExceptionTypeDef],  # (8)
    conflictException: NotRequired[ConflictExceptionTypeDef],  # (9)
    dependencyFailedException: NotRequired[DependencyFailedExceptionTypeDef],  # (10)
    badGatewayException: NotRequired[BadGatewayExceptionTypeDef],  # (11)
```

1. See [:material-code-braces: PayloadPartTypeDef](./type_defs.md#payloadparttypedef) 
2. See [:material-code-braces: TracePartTypeDef](./type_defs.md#traceparttypedef) 
3. See [:material-code-braces: InternalServerExceptionTypeDef](./type_defs.md#internalserverexceptiontypedef) 
4. See [:material-code-braces: ValidationExceptionTypeDef](./type_defs.md#validationexceptiontypedef) 
5. See [:material-code-braces: ResourceNotFoundExceptionTypeDef](./type_defs.md#resourcenotfoundexceptiontypedef) 
6. See [:material-code-braces: ServiceQuotaExceededExceptionTypeDef](./type_defs.md#servicequotaexceededexceptiontypedef) 
7. See [:material-code-braces: ThrottlingExceptionTypeDef](./type_defs.md#throttlingexceptiontypedef) 
8. See [:material-code-braces: AccessDeniedExceptionTypeDef](./type_defs.md#accessdeniedexceptiontypedef) 
9. See [:material-code-braces: ConflictExceptionTypeDef](./type_defs.md#conflictexceptiontypedef) 
10. See [:material-code-braces: DependencyFailedExceptionTypeDef](./type_defs.md#dependencyfailedexceptiontypedef) 
11. See [:material-code-braces: BadGatewayExceptionTypeDef](./type_defs.md#badgatewayexceptiontypedef) 
## InvokeAgentResponseTypeDef

```python
# InvokeAgentResponseTypeDef definition

class InvokeAgentResponseTypeDef(TypedDict):
    completion: AioEventStream[ResponseStreamTypeDef],  # (1)
    contentType: str,
    sessionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResponseStreamTypeDef](./type_defs.md#responsestreamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
