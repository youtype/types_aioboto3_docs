# Type definitions

> [Index](../README.md) > [LexModelBuildingService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [LexModelBuildingService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#lexmodelbuildingservice)
    type annotations stubs module [types-aiobotocore-lex-models](https://pypi.org/project/types-aiobotocore-lex-models/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## EnumerationValueUnionTypeDef

```python
# EnumerationValueUnionTypeDef definition

EnumerationValueUnionTypeDef = Union[
    EnumerationValueTypeDef,  # (1)
    EnumerationValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EnumerationValueTypeDef](./type_defs.md#enumerationvaluetypedef) 
2. See [:material-code-braces: EnumerationValueOutputTypeDef](./type_defs.md#enumerationvalueoutputtypedef) 

## PromptUnionTypeDef

```python
# PromptUnionTypeDef definition

PromptUnionTypeDef = Union[
    PromptTypeDef,  # (1)
    PromptOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PromptTypeDef](./type_defs.md#prompttypedef) 
2. See [:material-code-braces: PromptOutputTypeDef](./type_defs.md#promptoutputtypedef) 

## StatementUnionTypeDef

```python
# StatementUnionTypeDef definition

StatementUnionTypeDef = Union[
    StatementTypeDef,  # (1)
    StatementOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: StatementTypeDef](./type_defs.md#statementtypedef) 
2. See [:material-code-braces: StatementOutputTypeDef](./type_defs.md#statementoutputtypedef) 

## SlotDefaultValueSpecUnionTypeDef

```python
# SlotDefaultValueSpecUnionTypeDef definition

SlotDefaultValueSpecUnionTypeDef = Union[
    SlotDefaultValueSpecTypeDef,  # (1)
    SlotDefaultValueSpecOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SlotDefaultValueSpecTypeDef](./type_defs.md#slotdefaultvaluespectypedef) 
2. See [:material-code-braces: SlotDefaultValueSpecOutputTypeDef](./type_defs.md#slotdefaultvaluespecoutputtypedef) 

## SlotUnionTypeDef

```python
# SlotUnionTypeDef definition

SlotUnionTypeDef = Union[
    SlotTypeDef,  # (1)
    SlotOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SlotTypeDef](./type_defs.md#slottypedef) 
2. See [:material-code-braces: SlotOutputTypeDef](./type_defs.md#slotoutputtypedef) 



## BotChannelAssociationTypeDef

```python
# BotChannelAssociationTypeDef definition

class BotChannelAssociationTypeDef(TypedDict):
    name: NotRequired[str],
    description: NotRequired[str],
    botAlias: NotRequired[str],
    botName: NotRequired[str],
    createdDate: NotRequired[datetime],
    type: NotRequired[ChannelTypeType],  # (1)
    botConfiguration: NotRequired[dict[str, str]],
    status: NotRequired[ChannelStatusType],  # (2)
    failureReason: NotRequired[str],
```

1. See [:material-code-brackets: ChannelTypeType](./literals.md#channeltypetype) 
2. See [:material-code-brackets: ChannelStatusType](./literals.md#channelstatustype) 
## BotMetadataTypeDef

```python
# BotMetadataTypeDef definition

class BotMetadataTypeDef(TypedDict):
    name: NotRequired[str],
    description: NotRequired[str],
    status: NotRequired[StatusType],  # (1)
    lastUpdatedDate: NotRequired[datetime],
    createdDate: NotRequired[datetime],
    version: NotRequired[str],
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## BuiltinIntentMetadataTypeDef

```python
# BuiltinIntentMetadataTypeDef definition

class BuiltinIntentMetadataTypeDef(TypedDict):
    signature: NotRequired[str],
    supportedLocales: NotRequired[list[LocaleType]],  # (1)
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
## BuiltinIntentSlotTypeDef

```python
# BuiltinIntentSlotTypeDef definition

class BuiltinIntentSlotTypeDef(TypedDict):
    name: NotRequired[str],
```

## BuiltinSlotTypeMetadataTypeDef

```python
# BuiltinSlotTypeMetadataTypeDef definition

class BuiltinSlotTypeMetadataTypeDef(TypedDict):
    signature: NotRequired[str],
    supportedLocales: NotRequired[list[LocaleType]],  # (1)
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
## CodeHookTypeDef

```python
# CodeHookTypeDef definition

class CodeHookTypeDef(TypedDict):
    uri: str,
    messageVersion: str,
```

## LogSettingsRequestTypeDef

```python
# LogSettingsRequestTypeDef definition

class LogSettingsRequestTypeDef(TypedDict):
    logType: LogTypeType,  # (1)
    destination: DestinationType,  # (2)
    resourceArn: str,
    kmsKeyArn: NotRequired[str],
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
2. See [:material-code-brackets: DestinationType](./literals.md#destinationtype) 
## LogSettingsResponseTypeDef

```python
# LogSettingsResponseTypeDef definition

class LogSettingsResponseTypeDef(TypedDict):
    logType: NotRequired[LogTypeType],  # (1)
    destination: NotRequired[DestinationType],  # (2)
    kmsKeyArn: NotRequired[str],
    resourceArn: NotRequired[str],
    resourcePrefix: NotRequired[str],
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
2. See [:material-code-brackets: DestinationType](./literals.md#destinationtype) 
## CreateBotVersionRequestRequestTypeDef

```python
# CreateBotVersionRequestRequestTypeDef definition

class CreateBotVersionRequestRequestTypeDef(TypedDict):
    name: str,
    checksum: NotRequired[str],
```

## IntentTypeDef

```python
# IntentTypeDef definition

class IntentTypeDef(TypedDict):
    intentName: str,
    intentVersion: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## CreateIntentVersionRequestRequestTypeDef

```python
# CreateIntentVersionRequestRequestTypeDef definition

class CreateIntentVersionRequestRequestTypeDef(TypedDict):
    name: str,
    checksum: NotRequired[str],
```

## InputContextTypeDef

```python
# InputContextTypeDef definition

class InputContextTypeDef(TypedDict):
    name: str,
```

## KendraConfigurationTypeDef

```python
# KendraConfigurationTypeDef definition

class KendraConfigurationTypeDef(TypedDict):
    kendraIndex: str,
    role: str,
    queryFilterString: NotRequired[str],
```

## OutputContextTypeDef

```python
# OutputContextTypeDef definition

class OutputContextTypeDef(TypedDict):
    name: str,
    timeToLiveInSeconds: int,
    turnsToLive: int,
```

## CreateSlotTypeVersionRequestRequestTypeDef

```python
# CreateSlotTypeVersionRequestRequestTypeDef definition

class CreateSlotTypeVersionRequestRequestTypeDef(TypedDict):
    name: str,
    checksum: NotRequired[str],
```

## EnumerationValueOutputTypeDef

```python
# EnumerationValueOutputTypeDef definition

class EnumerationValueOutputTypeDef(TypedDict):
    value: str,
    synonyms: NotRequired[list[str]],
```

## DeleteBotAliasRequestRequestTypeDef

```python
# DeleteBotAliasRequestRequestTypeDef definition

class DeleteBotAliasRequestRequestTypeDef(TypedDict):
    name: str,
    botName: str,
```

## DeleteBotChannelAssociationRequestRequestTypeDef

```python
# DeleteBotChannelAssociationRequestRequestTypeDef definition

class DeleteBotChannelAssociationRequestRequestTypeDef(TypedDict):
    name: str,
    botName: str,
    botAlias: str,
```

## DeleteBotRequestRequestTypeDef

```python
# DeleteBotRequestRequestTypeDef definition

class DeleteBotRequestRequestTypeDef(TypedDict):
    name: str,
```

## DeleteBotVersionRequestRequestTypeDef

```python
# DeleteBotVersionRequestRequestTypeDef definition

class DeleteBotVersionRequestRequestTypeDef(TypedDict):
    name: str,
    version: str,
```

## DeleteIntentRequestRequestTypeDef

```python
# DeleteIntentRequestRequestTypeDef definition

class DeleteIntentRequestRequestTypeDef(TypedDict):
    name: str,
```

## DeleteIntentVersionRequestRequestTypeDef

```python
# DeleteIntentVersionRequestRequestTypeDef definition

class DeleteIntentVersionRequestRequestTypeDef(TypedDict):
    name: str,
    version: str,
```

## DeleteSlotTypeRequestRequestTypeDef

```python
# DeleteSlotTypeRequestRequestTypeDef definition

class DeleteSlotTypeRequestRequestTypeDef(TypedDict):
    name: str,
```

## DeleteSlotTypeVersionRequestRequestTypeDef

```python
# DeleteSlotTypeVersionRequestRequestTypeDef definition

class DeleteSlotTypeVersionRequestRequestTypeDef(TypedDict):
    name: str,
    version: str,
```

## DeleteUtterancesRequestRequestTypeDef

```python
# DeleteUtterancesRequestRequestTypeDef definition

class DeleteUtterancesRequestRequestTypeDef(TypedDict):
    botName: str,
    userId: str,
```

## EnumerationValueTypeDef

```python
# EnumerationValueTypeDef definition

class EnumerationValueTypeDef(TypedDict):
    value: str,
    synonyms: NotRequired[Sequence[str]],
```

## GetBotAliasRequestRequestTypeDef

```python
# GetBotAliasRequestRequestTypeDef definition

class GetBotAliasRequestRequestTypeDef(TypedDict):
    name: str,
    botName: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetBotAliasesRequestRequestTypeDef

```python
# GetBotAliasesRequestRequestTypeDef definition

class GetBotAliasesRequestRequestTypeDef(TypedDict):
    botName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    nameContains: NotRequired[str],
```

## GetBotChannelAssociationRequestRequestTypeDef

```python
# GetBotChannelAssociationRequestRequestTypeDef definition

class GetBotChannelAssociationRequestRequestTypeDef(TypedDict):
    name: str,
    botName: str,
    botAlias: str,
```

## GetBotChannelAssociationsRequestRequestTypeDef

```python
# GetBotChannelAssociationsRequestRequestTypeDef definition

class GetBotChannelAssociationsRequestRequestTypeDef(TypedDict):
    botName: str,
    botAlias: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    nameContains: NotRequired[str],
```

## GetBotRequestRequestTypeDef

```python
# GetBotRequestRequestTypeDef definition

class GetBotRequestRequestTypeDef(TypedDict):
    name: str,
    versionOrAlias: str,
```

## GetBotVersionsRequestRequestTypeDef

```python
# GetBotVersionsRequestRequestTypeDef definition

class GetBotVersionsRequestRequestTypeDef(TypedDict):
    name: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## GetBotsRequestRequestTypeDef

```python
# GetBotsRequestRequestTypeDef definition

class GetBotsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    nameContains: NotRequired[str],
```

## GetBuiltinIntentRequestRequestTypeDef

```python
# GetBuiltinIntentRequestRequestTypeDef definition

class GetBuiltinIntentRequestRequestTypeDef(TypedDict):
    signature: str,
```

## GetBuiltinIntentsRequestRequestTypeDef

```python
# GetBuiltinIntentsRequestRequestTypeDef definition

class GetBuiltinIntentsRequestRequestTypeDef(TypedDict):
    locale: NotRequired[LocaleType],  # (1)
    signatureContains: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
## GetBuiltinSlotTypesRequestRequestTypeDef

```python
# GetBuiltinSlotTypesRequestRequestTypeDef definition

class GetBuiltinSlotTypesRequestRequestTypeDef(TypedDict):
    locale: NotRequired[LocaleType],  # (1)
    signatureContains: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
## GetExportRequestRequestTypeDef

```python
# GetExportRequestRequestTypeDef definition

class GetExportRequestRequestTypeDef(TypedDict):
    name: str,
    version: str,
    resourceType: ResourceTypeType,  # (1)
    exportType: ExportTypeType,  # (2)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: ExportTypeType](./literals.md#exporttypetype) 
## GetImportRequestRequestTypeDef

```python
# GetImportRequestRequestTypeDef definition

class GetImportRequestRequestTypeDef(TypedDict):
    importId: str,
```

## GetIntentRequestRequestTypeDef

```python
# GetIntentRequestRequestTypeDef definition

class GetIntentRequestRequestTypeDef(TypedDict):
    name: str,
    version: str,
```

## GetIntentVersionsRequestRequestTypeDef

```python
# GetIntentVersionsRequestRequestTypeDef definition

class GetIntentVersionsRequestRequestTypeDef(TypedDict):
    name: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## IntentMetadataTypeDef

```python
# IntentMetadataTypeDef definition

class IntentMetadataTypeDef(TypedDict):
    name: NotRequired[str],
    description: NotRequired[str],
    lastUpdatedDate: NotRequired[datetime],
    createdDate: NotRequired[datetime],
    version: NotRequired[str],
```

## GetIntentsRequestRequestTypeDef

```python
# GetIntentsRequestRequestTypeDef definition

class GetIntentsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    nameContains: NotRequired[str],
```

## GetMigrationRequestRequestTypeDef

```python
# GetMigrationRequestRequestTypeDef definition

class GetMigrationRequestRequestTypeDef(TypedDict):
    migrationId: str,
```

## MigrationAlertTypeDef

```python
# MigrationAlertTypeDef definition

class MigrationAlertTypeDef(TypedDict):
    type: NotRequired[MigrationAlertTypeType],  # (1)
    message: NotRequired[str],
    details: NotRequired[list[str]],
    referenceURLs: NotRequired[list[str]],
```

1. See [:material-code-brackets: MigrationAlertTypeType](./literals.md#migrationalerttypetype) 
## GetMigrationsRequestRequestTypeDef

```python
# GetMigrationsRequestRequestTypeDef definition

class GetMigrationsRequestRequestTypeDef(TypedDict):
    sortByAttribute: NotRequired[MigrationSortAttributeType],  # (1)
    sortByOrder: NotRequired[SortOrderType],  # (2)
    v1BotNameContains: NotRequired[str],
    migrationStatusEquals: NotRequired[MigrationStatusType],  # (3)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: MigrationSortAttributeType](./literals.md#migrationsortattributetype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: MigrationStatusType](./literals.md#migrationstatustype) 
## MigrationSummaryTypeDef

```python
# MigrationSummaryTypeDef definition

class MigrationSummaryTypeDef(TypedDict):
    migrationId: NotRequired[str],
    v1BotName: NotRequired[str],
    v1BotVersion: NotRequired[str],
    v1BotLocale: NotRequired[LocaleType],  # (1)
    v2BotId: NotRequired[str],
    v2BotRole: NotRequired[str],
    migrationStatus: NotRequired[MigrationStatusType],  # (2)
    migrationStrategy: NotRequired[MigrationStrategyType],  # (3)
    migrationTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
2. See [:material-code-brackets: MigrationStatusType](./literals.md#migrationstatustype) 
3. See [:material-code-brackets: MigrationStrategyType](./literals.md#migrationstrategytype) 
## GetSlotTypeRequestRequestTypeDef

```python
# GetSlotTypeRequestRequestTypeDef definition

class GetSlotTypeRequestRequestTypeDef(TypedDict):
    name: str,
    version: str,
```

## GetSlotTypeVersionsRequestRequestTypeDef

```python
# GetSlotTypeVersionsRequestRequestTypeDef definition

class GetSlotTypeVersionsRequestRequestTypeDef(TypedDict):
    name: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## SlotTypeMetadataTypeDef

```python
# SlotTypeMetadataTypeDef definition

class SlotTypeMetadataTypeDef(TypedDict):
    name: NotRequired[str],
    description: NotRequired[str],
    lastUpdatedDate: NotRequired[datetime],
    createdDate: NotRequired[datetime],
    version: NotRequired[str],
```

## GetSlotTypesRequestRequestTypeDef

```python
# GetSlotTypesRequestRequestTypeDef definition

class GetSlotTypesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    nameContains: NotRequired[str],
```

## GetUtterancesViewRequestRequestTypeDef

```python
# GetUtterancesViewRequestRequestTypeDef definition

class GetUtterancesViewRequestRequestTypeDef(TypedDict):
    botName: str,
    botVersions: Sequence[str],
    statusType: StatusTypeType,  # (1)
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: str,
```

## MessageTypeDef

```python
# MessageTypeDef definition

class MessageTypeDef(TypedDict):
    contentType: ContentTypeType,  # (1)
    content: str,
    groupNumber: NotRequired[int],
```

1. See [:material-code-brackets: ContentTypeType](./literals.md#contenttypetype) 
## SlotDefaultValueTypeDef

```python
# SlotDefaultValueTypeDef definition

class SlotDefaultValueTypeDef(TypedDict):
    defaultValue: str,
```

## SlotTypeRegexConfigurationTypeDef

```python
# SlotTypeRegexConfigurationTypeDef definition

class SlotTypeRegexConfigurationTypeDef(TypedDict):
    pattern: str,
```

## StartMigrationRequestRequestTypeDef

```python
# StartMigrationRequestRequestTypeDef definition

class StartMigrationRequestRequestTypeDef(TypedDict):
    v1BotName: str,
    v1BotVersion: str,
    v2BotName: str,
    v2BotRole: str,
    migrationStrategy: MigrationStrategyType,  # (1)
```

1. See [:material-code-brackets: MigrationStrategyType](./literals.md#migrationstrategytype) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UtteranceDataTypeDef

```python
# UtteranceDataTypeDef definition

class UtteranceDataTypeDef(TypedDict):
    utteranceString: NotRequired[str],
    count: NotRequired[int],
    distinctUsers: NotRequired[int],
    firstUtteredDate: NotRequired[datetime],
    lastUtteredDate: NotRequired[datetime],
```

## FulfillmentActivityTypeDef

```python
# FulfillmentActivityTypeDef definition

class FulfillmentActivityTypeDef(TypedDict):
    type: FulfillmentActivityTypeType,  # (1)
    codeHook: NotRequired[CodeHookTypeDef],  # (2)
```

1. See [:material-code-brackets: FulfillmentActivityTypeType](./literals.md#fulfillmentactivitytypetype) 
2. See [:material-code-braces: CodeHookTypeDef](./type_defs.md#codehooktypedef) 
## ConversationLogsRequestTypeDef

```python
# ConversationLogsRequestTypeDef definition

class ConversationLogsRequestTypeDef(TypedDict):
    logSettings: Sequence[LogSettingsRequestTypeDef],  # (1)
    iamRoleArn: str,
```

1. See [:material-code-braces: LogSettingsRequestTypeDef](./type_defs.md#logsettingsrequesttypedef) 
## ConversationLogsResponseTypeDef

```python
# ConversationLogsResponseTypeDef definition

class ConversationLogsResponseTypeDef(TypedDict):
    logSettings: NotRequired[list[LogSettingsResponseTypeDef]],  # (1)
    iamRoleArn: NotRequired[str],
```

1. See [:material-code-braces: LogSettingsResponseTypeDef](./type_defs.md#logsettingsresponsetypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBotChannelAssociationResponseTypeDef

```python
# GetBotChannelAssociationResponseTypeDef definition

class GetBotChannelAssociationResponseTypeDef(TypedDict):
    name: str,
    description: str,
    botAlias: str,
    botName: str,
    createdDate: datetime,
    type: ChannelTypeType,  # (1)
    botConfiguration: dict[str, str],
    status: ChannelStatusType,  # (2)
    failureReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ChannelTypeType](./literals.md#channeltypetype) 
2. See [:material-code-brackets: ChannelStatusType](./literals.md#channelstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBotChannelAssociationsResponseTypeDef

```python
# GetBotChannelAssociationsResponseTypeDef definition

class GetBotChannelAssociationsResponseTypeDef(TypedDict):
    botChannelAssociations: list[BotChannelAssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BotChannelAssociationTypeDef](./type_defs.md#botchannelassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBotVersionsResponseTypeDef

```python
# GetBotVersionsResponseTypeDef definition

class GetBotVersionsResponseTypeDef(TypedDict):
    bots: list[BotMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BotMetadataTypeDef](./type_defs.md#botmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBotsResponseTypeDef

```python
# GetBotsResponseTypeDef definition

class GetBotsResponseTypeDef(TypedDict):
    bots: list[BotMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BotMetadataTypeDef](./type_defs.md#botmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBuiltinIntentResponseTypeDef

```python
# GetBuiltinIntentResponseTypeDef definition

class GetBuiltinIntentResponseTypeDef(TypedDict):
    signature: str,
    supportedLocales: list[LocaleType],  # (1)
    slots: list[BuiltinIntentSlotTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
2. See [:material-code-braces: BuiltinIntentSlotTypeDef](./type_defs.md#builtinintentslottypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBuiltinIntentsResponseTypeDef

```python
# GetBuiltinIntentsResponseTypeDef definition

class GetBuiltinIntentsResponseTypeDef(TypedDict):
    intents: list[BuiltinIntentMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BuiltinIntentMetadataTypeDef](./type_defs.md#builtinintentmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBuiltinSlotTypesResponseTypeDef

```python
# GetBuiltinSlotTypesResponseTypeDef definition

class GetBuiltinSlotTypesResponseTypeDef(TypedDict):
    slotTypes: list[BuiltinSlotTypeMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BuiltinSlotTypeMetadataTypeDef](./type_defs.md#builtinslottypemetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetExportResponseTypeDef

```python
# GetExportResponseTypeDef definition

class GetExportResponseTypeDef(TypedDict):
    name: str,
    version: str,
    resourceType: ResourceTypeType,  # (1)
    exportType: ExportTypeType,  # (2)
    exportStatus: ExportStatusType,  # (3)
    failureReason: str,
    url: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: ExportTypeType](./literals.md#exporttypetype) 
3. See [:material-code-brackets: ExportStatusType](./literals.md#exportstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetImportResponseTypeDef

```python
# GetImportResponseTypeDef definition

class GetImportResponseTypeDef(TypedDict):
    name: str,
    resourceType: ResourceTypeType,  # (1)
    mergeStrategy: MergeStrategyType,  # (2)
    importId: str,
    importStatus: ImportStatusType,  # (3)
    failureReason: list[str],
    createdDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: MergeStrategyType](./literals.md#mergestrategytype) 
3. See [:material-code-brackets: ImportStatusType](./literals.md#importstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMigrationResponseTypeDef

```python
# StartMigrationResponseTypeDef definition

class StartMigrationResponseTypeDef(TypedDict):
    v1BotName: str,
    v1BotVersion: str,
    v1BotLocale: LocaleType,  # (1)
    v2BotId: str,
    v2BotRole: str,
    migrationId: str,
    migrationStrategy: MigrationStrategyType,  # (2)
    migrationTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
2. See [:material-code-brackets: MigrationStrategyType](./literals.md#migrationstrategytype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBotAliasesRequestPaginateTypeDef

```python
# GetBotAliasesRequestPaginateTypeDef definition

class GetBotAliasesRequestPaginateTypeDef(TypedDict):
    botName: str,
    nameContains: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetBotChannelAssociationsRequestPaginateTypeDef

```python
# GetBotChannelAssociationsRequestPaginateTypeDef definition

class GetBotChannelAssociationsRequestPaginateTypeDef(TypedDict):
    botName: str,
    botAlias: str,
    nameContains: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetBotVersionsRequestPaginateTypeDef

```python
# GetBotVersionsRequestPaginateTypeDef definition

class GetBotVersionsRequestPaginateTypeDef(TypedDict):
    name: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetBotsRequestPaginateTypeDef

```python
# GetBotsRequestPaginateTypeDef definition

class GetBotsRequestPaginateTypeDef(TypedDict):
    nameContains: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetBuiltinIntentsRequestPaginateTypeDef

```python
# GetBuiltinIntentsRequestPaginateTypeDef definition

class GetBuiltinIntentsRequestPaginateTypeDef(TypedDict):
    locale: NotRequired[LocaleType],  # (1)
    signatureContains: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetBuiltinSlotTypesRequestPaginateTypeDef

```python
# GetBuiltinSlotTypesRequestPaginateTypeDef definition

class GetBuiltinSlotTypesRequestPaginateTypeDef(TypedDict):
    locale: NotRequired[LocaleType],  # (1)
    signatureContains: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetIntentVersionsRequestPaginateTypeDef

```python
# GetIntentVersionsRequestPaginateTypeDef definition

class GetIntentVersionsRequestPaginateTypeDef(TypedDict):
    name: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetIntentsRequestPaginateTypeDef

```python
# GetIntentsRequestPaginateTypeDef definition

class GetIntentsRequestPaginateTypeDef(TypedDict):
    nameContains: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetSlotTypeVersionsRequestPaginateTypeDef

```python
# GetSlotTypeVersionsRequestPaginateTypeDef definition

class GetSlotTypeVersionsRequestPaginateTypeDef(TypedDict):
    name: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetSlotTypesRequestPaginateTypeDef

```python
# GetSlotTypesRequestPaginateTypeDef definition

class GetSlotTypesRequestPaginateTypeDef(TypedDict):
    nameContains: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetIntentVersionsResponseTypeDef

```python
# GetIntentVersionsResponseTypeDef definition

class GetIntentVersionsResponseTypeDef(TypedDict):
    intents: list[IntentMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: IntentMetadataTypeDef](./type_defs.md#intentmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIntentsResponseTypeDef

```python
# GetIntentsResponseTypeDef definition

class GetIntentsResponseTypeDef(TypedDict):
    intents: list[IntentMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: IntentMetadataTypeDef](./type_defs.md#intentmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMigrationResponseTypeDef

```python
# GetMigrationResponseTypeDef definition

class GetMigrationResponseTypeDef(TypedDict):
    migrationId: str,
    v1BotName: str,
    v1BotVersion: str,
    v1BotLocale: LocaleType,  # (1)
    v2BotId: str,
    v2BotRole: str,
    migrationStatus: MigrationStatusType,  # (2)
    migrationStrategy: MigrationStrategyType,  # (3)
    migrationTimestamp: datetime,
    alerts: list[MigrationAlertTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
2. See [:material-code-brackets: MigrationStatusType](./literals.md#migrationstatustype) 
3. See [:material-code-brackets: MigrationStrategyType](./literals.md#migrationstrategytype) 
4. See [:material-code-braces: MigrationAlertTypeDef](./type_defs.md#migrationalerttypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMigrationsResponseTypeDef

```python
# GetMigrationsResponseTypeDef definition

class GetMigrationsResponseTypeDef(TypedDict):
    migrationSummaries: list[MigrationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MigrationSummaryTypeDef](./type_defs.md#migrationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSlotTypeVersionsResponseTypeDef

```python
# GetSlotTypeVersionsResponseTypeDef definition

class GetSlotTypeVersionsResponseTypeDef(TypedDict):
    slotTypes: list[SlotTypeMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SlotTypeMetadataTypeDef](./type_defs.md#slottypemetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSlotTypesResponseTypeDef

```python
# GetSlotTypesResponseTypeDef definition

class GetSlotTypesResponseTypeDef(TypedDict):
    slotTypes: list[SlotTypeMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SlotTypeMetadataTypeDef](./type_defs.md#slottypemetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: list[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartImportRequestRequestTypeDef

```python
# StartImportRequestRequestTypeDef definition

class StartImportRequestRequestTypeDef(TypedDict):
    payload: BlobTypeDef,
    resourceType: ResourceTypeType,  # (1)
    mergeStrategy: MergeStrategyType,  # (2)
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: MergeStrategyType](./literals.md#mergestrategytype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## StartImportResponseTypeDef

```python
# StartImportResponseTypeDef definition

class StartImportResponseTypeDef(TypedDict):
    name: str,
    resourceType: ResourceTypeType,  # (1)
    mergeStrategy: MergeStrategyType,  # (2)
    importId: str,
    importStatus: ImportStatusType,  # (3)
    tags: list[TagTypeDef],  # (4)
    createdDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: MergeStrategyType](./literals.md#mergestrategytype) 
3. See [:material-code-brackets: ImportStatusType](./literals.md#importstatustype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PromptOutputTypeDef

```python
# PromptOutputTypeDef definition

class PromptOutputTypeDef(TypedDict):
    messages: list[MessageTypeDef],  # (1)
    maxAttempts: int,
    responseCard: NotRequired[str],
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
## PromptTypeDef

```python
# PromptTypeDef definition

class PromptTypeDef(TypedDict):
    messages: Sequence[MessageTypeDef],  # (1)
    maxAttempts: int,
    responseCard: NotRequired[str],
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
## StatementOutputTypeDef

```python
# StatementOutputTypeDef definition

class StatementOutputTypeDef(TypedDict):
    messages: list[MessageTypeDef],  # (1)
    responseCard: NotRequired[str],
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
## StatementTypeDef

```python
# StatementTypeDef definition

class StatementTypeDef(TypedDict):
    messages: Sequence[MessageTypeDef],  # (1)
    responseCard: NotRequired[str],
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
## SlotDefaultValueSpecOutputTypeDef

```python
# SlotDefaultValueSpecOutputTypeDef definition

class SlotDefaultValueSpecOutputTypeDef(TypedDict):
    defaultValueList: list[SlotDefaultValueTypeDef],  # (1)
```

1. See [:material-code-braces: SlotDefaultValueTypeDef](./type_defs.md#slotdefaultvaluetypedef) 
## SlotDefaultValueSpecTypeDef

```python
# SlotDefaultValueSpecTypeDef definition

class SlotDefaultValueSpecTypeDef(TypedDict):
    defaultValueList: Sequence[SlotDefaultValueTypeDef],  # (1)
```

1. See [:material-code-braces: SlotDefaultValueTypeDef](./type_defs.md#slotdefaultvaluetypedef) 
## SlotTypeConfigurationTypeDef

```python
# SlotTypeConfigurationTypeDef definition

class SlotTypeConfigurationTypeDef(TypedDict):
    regexConfiguration: NotRequired[SlotTypeRegexConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: SlotTypeRegexConfigurationTypeDef](./type_defs.md#slottyperegexconfigurationtypedef) 
## UtteranceListTypeDef

```python
# UtteranceListTypeDef definition

class UtteranceListTypeDef(TypedDict):
    botVersion: NotRequired[str],
    utterances: NotRequired[list[UtteranceDataTypeDef]],  # (1)
```

1. See [:material-code-braces: UtteranceDataTypeDef](./type_defs.md#utterancedatatypedef) 
## PutBotAliasRequestRequestTypeDef

```python
# PutBotAliasRequestRequestTypeDef definition

class PutBotAliasRequestRequestTypeDef(TypedDict):
    name: str,
    botVersion: str,
    botName: str,
    description: NotRequired[str],
    checksum: NotRequired[str],
    conversationLogs: NotRequired[ConversationLogsRequestTypeDef],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ConversationLogsRequestTypeDef](./type_defs.md#conversationlogsrequesttypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## BotAliasMetadataTypeDef

```python
# BotAliasMetadataTypeDef definition

class BotAliasMetadataTypeDef(TypedDict):
    name: NotRequired[str],
    description: NotRequired[str],
    botVersion: NotRequired[str],
    botName: NotRequired[str],
    lastUpdatedDate: NotRequired[datetime],
    createdDate: NotRequired[datetime],
    checksum: NotRequired[str],
    conversationLogs: NotRequired[ConversationLogsResponseTypeDef],  # (1)
```

1. See [:material-code-braces: ConversationLogsResponseTypeDef](./type_defs.md#conversationlogsresponsetypedef) 
## GetBotAliasResponseTypeDef

```python
# GetBotAliasResponseTypeDef definition

class GetBotAliasResponseTypeDef(TypedDict):
    name: str,
    description: str,
    botVersion: str,
    botName: str,
    lastUpdatedDate: datetime,
    createdDate: datetime,
    checksum: str,
    conversationLogs: ConversationLogsResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConversationLogsResponseTypeDef](./type_defs.md#conversationlogsresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutBotAliasResponseTypeDef

```python
# PutBotAliasResponseTypeDef definition

class PutBotAliasResponseTypeDef(TypedDict):
    name: str,
    description: str,
    botVersion: str,
    botName: str,
    lastUpdatedDate: datetime,
    createdDate: datetime,
    checksum: str,
    conversationLogs: ConversationLogsResponseTypeDef,  # (1)
    tags: list[TagTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConversationLogsResponseTypeDef](./type_defs.md#conversationlogsresponsetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBotVersionResponseTypeDef

```python
# CreateBotVersionResponseTypeDef definition

class CreateBotVersionResponseTypeDef(TypedDict):
    name: str,
    description: str,
    intents: list[IntentTypeDef],  # (1)
    clarificationPrompt: PromptOutputTypeDef,  # (2)
    abortStatement: StatementOutputTypeDef,  # (3)
    status: StatusType,  # (4)
    failureReason: str,
    lastUpdatedDate: datetime,
    createdDate: datetime,
    idleSessionTTLInSeconds: int,
    voiceId: str,
    checksum: str,
    version: str,
    locale: LocaleType,  # (5)
    childDirected: bool,
    enableModelImprovements: bool,
    detectSentiment: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: IntentTypeDef](./type_defs.md#intenttypedef) 
2. See [:material-code-braces: PromptOutputTypeDef](./type_defs.md#promptoutputtypedef) 
3. See [:material-code-braces: StatementOutputTypeDef](./type_defs.md#statementoutputtypedef) 
4. See [:material-code-brackets: StatusType](./literals.md#statustype) 
5. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FollowUpPromptOutputTypeDef

```python
# FollowUpPromptOutputTypeDef definition

class FollowUpPromptOutputTypeDef(TypedDict):
    prompt: PromptOutputTypeDef,  # (1)
    rejectionStatement: StatementOutputTypeDef,  # (2)
```

1. See [:material-code-braces: PromptOutputTypeDef](./type_defs.md#promptoutputtypedef) 
2. See [:material-code-braces: StatementOutputTypeDef](./type_defs.md#statementoutputtypedef) 
## GetBotResponseTypeDef

```python
# GetBotResponseTypeDef definition

class GetBotResponseTypeDef(TypedDict):
    name: str,
    description: str,
    intents: list[IntentTypeDef],  # (1)
    enableModelImprovements: bool,
    nluIntentConfidenceThreshold: float,
    clarificationPrompt: PromptOutputTypeDef,  # (2)
    abortStatement: StatementOutputTypeDef,  # (3)
    status: StatusType,  # (4)
    failureReason: str,
    lastUpdatedDate: datetime,
    createdDate: datetime,
    idleSessionTTLInSeconds: int,
    voiceId: str,
    checksum: str,
    version: str,
    locale: LocaleType,  # (5)
    childDirected: bool,
    detectSentiment: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: IntentTypeDef](./type_defs.md#intenttypedef) 
2. See [:material-code-braces: PromptOutputTypeDef](./type_defs.md#promptoutputtypedef) 
3. See [:material-code-braces: StatementOutputTypeDef](./type_defs.md#statementoutputtypedef) 
4. See [:material-code-brackets: StatusType](./literals.md#statustype) 
5. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutBotResponseTypeDef

```python
# PutBotResponseTypeDef definition

class PutBotResponseTypeDef(TypedDict):
    name: str,
    description: str,
    intents: list[IntentTypeDef],  # (1)
    enableModelImprovements: bool,
    nluIntentConfidenceThreshold: float,
    clarificationPrompt: PromptOutputTypeDef,  # (2)
    abortStatement: StatementOutputTypeDef,  # (3)
    status: StatusType,  # (4)
    failureReason: str,
    lastUpdatedDate: datetime,
    createdDate: datetime,
    idleSessionTTLInSeconds: int,
    voiceId: str,
    checksum: str,
    version: str,
    locale: LocaleType,  # (5)
    childDirected: bool,
    createVersion: bool,
    detectSentiment: bool,
    tags: list[TagTypeDef],  # (6)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-braces: IntentTypeDef](./type_defs.md#intenttypedef) 
2. See [:material-code-braces: PromptOutputTypeDef](./type_defs.md#promptoutputtypedef) 
3. See [:material-code-braces: StatementOutputTypeDef](./type_defs.md#statementoutputtypedef) 
4. See [:material-code-brackets: StatusType](./literals.md#statustype) 
5. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutBotRequestRequestTypeDef

```python
# PutBotRequestRequestTypeDef definition

class PutBotRequestRequestTypeDef(TypedDict):
    name: str,
    locale: LocaleType,  # (1)
    childDirected: bool,
    description: NotRequired[str],
    intents: NotRequired[Sequence[IntentTypeDef]],  # (2)
    enableModelImprovements: NotRequired[bool],
    nluIntentConfidenceThreshold: NotRequired[float],
    clarificationPrompt: NotRequired[PromptTypeDef],  # (3)
    abortStatement: NotRequired[StatementTypeDef],  # (4)
    idleSessionTTLInSeconds: NotRequired[int],
    voiceId: NotRequired[str],
    checksum: NotRequired[str],
    processBehavior: NotRequired[ProcessBehaviorType],  # (5)
    detectSentiment: NotRequired[bool],
    createVersion: NotRequired[bool],
    tags: NotRequired[Sequence[TagTypeDef]],  # (6)
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
2. See [:material-code-braces: IntentTypeDef](./type_defs.md#intenttypedef) 
3. See [:material-code-braces: PromptTypeDef](./type_defs.md#prompttypedef) 
4. See [:material-code-braces: StatementTypeDef](./type_defs.md#statementtypedef) 
5. See [:material-code-brackets: ProcessBehaviorType](./literals.md#processbehaviortype) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## SlotOutputTypeDef

```python
# SlotOutputTypeDef definition

class SlotOutputTypeDef(TypedDict):
    name: str,
    slotConstraint: SlotConstraintType,  # (1)
    description: NotRequired[str],
    slotType: NotRequired[str],
    slotTypeVersion: NotRequired[str],
    valueElicitationPrompt: NotRequired[PromptOutputTypeDef],  # (2)
    priority: NotRequired[int],
    sampleUtterances: NotRequired[list[str]],
    responseCard: NotRequired[str],
    obfuscationSetting: NotRequired[ObfuscationSettingType],  # (3)
    defaultValueSpec: NotRequired[SlotDefaultValueSpecOutputTypeDef],  # (4)
```

1. See [:material-code-brackets: SlotConstraintType](./literals.md#slotconstrainttype) 
2. See [:material-code-braces: PromptOutputTypeDef](./type_defs.md#promptoutputtypedef) 
3. See [:material-code-brackets: ObfuscationSettingType](./literals.md#obfuscationsettingtype) 
4. See [:material-code-braces: SlotDefaultValueSpecOutputTypeDef](./type_defs.md#slotdefaultvaluespecoutputtypedef) 
## CreateSlotTypeVersionResponseTypeDef

```python
# CreateSlotTypeVersionResponseTypeDef definition

class CreateSlotTypeVersionResponseTypeDef(TypedDict):
    name: str,
    description: str,
    enumerationValues: list[EnumerationValueOutputTypeDef],  # (1)
    lastUpdatedDate: datetime,
    createdDate: datetime,
    version: str,
    checksum: str,
    valueSelectionStrategy: SlotValueSelectionStrategyType,  # (2)
    parentSlotTypeSignature: str,
    slotTypeConfigurations: list[SlotTypeConfigurationTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: EnumerationValueOutputTypeDef](./type_defs.md#enumerationvalueoutputtypedef) 
2. See [:material-code-brackets: SlotValueSelectionStrategyType](./literals.md#slotvalueselectionstrategytype) 
3. See [:material-code-braces: SlotTypeConfigurationTypeDef](./type_defs.md#slottypeconfigurationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSlotTypeResponseTypeDef

```python
# GetSlotTypeResponseTypeDef definition

class GetSlotTypeResponseTypeDef(TypedDict):
    name: str,
    description: str,
    enumerationValues: list[EnumerationValueOutputTypeDef],  # (1)
    lastUpdatedDate: datetime,
    createdDate: datetime,
    version: str,
    checksum: str,
    valueSelectionStrategy: SlotValueSelectionStrategyType,  # (2)
    parentSlotTypeSignature: str,
    slotTypeConfigurations: list[SlotTypeConfigurationTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: EnumerationValueOutputTypeDef](./type_defs.md#enumerationvalueoutputtypedef) 
2. See [:material-code-brackets: SlotValueSelectionStrategyType](./literals.md#slotvalueselectionstrategytype) 
3. See [:material-code-braces: SlotTypeConfigurationTypeDef](./type_defs.md#slottypeconfigurationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutSlotTypeRequestRequestTypeDef

```python
# PutSlotTypeRequestRequestTypeDef definition

class PutSlotTypeRequestRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    enumerationValues: NotRequired[Sequence[EnumerationValueUnionTypeDef]],  # (1)
    checksum: NotRequired[str],
    valueSelectionStrategy: NotRequired[SlotValueSelectionStrategyType],  # (2)
    createVersion: NotRequired[bool],
    parentSlotTypeSignature: NotRequired[str],
    slotTypeConfigurations: NotRequired[Sequence[SlotTypeConfigurationTypeDef]],  # (3)
```

1. See [:material-code-braces: EnumerationValueTypeDef](./type_defs.md#enumerationvaluetypedef) [:material-code-braces: EnumerationValueOutputTypeDef](./type_defs.md#enumerationvalueoutputtypedef) 
2. See [:material-code-brackets: SlotValueSelectionStrategyType](./literals.md#slotvalueselectionstrategytype) 
3. See [:material-code-braces: SlotTypeConfigurationTypeDef](./type_defs.md#slottypeconfigurationtypedef) 
## PutSlotTypeResponseTypeDef

```python
# PutSlotTypeResponseTypeDef definition

class PutSlotTypeResponseTypeDef(TypedDict):
    name: str,
    description: str,
    enumerationValues: list[EnumerationValueOutputTypeDef],  # (1)
    lastUpdatedDate: datetime,
    createdDate: datetime,
    version: str,
    checksum: str,
    valueSelectionStrategy: SlotValueSelectionStrategyType,  # (2)
    createVersion: bool,
    parentSlotTypeSignature: str,
    slotTypeConfigurations: list[SlotTypeConfigurationTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: EnumerationValueOutputTypeDef](./type_defs.md#enumerationvalueoutputtypedef) 
2. See [:material-code-brackets: SlotValueSelectionStrategyType](./literals.md#slotvalueselectionstrategytype) 
3. See [:material-code-braces: SlotTypeConfigurationTypeDef](./type_defs.md#slottypeconfigurationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUtterancesViewResponseTypeDef

```python
# GetUtterancesViewResponseTypeDef definition

class GetUtterancesViewResponseTypeDef(TypedDict):
    botName: str,
    utterances: list[UtteranceListTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UtteranceListTypeDef](./type_defs.md#utterancelisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBotAliasesResponseTypeDef

```python
# GetBotAliasesResponseTypeDef definition

class GetBotAliasesResponseTypeDef(TypedDict):
    BotAliases: list[BotAliasMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BotAliasMetadataTypeDef](./type_defs.md#botaliasmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FollowUpPromptTypeDef

```python
# FollowUpPromptTypeDef definition

class FollowUpPromptTypeDef(TypedDict):
    prompt: PromptUnionTypeDef,  # (1)
    rejectionStatement: StatementUnionTypeDef,  # (2)
```

1. See [:material-code-braces: PromptTypeDef](./type_defs.md#prompttypedef) [:material-code-braces: PromptOutputTypeDef](./type_defs.md#promptoutputtypedef) 
2. See [:material-code-braces: StatementTypeDef](./type_defs.md#statementtypedef) [:material-code-braces: StatementOutputTypeDef](./type_defs.md#statementoutputtypedef) 
## CreateIntentVersionResponseTypeDef

```python
# CreateIntentVersionResponseTypeDef definition

class CreateIntentVersionResponseTypeDef(TypedDict):
    name: str,
    description: str,
    slots: list[SlotOutputTypeDef],  # (1)
    sampleUtterances: list[str],
    confirmationPrompt: PromptOutputTypeDef,  # (2)
    rejectionStatement: StatementOutputTypeDef,  # (3)
    followUpPrompt: FollowUpPromptOutputTypeDef,  # (4)
    conclusionStatement: StatementOutputTypeDef,  # (3)
    dialogCodeHook: CodeHookTypeDef,  # (6)
    fulfillmentActivity: FulfillmentActivityTypeDef,  # (7)
    parentIntentSignature: str,
    lastUpdatedDate: datetime,
    createdDate: datetime,
    version: str,
    checksum: str,
    kendraConfiguration: KendraConfigurationTypeDef,  # (8)
    inputContexts: list[InputContextTypeDef],  # (9)
    outputContexts: list[OutputContextTypeDef],  # (10)
    ResponseMetadata: ResponseMetadataTypeDef,  # (11)
```

1. See [:material-code-braces: SlotOutputTypeDef](./type_defs.md#slotoutputtypedef) 
2. See [:material-code-braces: PromptOutputTypeDef](./type_defs.md#promptoutputtypedef) 
3. See [:material-code-braces: StatementOutputTypeDef](./type_defs.md#statementoutputtypedef) 
4. See [:material-code-braces: FollowUpPromptOutputTypeDef](./type_defs.md#followuppromptoutputtypedef) 
5. See [:material-code-braces: StatementOutputTypeDef](./type_defs.md#statementoutputtypedef) 
6. See [:material-code-braces: CodeHookTypeDef](./type_defs.md#codehooktypedef) 
7. See [:material-code-braces: FulfillmentActivityTypeDef](./type_defs.md#fulfillmentactivitytypedef) 
8. See [:material-code-braces: KendraConfigurationTypeDef](./type_defs.md#kendraconfigurationtypedef) 
9. See [:material-code-braces: InputContextTypeDef](./type_defs.md#inputcontexttypedef) 
10. See [:material-code-braces: OutputContextTypeDef](./type_defs.md#outputcontexttypedef) 
11. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIntentResponseTypeDef

```python
# GetIntentResponseTypeDef definition

class GetIntentResponseTypeDef(TypedDict):
    name: str,
    description: str,
    slots: list[SlotOutputTypeDef],  # (1)
    sampleUtterances: list[str],
    confirmationPrompt: PromptOutputTypeDef,  # (2)
    rejectionStatement: StatementOutputTypeDef,  # (3)
    followUpPrompt: FollowUpPromptOutputTypeDef,  # (4)
    conclusionStatement: StatementOutputTypeDef,  # (3)
    dialogCodeHook: CodeHookTypeDef,  # (6)
    fulfillmentActivity: FulfillmentActivityTypeDef,  # (7)
    parentIntentSignature: str,
    lastUpdatedDate: datetime,
    createdDate: datetime,
    version: str,
    checksum: str,
    kendraConfiguration: KendraConfigurationTypeDef,  # (8)
    inputContexts: list[InputContextTypeDef],  # (9)
    outputContexts: list[OutputContextTypeDef],  # (10)
    ResponseMetadata: ResponseMetadataTypeDef,  # (11)
```

1. See [:material-code-braces: SlotOutputTypeDef](./type_defs.md#slotoutputtypedef) 
2. See [:material-code-braces: PromptOutputTypeDef](./type_defs.md#promptoutputtypedef) 
3. See [:material-code-braces: StatementOutputTypeDef](./type_defs.md#statementoutputtypedef) 
4. See [:material-code-braces: FollowUpPromptOutputTypeDef](./type_defs.md#followuppromptoutputtypedef) 
5. See [:material-code-braces: StatementOutputTypeDef](./type_defs.md#statementoutputtypedef) 
6. See [:material-code-braces: CodeHookTypeDef](./type_defs.md#codehooktypedef) 
7. See [:material-code-braces: FulfillmentActivityTypeDef](./type_defs.md#fulfillmentactivitytypedef) 
8. See [:material-code-braces: KendraConfigurationTypeDef](./type_defs.md#kendraconfigurationtypedef) 
9. See [:material-code-braces: InputContextTypeDef](./type_defs.md#inputcontexttypedef) 
10. See [:material-code-braces: OutputContextTypeDef](./type_defs.md#outputcontexttypedef) 
11. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutIntentResponseTypeDef

```python
# PutIntentResponseTypeDef definition

class PutIntentResponseTypeDef(TypedDict):
    name: str,
    description: str,
    slots: list[SlotOutputTypeDef],  # (1)
    sampleUtterances: list[str],
    confirmationPrompt: PromptOutputTypeDef,  # (2)
    rejectionStatement: StatementOutputTypeDef,  # (3)
    followUpPrompt: FollowUpPromptOutputTypeDef,  # (4)
    conclusionStatement: StatementOutputTypeDef,  # (3)
    dialogCodeHook: CodeHookTypeDef,  # (6)
    fulfillmentActivity: FulfillmentActivityTypeDef,  # (7)
    parentIntentSignature: str,
    lastUpdatedDate: datetime,
    createdDate: datetime,
    version: str,
    checksum: str,
    createVersion: bool,
    kendraConfiguration: KendraConfigurationTypeDef,  # (8)
    inputContexts: list[InputContextTypeDef],  # (9)
    outputContexts: list[OutputContextTypeDef],  # (10)
    ResponseMetadata: ResponseMetadataTypeDef,  # (11)
```

1. See [:material-code-braces: SlotOutputTypeDef](./type_defs.md#slotoutputtypedef) 
2. See [:material-code-braces: PromptOutputTypeDef](./type_defs.md#promptoutputtypedef) 
3. See [:material-code-braces: StatementOutputTypeDef](./type_defs.md#statementoutputtypedef) 
4. See [:material-code-braces: FollowUpPromptOutputTypeDef](./type_defs.md#followuppromptoutputtypedef) 
5. See [:material-code-braces: StatementOutputTypeDef](./type_defs.md#statementoutputtypedef) 
6. See [:material-code-braces: CodeHookTypeDef](./type_defs.md#codehooktypedef) 
7. See [:material-code-braces: FulfillmentActivityTypeDef](./type_defs.md#fulfillmentactivitytypedef) 
8. See [:material-code-braces: KendraConfigurationTypeDef](./type_defs.md#kendraconfigurationtypedef) 
9. See [:material-code-braces: InputContextTypeDef](./type_defs.md#inputcontexttypedef) 
10. See [:material-code-braces: OutputContextTypeDef](./type_defs.md#outputcontexttypedef) 
11. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SlotTypeDef

```python
# SlotTypeDef definition

class SlotTypeDef(TypedDict):
    name: str,
    slotConstraint: SlotConstraintType,  # (1)
    description: NotRequired[str],
    slotType: NotRequired[str],
    slotTypeVersion: NotRequired[str],
    valueElicitationPrompt: NotRequired[PromptUnionTypeDef],  # (2)
    priority: NotRequired[int],
    sampleUtterances: NotRequired[Sequence[str]],
    responseCard: NotRequired[str],
    obfuscationSetting: NotRequired[ObfuscationSettingType],  # (3)
    defaultValueSpec: NotRequired[SlotDefaultValueSpecUnionTypeDef],  # (4)
```

1. See [:material-code-brackets: SlotConstraintType](./literals.md#slotconstrainttype) 
2. See [:material-code-braces: PromptTypeDef](./type_defs.md#prompttypedef) [:material-code-braces: PromptOutputTypeDef](./type_defs.md#promptoutputtypedef) 
3. See [:material-code-brackets: ObfuscationSettingType](./literals.md#obfuscationsettingtype) 
4. See [:material-code-braces: SlotDefaultValueSpecTypeDef](./type_defs.md#slotdefaultvaluespectypedef) [:material-code-braces: SlotDefaultValueSpecOutputTypeDef](./type_defs.md#slotdefaultvaluespecoutputtypedef) 
## PutIntentRequestRequestTypeDef

```python
# PutIntentRequestRequestTypeDef definition

class PutIntentRequestRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    slots: NotRequired[Sequence[SlotUnionTypeDef]],  # (1)
    sampleUtterances: NotRequired[Sequence[str]],
    confirmationPrompt: NotRequired[PromptTypeDef],  # (2)
    rejectionStatement: NotRequired[StatementTypeDef],  # (3)
    followUpPrompt: NotRequired[FollowUpPromptTypeDef],  # (4)
    conclusionStatement: NotRequired[StatementTypeDef],  # (3)
    dialogCodeHook: NotRequired[CodeHookTypeDef],  # (6)
    fulfillmentActivity: NotRequired[FulfillmentActivityTypeDef],  # (7)
    parentIntentSignature: NotRequired[str],
    checksum: NotRequired[str],
    createVersion: NotRequired[bool],
    kendraConfiguration: NotRequired[KendraConfigurationTypeDef],  # (8)
    inputContexts: NotRequired[Sequence[InputContextTypeDef]],  # (9)
    outputContexts: NotRequired[Sequence[OutputContextTypeDef]],  # (10)
```

1. See [:material-code-braces: SlotTypeDef](./type_defs.md#slottypedef) [:material-code-braces: SlotOutputTypeDef](./type_defs.md#slotoutputtypedef) 
2. See [:material-code-braces: PromptTypeDef](./type_defs.md#prompttypedef) 
3. See [:material-code-braces: StatementTypeDef](./type_defs.md#statementtypedef) 
4. See [:material-code-braces: FollowUpPromptTypeDef](./type_defs.md#followupprompttypedef) 
5. See [:material-code-braces: StatementTypeDef](./type_defs.md#statementtypedef) 
6. See [:material-code-braces: CodeHookTypeDef](./type_defs.md#codehooktypedef) 
7. See [:material-code-braces: FulfillmentActivityTypeDef](./type_defs.md#fulfillmentactivitytypedef) 
8. See [:material-code-braces: KendraConfigurationTypeDef](./type_defs.md#kendraconfigurationtypedef) 
9. See [:material-code-braces: InputContextTypeDef](./type_defs.md#inputcontexttypedef) 
10. See [:material-code-braces: OutputContextTypeDef](./type_defs.md#outputcontexttypedef) 