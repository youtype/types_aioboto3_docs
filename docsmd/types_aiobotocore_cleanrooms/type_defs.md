# Type definitions

> [Index](../README.md) > [CleanRoomsService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CleanRoomsService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
    type annotations stubs module [types-aiobotocore-cleanrooms](https://pypi.org/project/types-aiobotocore-cleanrooms/).



## AggregateColumnTypeDef

```python
# AggregateColumnTypeDef definition

class AggregateColumnTypeDef(TypedDict):
    columnNames: Sequence[str],
    function: AggregateFunctionNameType,  # (1)
```

1. See [:material-code-brackets: AggregateFunctionNameType](./literals.md#aggregatefunctionnametype) 
## AggregationConstraintTypeDef

```python
# AggregationConstraintTypeDef definition

class AggregationConstraintTypeDef(TypedDict):
    columnName: str,
    minimum: int,
    type: AggregationTypeType,  # (1)
```

1. See [:material-code-brackets: AggregationTypeType](./literals.md#aggregationtypetype) 
## AnalysisParameterTypeDef

```python
# AnalysisParameterTypeDef definition

class AnalysisParameterTypeDef(TypedDict):
    name: str,
    type: ParameterTypeType,  # (1)
    defaultValue: NotRequired[str],
```

1. See [:material-code-brackets: ParameterTypeType](./literals.md#parametertypetype) 
## AnalysisRuleListTypeDef

```python
# AnalysisRuleListTypeDef definition

class AnalysisRuleListTypeDef(TypedDict):
    joinColumns: Sequence[str],
    listColumns: Sequence[str],
    allowedJoinOperators: NotRequired[Sequence[JoinOperatorType]],  # (1)
```

1. See [:material-code-brackets: JoinOperatorType](./literals.md#joinoperatortype) 
## AnalysisSchemaTypeDef

```python
# AnalysisSchemaTypeDef definition

class AnalysisSchemaTypeDef(TypedDict):
    referencedTables: NotRequired[List[str]],
```

## AnalysisSourceTypeDef

```python
# AnalysisSourceTypeDef definition

class AnalysisSourceTypeDef(TypedDict):
    text: NotRequired[str],
```

## AnalysisTemplateSummaryTypeDef

```python
# AnalysisTemplateSummaryTypeDef definition

class AnalysisTemplateSummaryTypeDef(TypedDict):
    arn: str,
    createTime: datetime,
    id: str,
    name: str,
    updateTime: datetime,
    membershipArn: str,
    membershipId: str,
    collaborationArn: str,
    collaborationId: str,
    description: NotRequired[str],
```

## BatchGetCollaborationAnalysisTemplateErrorTypeDef

```python
# BatchGetCollaborationAnalysisTemplateErrorTypeDef definition

class BatchGetCollaborationAnalysisTemplateErrorTypeDef(TypedDict):
    arn: str,
    code: str,
    message: str,
```

## BatchGetCollaborationAnalysisTemplateInputRequestTypeDef

```python
# BatchGetCollaborationAnalysisTemplateInputRequestTypeDef definition

class BatchGetCollaborationAnalysisTemplateInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    analysisTemplateArns: Sequence[str],
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

## BatchGetSchemaErrorTypeDef

```python
# BatchGetSchemaErrorTypeDef definition

class BatchGetSchemaErrorTypeDef(TypedDict):
    name: str,
    code: str,
    message: str,
```

## BatchGetSchemaInputRequestTypeDef

```python
# BatchGetSchemaInputRequestTypeDef definition

class BatchGetSchemaInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    names: Sequence[str],
```

## CollaborationAnalysisTemplateSummaryTypeDef

```python
# CollaborationAnalysisTemplateSummaryTypeDef definition

class CollaborationAnalysisTemplateSummaryTypeDef(TypedDict):
    arn: str,
    createTime: datetime,
    id: str,
    name: str,
    updateTime: datetime,
    collaborationArn: str,
    collaborationId: str,
    creatorAccountId: str,
    description: NotRequired[str],
```

## CollaborationConfiguredAudienceModelAssociationSummaryTypeDef

```python
# CollaborationConfiguredAudienceModelAssociationSummaryTypeDef definition

class CollaborationConfiguredAudienceModelAssociationSummaryTypeDef(TypedDict):
    arn: str,
    createTime: datetime,
    id: str,
    name: str,
    updateTime: datetime,
    collaborationArn: str,
    collaborationId: str,
    creatorAccountId: str,
    description: NotRequired[str],
```

## CollaborationConfiguredAudienceModelAssociationTypeDef

```python
# CollaborationConfiguredAudienceModelAssociationTypeDef definition

class CollaborationConfiguredAudienceModelAssociationTypeDef(TypedDict):
    id: str,
    arn: str,
    collaborationId: str,
    collaborationArn: str,
    configuredAudienceModelArn: str,
    name: str,
    creatorAccountId: str,
    createTime: datetime,
    updateTime: datetime,
    description: NotRequired[str],
```

## CollaborationPrivacyBudgetTemplateSummaryTypeDef

```python
# CollaborationPrivacyBudgetTemplateSummaryTypeDef definition

class CollaborationPrivacyBudgetTemplateSummaryTypeDef(TypedDict):
    id: str,
    arn: str,
    collaborationId: str,
    collaborationArn: str,
    creatorAccountId: str,
    privacyBudgetType: PrivacyBudgetTypeType,  # (1)
    createTime: datetime,
    updateTime: datetime,
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
## CollaborationSummaryTypeDef

```python
# CollaborationSummaryTypeDef definition

class CollaborationSummaryTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    creatorAccountId: str,
    creatorDisplayName: str,
    createTime: datetime,
    updateTime: datetime,
    memberStatus: MemberStatusType,  # (1)
    membershipId: NotRequired[str],
    membershipArn: NotRequired[str],
```

1. See [:material-code-brackets: MemberStatusType](./literals.md#memberstatustype) 
## DataEncryptionMetadataTypeDef

```python
# DataEncryptionMetadataTypeDef definition

class DataEncryptionMetadataTypeDef(TypedDict):
    allowCleartext: bool,
    allowDuplicates: bool,
    allowJoinsOnColumnsWithDifferentNames: bool,
    preserveNulls: bool,
```

## ColumnTypeDef

```python
# ColumnTypeDef definition

class ColumnTypeDef(TypedDict):
    name: str,
    type: str,
```

## ConfiguredAudienceModelAssociationSummaryTypeDef

```python
# ConfiguredAudienceModelAssociationSummaryTypeDef definition

class ConfiguredAudienceModelAssociationSummaryTypeDef(TypedDict):
    membershipId: str,
    membershipArn: str,
    collaborationArn: str,
    collaborationId: str,
    createTime: datetime,
    updateTime: datetime,
    id: str,
    arn: str,
    name: str,
    configuredAudienceModelArn: str,
    description: NotRequired[str],
```

## ConfiguredAudienceModelAssociationTypeDef

```python
# ConfiguredAudienceModelAssociationTypeDef definition

class ConfiguredAudienceModelAssociationTypeDef(TypedDict):
    id: str,
    arn: str,
    configuredAudienceModelArn: str,
    membershipId: str,
    membershipArn: str,
    collaborationId: str,
    collaborationArn: str,
    name: str,
    manageResourcePolicies: bool,
    createTime: datetime,
    updateTime: datetime,
    description: NotRequired[str],
```

## ConfiguredTableAssociationSummaryTypeDef

```python
# ConfiguredTableAssociationSummaryTypeDef definition

class ConfiguredTableAssociationSummaryTypeDef(TypedDict):
    configuredTableId: str,
    membershipId: str,
    membershipArn: str,
    name: str,
    createTime: datetime,
    updateTime: datetime,
    id: str,
    arn: str,
```

## ConfiguredTableAssociationTypeDef

```python
# ConfiguredTableAssociationTypeDef definition

class ConfiguredTableAssociationTypeDef(TypedDict):
    arn: str,
    id: str,
    configuredTableId: str,
    configuredTableArn: str,
    membershipId: str,
    membershipArn: str,
    roleArn: str,
    name: str,
    createTime: datetime,
    updateTime: datetime,
    description: NotRequired[str],
```

## ConfiguredTableSummaryTypeDef

```python
# ConfiguredTableSummaryTypeDef definition

class ConfiguredTableSummaryTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    createTime: datetime,
    updateTime: datetime,
    analysisRuleTypes: List[ConfiguredTableAnalysisRuleTypeType],  # (1)
    analysisMethod: AnalysisMethodType,  # (2)
```

1. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
2. See [:material-code-brackets: AnalysisMethodType](./literals.md#analysismethodtype) 
## CreateConfiguredAudienceModelAssociationInputRequestTypeDef

```python
# CreateConfiguredAudienceModelAssociationInputRequestTypeDef definition

class CreateConfiguredAudienceModelAssociationInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    configuredAudienceModelArn: str,
    configuredAudienceModelAssociationName: str,
    manageResourcePolicies: bool,
    tags: NotRequired[Mapping[str, str]],
    description: NotRequired[str],
```

## CreateConfiguredTableAssociationInputRequestTypeDef

```python
# CreateConfiguredTableAssociationInputRequestTypeDef definition

class CreateConfiguredTableAssociationInputRequestTypeDef(TypedDict):
    name: str,
    membershipIdentifier: str,
    configuredTableIdentifier: str,
    roleArn: str,
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## DeleteAnalysisTemplateInputRequestTypeDef

```python
# DeleteAnalysisTemplateInputRequestTypeDef definition

class DeleteAnalysisTemplateInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    analysisTemplateIdentifier: str,
```

## DeleteCollaborationInputRequestTypeDef

```python
# DeleteCollaborationInputRequestTypeDef definition

class DeleteCollaborationInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
```

## DeleteConfiguredAudienceModelAssociationInputRequestTypeDef

```python
# DeleteConfiguredAudienceModelAssociationInputRequestTypeDef definition

class DeleteConfiguredAudienceModelAssociationInputRequestTypeDef(TypedDict):
    configuredAudienceModelAssociationIdentifier: str,
    membershipIdentifier: str,
```

## DeleteConfiguredTableAnalysisRuleInputRequestTypeDef

```python
# DeleteConfiguredTableAnalysisRuleInputRequestTypeDef definition

class DeleteConfiguredTableAnalysisRuleInputRequestTypeDef(TypedDict):
    configuredTableIdentifier: str,
    analysisRuleType: ConfiguredTableAnalysisRuleTypeType,  # (1)
```

1. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
## DeleteConfiguredTableAssociationInputRequestTypeDef

```python
# DeleteConfiguredTableAssociationInputRequestTypeDef definition

class DeleteConfiguredTableAssociationInputRequestTypeDef(TypedDict):
    configuredTableAssociationIdentifier: str,
    membershipIdentifier: str,
```

## DeleteConfiguredTableInputRequestTypeDef

```python
# DeleteConfiguredTableInputRequestTypeDef definition

class DeleteConfiguredTableInputRequestTypeDef(TypedDict):
    configuredTableIdentifier: str,
```

## DeleteMemberInputRequestTypeDef

```python
# DeleteMemberInputRequestTypeDef definition

class DeleteMemberInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    accountId: str,
```

## DeleteMembershipInputRequestTypeDef

```python
# DeleteMembershipInputRequestTypeDef definition

class DeleteMembershipInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
```

## DeletePrivacyBudgetTemplateInputRequestTypeDef

```python
# DeletePrivacyBudgetTemplateInputRequestTypeDef definition

class DeletePrivacyBudgetTemplateInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    privacyBudgetTemplateIdentifier: str,
```

## DifferentialPrivacyColumnTypeDef

```python
# DifferentialPrivacyColumnTypeDef definition

class DifferentialPrivacyColumnTypeDef(TypedDict):
    name: str,
```

## DifferentialPrivacySensitivityParametersTypeDef

```python
# DifferentialPrivacySensitivityParametersTypeDef definition

class DifferentialPrivacySensitivityParametersTypeDef(TypedDict):
    aggregationType: DifferentialPrivacyAggregationTypeType,  # (1)
    aggregationExpression: str,
    userContributionLimit: int,
    minColumnValue: NotRequired[float],
    maxColumnValue: NotRequired[float],
```

1. See [:material-code-brackets: DifferentialPrivacyAggregationTypeType](./literals.md#differentialprivacyaggregationtypetype) 
## DifferentialPrivacyPreviewAggregationTypeDef

```python
# DifferentialPrivacyPreviewAggregationTypeDef definition

class DifferentialPrivacyPreviewAggregationTypeDef(TypedDict):
    type: DifferentialPrivacyAggregationTypeType,  # (1)
    maxCount: int,
```

1. See [:material-code-brackets: DifferentialPrivacyAggregationTypeType](./literals.md#differentialprivacyaggregationtypetype) 
## DifferentialPrivacyPreviewParametersInputTypeDef

```python
# DifferentialPrivacyPreviewParametersInputTypeDef definition

class DifferentialPrivacyPreviewParametersInputTypeDef(TypedDict):
    epsilon: int,
    usersNoisePerQuery: int,
```

## DifferentialPrivacyPrivacyBudgetAggregationTypeDef

```python
# DifferentialPrivacyPrivacyBudgetAggregationTypeDef definition

class DifferentialPrivacyPrivacyBudgetAggregationTypeDef(TypedDict):
    type: DifferentialPrivacyAggregationTypeType,  # (1)
    maxCount: int,
    remainingCount: int,
```

1. See [:material-code-brackets: DifferentialPrivacyAggregationTypeType](./literals.md#differentialprivacyaggregationtypetype) 
## DifferentialPrivacyTemplateParametersInputTypeDef

```python
# DifferentialPrivacyTemplateParametersInputTypeDef definition

class DifferentialPrivacyTemplateParametersInputTypeDef(TypedDict):
    epsilon: int,
    usersNoisePerQuery: int,
```

## DifferentialPrivacyTemplateParametersOutputTypeDef

```python
# DifferentialPrivacyTemplateParametersOutputTypeDef definition

class DifferentialPrivacyTemplateParametersOutputTypeDef(TypedDict):
    epsilon: int,
    usersNoisePerQuery: int,
```

## DifferentialPrivacyTemplateUpdateParametersTypeDef

```python
# DifferentialPrivacyTemplateUpdateParametersTypeDef definition

class DifferentialPrivacyTemplateUpdateParametersTypeDef(TypedDict):
    epsilon: NotRequired[int],
    usersNoisePerQuery: NotRequired[int],
```

## GetAnalysisTemplateInputRequestTypeDef

```python
# GetAnalysisTemplateInputRequestTypeDef definition

class GetAnalysisTemplateInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    analysisTemplateIdentifier: str,
```

## GetCollaborationAnalysisTemplateInputRequestTypeDef

```python
# GetCollaborationAnalysisTemplateInputRequestTypeDef definition

class GetCollaborationAnalysisTemplateInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    analysisTemplateArn: str,
```

## GetCollaborationConfiguredAudienceModelAssociationInputRequestTypeDef

```python
# GetCollaborationConfiguredAudienceModelAssociationInputRequestTypeDef definition

class GetCollaborationConfiguredAudienceModelAssociationInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    configuredAudienceModelAssociationIdentifier: str,
```

## GetCollaborationInputRequestTypeDef

```python
# GetCollaborationInputRequestTypeDef definition

class GetCollaborationInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
```

## GetCollaborationPrivacyBudgetTemplateInputRequestTypeDef

```python
# GetCollaborationPrivacyBudgetTemplateInputRequestTypeDef definition

class GetCollaborationPrivacyBudgetTemplateInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    privacyBudgetTemplateIdentifier: str,
```

## GetConfiguredAudienceModelAssociationInputRequestTypeDef

```python
# GetConfiguredAudienceModelAssociationInputRequestTypeDef definition

class GetConfiguredAudienceModelAssociationInputRequestTypeDef(TypedDict):
    configuredAudienceModelAssociationIdentifier: str,
    membershipIdentifier: str,
```

## GetConfiguredTableAnalysisRuleInputRequestTypeDef

```python
# GetConfiguredTableAnalysisRuleInputRequestTypeDef definition

class GetConfiguredTableAnalysisRuleInputRequestTypeDef(TypedDict):
    configuredTableIdentifier: str,
    analysisRuleType: ConfiguredTableAnalysisRuleTypeType,  # (1)
```

1. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
## GetConfiguredTableAssociationInputRequestTypeDef

```python
# GetConfiguredTableAssociationInputRequestTypeDef definition

class GetConfiguredTableAssociationInputRequestTypeDef(TypedDict):
    configuredTableAssociationIdentifier: str,
    membershipIdentifier: str,
```

## GetConfiguredTableInputRequestTypeDef

```python
# GetConfiguredTableInputRequestTypeDef definition

class GetConfiguredTableInputRequestTypeDef(TypedDict):
    configuredTableIdentifier: str,
```

## GetMembershipInputRequestTypeDef

```python
# GetMembershipInputRequestTypeDef definition

class GetMembershipInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
```

## GetPrivacyBudgetTemplateInputRequestTypeDef

```python
# GetPrivacyBudgetTemplateInputRequestTypeDef definition

class GetPrivacyBudgetTemplateInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    privacyBudgetTemplateIdentifier: str,
```

## GetProtectedQueryInputRequestTypeDef

```python
# GetProtectedQueryInputRequestTypeDef definition

class GetProtectedQueryInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    protectedQueryIdentifier: str,
```

## GetSchemaAnalysisRuleInputRequestTypeDef

```python
# GetSchemaAnalysisRuleInputRequestTypeDef definition

class GetSchemaAnalysisRuleInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    name: str,
    type: AnalysisRuleTypeType,  # (1)
```

1. See [:material-code-brackets: AnalysisRuleTypeType](./literals.md#analysisruletypetype) 
## GetSchemaInputRequestTypeDef

```python
# GetSchemaInputRequestTypeDef definition

class GetSchemaInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    name: str,
```

## GlueTableReferenceTypeDef

```python
# GlueTableReferenceTypeDef definition

class GlueTableReferenceTypeDef(TypedDict):
    tableName: str,
    databaseName: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAnalysisTemplatesInputRequestTypeDef

```python
# ListAnalysisTemplatesInputRequestTypeDef definition

class ListAnalysisTemplatesInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListCollaborationAnalysisTemplatesInputRequestTypeDef

```python
# ListCollaborationAnalysisTemplatesInputRequestTypeDef definition

class ListCollaborationAnalysisTemplatesInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListCollaborationConfiguredAudienceModelAssociationsInputRequestTypeDef

```python
# ListCollaborationConfiguredAudienceModelAssociationsInputRequestTypeDef definition

class ListCollaborationConfiguredAudienceModelAssociationsInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListCollaborationPrivacyBudgetTemplatesInputRequestTypeDef

```python
# ListCollaborationPrivacyBudgetTemplatesInputRequestTypeDef definition

class ListCollaborationPrivacyBudgetTemplatesInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListCollaborationPrivacyBudgetsInputRequestTypeDef

```python
# ListCollaborationPrivacyBudgetsInputRequestTypeDef definition

class ListCollaborationPrivacyBudgetsInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    privacyBudgetType: PrivacyBudgetTypeType,  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
## ListCollaborationsInputRequestTypeDef

```python
# ListCollaborationsInputRequestTypeDef definition

class ListCollaborationsInputRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    memberStatus: NotRequired[FilterableMemberStatusType],  # (1)
```

1. See [:material-code-brackets: FilterableMemberStatusType](./literals.md#filterablememberstatustype) 
## ListConfiguredAudienceModelAssociationsInputRequestTypeDef

```python
# ListConfiguredAudienceModelAssociationsInputRequestTypeDef definition

class ListConfiguredAudienceModelAssociationsInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListConfiguredTableAssociationsInputRequestTypeDef

```python
# ListConfiguredTableAssociationsInputRequestTypeDef definition

class ListConfiguredTableAssociationsInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListConfiguredTablesInputRequestTypeDef

```python
# ListConfiguredTablesInputRequestTypeDef definition

class ListConfiguredTablesInputRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListMembersInputRequestTypeDef

```python
# ListMembersInputRequestTypeDef definition

class ListMembersInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListMembershipsInputRequestTypeDef

```python
# ListMembershipsInputRequestTypeDef definition

class ListMembershipsInputRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    status: NotRequired[MembershipStatusType],  # (1)
```

1. See [:material-code-brackets: MembershipStatusType](./literals.md#membershipstatustype) 
## ListPrivacyBudgetTemplatesInputRequestTypeDef

```python
# ListPrivacyBudgetTemplatesInputRequestTypeDef definition

class ListPrivacyBudgetTemplatesInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## PrivacyBudgetTemplateSummaryTypeDef

```python
# PrivacyBudgetTemplateSummaryTypeDef definition

class PrivacyBudgetTemplateSummaryTypeDef(TypedDict):
    id: str,
    arn: str,
    membershipId: str,
    membershipArn: str,
    collaborationId: str,
    collaborationArn: str,
    privacyBudgetType: PrivacyBudgetTypeType,  # (1)
    createTime: datetime,
    updateTime: datetime,
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
## ListPrivacyBudgetsInputRequestTypeDef

```python
# ListPrivacyBudgetsInputRequestTypeDef definition

class ListPrivacyBudgetsInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    privacyBudgetType: PrivacyBudgetTypeType,  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
## ListProtectedQueriesInputRequestTypeDef

```python
# ListProtectedQueriesInputRequestTypeDef definition

class ListProtectedQueriesInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    status: NotRequired[ProtectedQueryStatusType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: ProtectedQueryStatusType](./literals.md#protectedquerystatustype) 
## ProtectedQuerySummaryTypeDef

```python
# ProtectedQuerySummaryTypeDef definition

class ProtectedQuerySummaryTypeDef(TypedDict):
    id: str,
    membershipId: str,
    membershipArn: str,
    createTime: datetime,
    status: ProtectedQueryStatusType,  # (1)
```

1. See [:material-code-brackets: ProtectedQueryStatusType](./literals.md#protectedquerystatustype) 
## ListSchemasInputRequestTypeDef

```python
# ListSchemasInputRequestTypeDef definition

class ListSchemasInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    schemaType: NotRequired[SchemaTypeType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: SchemaTypeType](./literals.md#schematypetype) 
## SchemaSummaryTypeDef

```python
# SchemaSummaryTypeDef definition

class SchemaSummaryTypeDef(TypedDict):
    name: str,
    type: SchemaTypeType,  # (1)
    creatorAccountId: str,
    createTime: datetime,
    updateTime: datetime,
    collaborationId: str,
    collaborationArn: str,
    analysisRuleTypes: List[AnalysisRuleTypeType],  # (2)
    analysisMethod: NotRequired[AnalysisMethodType],  # (3)
```

1. See [:material-code-brackets: SchemaTypeType](./literals.md#schematypetype) 
2. See [:material-code-brackets: AnalysisRuleTypeType](./literals.md#analysisruletypetype) 
3. See [:material-code-brackets: AnalysisMethodType](./literals.md#analysismethodtype) 
## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
```

## MembershipQueryComputePaymentConfigTypeDef

```python
# MembershipQueryComputePaymentConfigTypeDef definition

class MembershipQueryComputePaymentConfigTypeDef(TypedDict):
    isResponsible: bool,
```

## ProtectedQueryS3OutputConfigurationTypeDef

```python
# ProtectedQueryS3OutputConfigurationTypeDef definition

class ProtectedQueryS3OutputConfigurationTypeDef(TypedDict):
    resultFormat: ResultFormatType,  # (1)
    bucket: str,
    keyPrefix: NotRequired[str],
```

1. See [:material-code-brackets: ResultFormatType](./literals.md#resultformattype) 
## QueryComputePaymentConfigTypeDef

```python
# QueryComputePaymentConfigTypeDef definition

class QueryComputePaymentConfigTypeDef(TypedDict):
    isResponsible: bool,
```

## ProtectedQueryErrorTypeDef

```python
# ProtectedQueryErrorTypeDef definition

class ProtectedQueryErrorTypeDef(TypedDict):
    message: str,
    code: str,
```

## ProtectedQueryS3OutputTypeDef

```python
# ProtectedQueryS3OutputTypeDef definition

class ProtectedQueryS3OutputTypeDef(TypedDict):
    location: str,
```

## ProtectedQuerySingleMemberOutputTypeDef

```python
# ProtectedQuerySingleMemberOutputTypeDef definition

class ProtectedQuerySingleMemberOutputTypeDef(TypedDict):
    accountId: str,
```

## ProtectedQuerySQLParametersTypeDef

```python
# ProtectedQuerySQLParametersTypeDef definition

class ProtectedQuerySQLParametersTypeDef(TypedDict):
    queryString: NotRequired[str],
    analysisTemplateArn: NotRequired[str],
    parameters: NotRequired[Dict[str, str]],
```

## ProtectedQueryStatisticsTypeDef

```python
# ProtectedQueryStatisticsTypeDef definition

class ProtectedQueryStatisticsTypeDef(TypedDict):
    totalDurationInMillis: NotRequired[int],
```

## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateAnalysisTemplateInputRequestTypeDef

```python
# UpdateAnalysisTemplateInputRequestTypeDef definition

class UpdateAnalysisTemplateInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    analysisTemplateIdentifier: str,
    description: NotRequired[str],
```

## UpdateCollaborationInputRequestTypeDef

```python
# UpdateCollaborationInputRequestTypeDef definition

class UpdateCollaborationInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    name: NotRequired[str],
    description: NotRequired[str],
```

## UpdateConfiguredAudienceModelAssociationInputRequestTypeDef

```python
# UpdateConfiguredAudienceModelAssociationInputRequestTypeDef definition

class UpdateConfiguredAudienceModelAssociationInputRequestTypeDef(TypedDict):
    configuredAudienceModelAssociationIdentifier: str,
    membershipIdentifier: str,
    description: NotRequired[str],
    name: NotRequired[str],
```

## UpdateConfiguredTableAssociationInputRequestTypeDef

```python
# UpdateConfiguredTableAssociationInputRequestTypeDef definition

class UpdateConfiguredTableAssociationInputRequestTypeDef(TypedDict):
    configuredTableAssociationIdentifier: str,
    membershipIdentifier: str,
    description: NotRequired[str],
    roleArn: NotRequired[str],
```

## UpdateConfiguredTableInputRequestTypeDef

```python
# UpdateConfiguredTableInputRequestTypeDef definition

class UpdateConfiguredTableInputRequestTypeDef(TypedDict):
    configuredTableIdentifier: str,
    name: NotRequired[str],
    description: NotRequired[str],
```

## UpdateProtectedQueryInputRequestTypeDef

```python
# UpdateProtectedQueryInputRequestTypeDef definition

class UpdateProtectedQueryInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    protectedQueryIdentifier: str,
    targetStatus: TargetProtectedQueryStatusType,  # (1)
```

1. See [:material-code-brackets: TargetProtectedQueryStatusType](./literals.md#targetprotectedquerystatustype) 
## AnalysisRuleAggregationTypeDef

```python
# AnalysisRuleAggregationTypeDef definition

class AnalysisRuleAggregationTypeDef(TypedDict):
    aggregateColumns: Sequence[AggregateColumnTypeDef],  # (1)
    joinColumns: Sequence[str],
    dimensionColumns: Sequence[str],
    scalarFunctions: Sequence[ScalarFunctionsType],  # (4)
    outputConstraints: Sequence[AggregationConstraintTypeDef],  # (5)
    joinRequired: NotRequired[JoinRequiredOptionType],  # (2)
    allowedJoinOperators: NotRequired[Sequence[JoinOperatorType]],  # (3)
```

1. See [:material-code-braces: AggregateColumnTypeDef](./type_defs.md#aggregatecolumntypedef) 
2. See [:material-code-brackets: JoinRequiredOptionType](./literals.md#joinrequiredoptiontype) 
3. See [:material-code-brackets: JoinOperatorType](./literals.md#joinoperatortype) 
4. See [:material-code-brackets: ScalarFunctionsType](./literals.md#scalarfunctionstype) 
5. See [:material-code-braces: AggregationConstraintTypeDef](./type_defs.md#aggregationconstrainttypedef) 
## AnalysisTemplateTypeDef

```python
# AnalysisTemplateTypeDef definition

class AnalysisTemplateTypeDef(TypedDict):
    id: str,
    arn: str,
    collaborationId: str,
    collaborationArn: str,
    membershipId: str,
    membershipArn: str,
    name: str,
    createTime: datetime,
    updateTime: datetime,
    schema: AnalysisSchemaTypeDef,  # (1)
    format: AnalysisFormatType,  # (2)
    source: AnalysisSourceTypeDef,  # (3)
    description: NotRequired[str],
    analysisParameters: NotRequired[List[AnalysisParameterTypeDef]],  # (4)
```

1. See [:material-code-braces: AnalysisSchemaTypeDef](./type_defs.md#analysisschematypedef) 
2. See [:material-code-brackets: AnalysisFormatType](./literals.md#analysisformattype) 
3. See [:material-code-braces: AnalysisSourceTypeDef](./type_defs.md#analysissourcetypedef) 
4. See [:material-code-braces: AnalysisParameterTypeDef](./type_defs.md#analysisparametertypedef) 
## CollaborationAnalysisTemplateTypeDef

```python
# CollaborationAnalysisTemplateTypeDef definition

class CollaborationAnalysisTemplateTypeDef(TypedDict):
    id: str,
    arn: str,
    collaborationId: str,
    collaborationArn: str,
    creatorAccountId: str,
    name: str,
    createTime: datetime,
    updateTime: datetime,
    schema: AnalysisSchemaTypeDef,  # (1)
    format: AnalysisFormatType,  # (2)
    source: AnalysisSourceTypeDef,  # (3)
    description: NotRequired[str],
    analysisParameters: NotRequired[List[AnalysisParameterTypeDef]],  # (4)
```

1. See [:material-code-braces: AnalysisSchemaTypeDef](./type_defs.md#analysisschematypedef) 
2. See [:material-code-brackets: AnalysisFormatType](./literals.md#analysisformattype) 
3. See [:material-code-braces: AnalysisSourceTypeDef](./type_defs.md#analysissourcetypedef) 
4. See [:material-code-braces: AnalysisParameterTypeDef](./type_defs.md#analysisparametertypedef) 
## CreateAnalysisTemplateInputRequestTypeDef

```python
# CreateAnalysisTemplateInputRequestTypeDef definition

class CreateAnalysisTemplateInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    name: str,
    format: AnalysisFormatType,  # (1)
    source: AnalysisSourceTypeDef,  # (2)
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    analysisParameters: NotRequired[Sequence[AnalysisParameterTypeDef]],  # (3)
```

1. See [:material-code-brackets: AnalysisFormatType](./literals.md#analysisformattype) 
2. See [:material-code-braces: AnalysisSourceTypeDef](./type_defs.md#analysissourcetypedef) 
3. See [:material-code-braces: AnalysisParameterTypeDef](./type_defs.md#analysisparametertypedef) 
## ListAnalysisTemplatesOutputTypeDef

```python
# ListAnalysisTemplatesOutputTypeDef definition

class ListAnalysisTemplatesOutputTypeDef(TypedDict):
    nextToken: str,
    analysisTemplateSummaries: List[AnalysisTemplateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalysisTemplateSummaryTypeDef](./type_defs.md#analysistemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCollaborationAnalysisTemplatesOutputTypeDef

```python
# ListCollaborationAnalysisTemplatesOutputTypeDef definition

class ListCollaborationAnalysisTemplatesOutputTypeDef(TypedDict):
    nextToken: str,
    collaborationAnalysisTemplateSummaries: List[CollaborationAnalysisTemplateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CollaborationAnalysisTemplateSummaryTypeDef](./type_defs.md#collaborationanalysistemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCollaborationConfiguredAudienceModelAssociationsOutputTypeDef

```python
# ListCollaborationConfiguredAudienceModelAssociationsOutputTypeDef definition

class ListCollaborationConfiguredAudienceModelAssociationsOutputTypeDef(TypedDict):
    collaborationConfiguredAudienceModelAssociationSummaries: List[CollaborationConfiguredAudienceModelAssociationSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CollaborationConfiguredAudienceModelAssociationSummaryTypeDef](./type_defs.md#collaborationconfiguredaudiencemodelassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCollaborationConfiguredAudienceModelAssociationOutputTypeDef

```python
# GetCollaborationConfiguredAudienceModelAssociationOutputTypeDef definition

class GetCollaborationConfiguredAudienceModelAssociationOutputTypeDef(TypedDict):
    collaborationConfiguredAudienceModelAssociation: CollaborationConfiguredAudienceModelAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CollaborationConfiguredAudienceModelAssociationTypeDef](./type_defs.md#collaborationconfiguredaudiencemodelassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCollaborationPrivacyBudgetTemplatesOutputTypeDef

```python
# ListCollaborationPrivacyBudgetTemplatesOutputTypeDef definition

class ListCollaborationPrivacyBudgetTemplatesOutputTypeDef(TypedDict):
    nextToken: str,
    collaborationPrivacyBudgetTemplateSummaries: List[CollaborationPrivacyBudgetTemplateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CollaborationPrivacyBudgetTemplateSummaryTypeDef](./type_defs.md#collaborationprivacybudgettemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCollaborationsOutputTypeDef

```python
# ListCollaborationsOutputTypeDef definition

class ListCollaborationsOutputTypeDef(TypedDict):
    nextToken: str,
    collaborationList: List[CollaborationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CollaborationSummaryTypeDef](./type_defs.md#collaborationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CollaborationTypeDef

```python
# CollaborationTypeDef definition

class CollaborationTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    creatorAccountId: str,
    creatorDisplayName: str,
    createTime: datetime,
    updateTime: datetime,
    memberStatus: MemberStatusType,  # (1)
    queryLogStatus: CollaborationQueryLogStatusType,  # (3)
    description: NotRequired[str],
    membershipId: NotRequired[str],
    membershipArn: NotRequired[str],
    dataEncryptionMetadata: NotRequired[DataEncryptionMetadataTypeDef],  # (2)
```

1. See [:material-code-brackets: MemberStatusType](./literals.md#memberstatustype) 
2. See [:material-code-braces: DataEncryptionMetadataTypeDef](./type_defs.md#dataencryptionmetadatatypedef) 
3. See [:material-code-brackets: CollaborationQueryLogStatusType](./literals.md#collaborationquerylogstatustype) 
## SchemaTypeDef

```python
# SchemaTypeDef definition

class SchemaTypeDef(TypedDict):
    columns: List[ColumnTypeDef],  # (1)
    partitionKeys: List[ColumnTypeDef],  # (1)
    analysisRuleTypes: List[AnalysisRuleTypeType],  # (3)
    creatorAccountId: str,
    name: str,
    collaborationId: str,
    collaborationArn: str,
    description: str,
    createTime: datetime,
    updateTime: datetime,
    type: SchemaTypeType,  # (5)
    analysisMethod: NotRequired[AnalysisMethodType],  # (4)
```

1. See [:material-code-braces: ColumnTypeDef](./type_defs.md#columntypedef) 
2. See [:material-code-braces: ColumnTypeDef](./type_defs.md#columntypedef) 
3. See [:material-code-brackets: AnalysisRuleTypeType](./literals.md#analysisruletypetype) 
4. See [:material-code-brackets: AnalysisMethodType](./literals.md#analysismethodtype) 
5. See [:material-code-brackets: SchemaTypeType](./literals.md#schematypetype) 
## ListConfiguredAudienceModelAssociationsOutputTypeDef

```python
# ListConfiguredAudienceModelAssociationsOutputTypeDef definition

class ListConfiguredAudienceModelAssociationsOutputTypeDef(TypedDict):
    configuredAudienceModelAssociationSummaries: List[ConfiguredAudienceModelAssociationSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredAudienceModelAssociationSummaryTypeDef](./type_defs.md#configuredaudiencemodelassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfiguredAudienceModelAssociationOutputTypeDef

```python
# CreateConfiguredAudienceModelAssociationOutputTypeDef definition

class CreateConfiguredAudienceModelAssociationOutputTypeDef(TypedDict):
    configuredAudienceModelAssociation: ConfiguredAudienceModelAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredAudienceModelAssociationTypeDef](./type_defs.md#configuredaudiencemodelassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConfiguredAudienceModelAssociationOutputTypeDef

```python
# GetConfiguredAudienceModelAssociationOutputTypeDef definition

class GetConfiguredAudienceModelAssociationOutputTypeDef(TypedDict):
    configuredAudienceModelAssociation: ConfiguredAudienceModelAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredAudienceModelAssociationTypeDef](./type_defs.md#configuredaudiencemodelassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConfiguredAudienceModelAssociationOutputTypeDef

```python
# UpdateConfiguredAudienceModelAssociationOutputTypeDef definition

class UpdateConfiguredAudienceModelAssociationOutputTypeDef(TypedDict):
    configuredAudienceModelAssociation: ConfiguredAudienceModelAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredAudienceModelAssociationTypeDef](./type_defs.md#configuredaudiencemodelassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfiguredTableAssociationsOutputTypeDef

```python
# ListConfiguredTableAssociationsOutputTypeDef definition

class ListConfiguredTableAssociationsOutputTypeDef(TypedDict):
    configuredTableAssociationSummaries: List[ConfiguredTableAssociationSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableAssociationSummaryTypeDef](./type_defs.md#configuredtableassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfiguredTableAssociationOutputTypeDef

```python
# CreateConfiguredTableAssociationOutputTypeDef definition

class CreateConfiguredTableAssociationOutputTypeDef(TypedDict):
    configuredTableAssociation: ConfiguredTableAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableAssociationTypeDef](./type_defs.md#configuredtableassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConfiguredTableAssociationOutputTypeDef

```python
# GetConfiguredTableAssociationOutputTypeDef definition

class GetConfiguredTableAssociationOutputTypeDef(TypedDict):
    configuredTableAssociation: ConfiguredTableAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableAssociationTypeDef](./type_defs.md#configuredtableassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConfiguredTableAssociationOutputTypeDef

```python
# UpdateConfiguredTableAssociationOutputTypeDef definition

class UpdateConfiguredTableAssociationOutputTypeDef(TypedDict):
    configuredTableAssociation: ConfiguredTableAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableAssociationTypeDef](./type_defs.md#configuredtableassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfiguredTablesOutputTypeDef

```python
# ListConfiguredTablesOutputTypeDef definition

class ListConfiguredTablesOutputTypeDef(TypedDict):
    configuredTableSummaries: List[ConfiguredTableSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableSummaryTypeDef](./type_defs.md#configuredtablesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DifferentialPrivacyConfigurationTypeDef

```python
# DifferentialPrivacyConfigurationTypeDef definition

class DifferentialPrivacyConfigurationTypeDef(TypedDict):
    columns: Sequence[DifferentialPrivacyColumnTypeDef],  # (1)
```

1. See [:material-code-braces: DifferentialPrivacyColumnTypeDef](./type_defs.md#differentialprivacycolumntypedef) 
## DifferentialPrivacyParametersTypeDef

```python
# DifferentialPrivacyParametersTypeDef definition

class DifferentialPrivacyParametersTypeDef(TypedDict):
    sensitivityParameters: List[DifferentialPrivacySensitivityParametersTypeDef],  # (1)
```

1. See [:material-code-braces: DifferentialPrivacySensitivityParametersTypeDef](./type_defs.md#differentialprivacysensitivityparameterstypedef) 
## DifferentialPrivacyPrivacyImpactTypeDef

```python
# DifferentialPrivacyPrivacyImpactTypeDef definition

class DifferentialPrivacyPrivacyImpactTypeDef(TypedDict):
    aggregations: List[DifferentialPrivacyPreviewAggregationTypeDef],  # (1)
```

1. See [:material-code-braces: DifferentialPrivacyPreviewAggregationTypeDef](./type_defs.md#differentialprivacypreviewaggregationtypedef) 
## PreviewPrivacyImpactParametersInputTypeDef

```python
# PreviewPrivacyImpactParametersInputTypeDef definition

class PreviewPrivacyImpactParametersInputTypeDef(TypedDict):
    differentialPrivacy: NotRequired[DifferentialPrivacyPreviewParametersInputTypeDef],  # (1)
```

1. See [:material-code-braces: DifferentialPrivacyPreviewParametersInputTypeDef](./type_defs.md#differentialprivacypreviewparametersinputtypedef) 
## DifferentialPrivacyPrivacyBudgetTypeDef

```python
# DifferentialPrivacyPrivacyBudgetTypeDef definition

class DifferentialPrivacyPrivacyBudgetTypeDef(TypedDict):
    aggregations: List[DifferentialPrivacyPrivacyBudgetAggregationTypeDef],  # (1)
    epsilon: int,
```

1. See [:material-code-braces: DifferentialPrivacyPrivacyBudgetAggregationTypeDef](./type_defs.md#differentialprivacyprivacybudgetaggregationtypedef) 
## PrivacyBudgetTemplateParametersInputTypeDef

```python
# PrivacyBudgetTemplateParametersInputTypeDef definition

class PrivacyBudgetTemplateParametersInputTypeDef(TypedDict):
    differentialPrivacy: NotRequired[DifferentialPrivacyTemplateParametersInputTypeDef],  # (1)
```

1. See [:material-code-braces: DifferentialPrivacyTemplateParametersInputTypeDef](./type_defs.md#differentialprivacytemplateparametersinputtypedef) 
## PrivacyBudgetTemplateParametersOutputTypeDef

```python
# PrivacyBudgetTemplateParametersOutputTypeDef definition

class PrivacyBudgetTemplateParametersOutputTypeDef(TypedDict):
    differentialPrivacy: NotRequired[DifferentialPrivacyTemplateParametersOutputTypeDef],  # (1)
```

1. See [:material-code-braces: DifferentialPrivacyTemplateParametersOutputTypeDef](./type_defs.md#differentialprivacytemplateparametersoutputtypedef) 
## PrivacyBudgetTemplateUpdateParametersTypeDef

```python
# PrivacyBudgetTemplateUpdateParametersTypeDef definition

class PrivacyBudgetTemplateUpdateParametersTypeDef(TypedDict):
    differentialPrivacy: NotRequired[DifferentialPrivacyTemplateUpdateParametersTypeDef],  # (1)
```

1. See [:material-code-braces: DifferentialPrivacyTemplateUpdateParametersTypeDef](./type_defs.md#differentialprivacytemplateupdateparameterstypedef) 
## TableReferenceTypeDef

```python
# TableReferenceTypeDef definition

class TableReferenceTypeDef(TypedDict):
    glue: NotRequired[GlueTableReferenceTypeDef],  # (1)
```

1. See [:material-code-braces: GlueTableReferenceTypeDef](./type_defs.md#gluetablereferencetypedef) 
## ListAnalysisTemplatesInputListAnalysisTemplatesPaginateTypeDef

```python
# ListAnalysisTemplatesInputListAnalysisTemplatesPaginateTypeDef definition

class ListAnalysisTemplatesInputListAnalysisTemplatesPaginateTypeDef(TypedDict):
    membershipIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCollaborationAnalysisTemplatesInputListCollaborationAnalysisTemplatesPaginateTypeDef

```python
# ListCollaborationAnalysisTemplatesInputListCollaborationAnalysisTemplatesPaginateTypeDef definition

class ListCollaborationAnalysisTemplatesInputListCollaborationAnalysisTemplatesPaginateTypeDef(TypedDict):
    collaborationIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCollaborationConfiguredAudienceModelAssociationsInputListCollaborationConfiguredAudienceModelAssociationsPaginateTypeDef

```python
# ListCollaborationConfiguredAudienceModelAssociationsInputListCollaborationConfiguredAudienceModelAssociationsPaginateTypeDef definition

class ListCollaborationConfiguredAudienceModelAssociationsInputListCollaborationConfiguredAudienceModelAssociationsPaginateTypeDef(TypedDict):
    collaborationIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCollaborationPrivacyBudgetTemplatesInputListCollaborationPrivacyBudgetTemplatesPaginateTypeDef

```python
# ListCollaborationPrivacyBudgetTemplatesInputListCollaborationPrivacyBudgetTemplatesPaginateTypeDef definition

class ListCollaborationPrivacyBudgetTemplatesInputListCollaborationPrivacyBudgetTemplatesPaginateTypeDef(TypedDict):
    collaborationIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCollaborationPrivacyBudgetsInputListCollaborationPrivacyBudgetsPaginateTypeDef

```python
# ListCollaborationPrivacyBudgetsInputListCollaborationPrivacyBudgetsPaginateTypeDef definition

class ListCollaborationPrivacyBudgetsInputListCollaborationPrivacyBudgetsPaginateTypeDef(TypedDict):
    collaborationIdentifier: str,
    privacyBudgetType: PrivacyBudgetTypeType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCollaborationsInputListCollaborationsPaginateTypeDef

```python
# ListCollaborationsInputListCollaborationsPaginateTypeDef definition

class ListCollaborationsInputListCollaborationsPaginateTypeDef(TypedDict):
    memberStatus: NotRequired[FilterableMemberStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: FilterableMemberStatusType](./literals.md#filterablememberstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConfiguredAudienceModelAssociationsInputListConfiguredAudienceModelAssociationsPaginateTypeDef

```python
# ListConfiguredAudienceModelAssociationsInputListConfiguredAudienceModelAssociationsPaginateTypeDef definition

class ListConfiguredAudienceModelAssociationsInputListConfiguredAudienceModelAssociationsPaginateTypeDef(TypedDict):
    membershipIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef

```python
# ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef definition

class ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef(TypedDict):
    membershipIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef

```python
# ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef definition

class ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMembersInputListMembersPaginateTypeDef

```python
# ListMembersInputListMembersPaginateTypeDef definition

class ListMembersInputListMembersPaginateTypeDef(TypedDict):
    collaborationIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMembershipsInputListMembershipsPaginateTypeDef

```python
# ListMembershipsInputListMembershipsPaginateTypeDef definition

class ListMembershipsInputListMembershipsPaginateTypeDef(TypedDict):
    status: NotRequired[MembershipStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: MembershipStatusType](./literals.md#membershipstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPrivacyBudgetTemplatesInputListPrivacyBudgetTemplatesPaginateTypeDef

```python
# ListPrivacyBudgetTemplatesInputListPrivacyBudgetTemplatesPaginateTypeDef definition

class ListPrivacyBudgetTemplatesInputListPrivacyBudgetTemplatesPaginateTypeDef(TypedDict):
    membershipIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPrivacyBudgetsInputListPrivacyBudgetsPaginateTypeDef

```python
# ListPrivacyBudgetsInputListPrivacyBudgetsPaginateTypeDef definition

class ListPrivacyBudgetsInputListPrivacyBudgetsPaginateTypeDef(TypedDict):
    membershipIdentifier: str,
    privacyBudgetType: PrivacyBudgetTypeType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef

```python
# ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef definition

class ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef(TypedDict):
    membershipIdentifier: str,
    status: NotRequired[ProtectedQueryStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ProtectedQueryStatusType](./literals.md#protectedquerystatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSchemasInputListSchemasPaginateTypeDef

```python
# ListSchemasInputListSchemasPaginateTypeDef definition

class ListSchemasInputListSchemasPaginateTypeDef(TypedDict):
    collaborationIdentifier: str,
    schemaType: NotRequired[SchemaTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SchemaTypeType](./literals.md#schematypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPrivacyBudgetTemplatesOutputTypeDef

```python
# ListPrivacyBudgetTemplatesOutputTypeDef definition

class ListPrivacyBudgetTemplatesOutputTypeDef(TypedDict):
    nextToken: str,
    privacyBudgetTemplateSummaries: List[PrivacyBudgetTemplateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PrivacyBudgetTemplateSummaryTypeDef](./type_defs.md#privacybudgettemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProtectedQueriesOutputTypeDef

```python
# ListProtectedQueriesOutputTypeDef definition

class ListProtectedQueriesOutputTypeDef(TypedDict):
    nextToken: str,
    protectedQueries: List[ProtectedQuerySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProtectedQuerySummaryTypeDef](./type_defs.md#protectedquerysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSchemasOutputTypeDef

```python
# ListSchemasOutputTypeDef definition

class ListSchemasOutputTypeDef(TypedDict):
    schemaSummaries: List[SchemaSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaSummaryTypeDef](./type_defs.md#schemasummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MembershipPaymentConfigurationTypeDef

```python
# MembershipPaymentConfigurationTypeDef definition

class MembershipPaymentConfigurationTypeDef(TypedDict):
    queryCompute: MembershipQueryComputePaymentConfigTypeDef,  # (1)
```

1. See [:material-code-braces: MembershipQueryComputePaymentConfigTypeDef](./type_defs.md#membershipquerycomputepaymentconfigtypedef) 
## MembershipProtectedQueryOutputConfigurationTypeDef

```python
# MembershipProtectedQueryOutputConfigurationTypeDef definition

class MembershipProtectedQueryOutputConfigurationTypeDef(TypedDict):
    s3: NotRequired[ProtectedQueryS3OutputConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ProtectedQueryS3OutputConfigurationTypeDef](./type_defs.md#protectedquerys3outputconfigurationtypedef) 
## ProtectedQueryOutputConfigurationTypeDef

```python
# ProtectedQueryOutputConfigurationTypeDef definition

class ProtectedQueryOutputConfigurationTypeDef(TypedDict):
    s3: NotRequired[ProtectedQueryS3OutputConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ProtectedQueryS3OutputConfigurationTypeDef](./type_defs.md#protectedquerys3outputconfigurationtypedef) 
## PaymentConfigurationTypeDef

```python
# PaymentConfigurationTypeDef definition

class PaymentConfigurationTypeDef(TypedDict):
    queryCompute: QueryComputePaymentConfigTypeDef,  # (1)
```

1. See [:material-code-braces: QueryComputePaymentConfigTypeDef](./type_defs.md#querycomputepaymentconfigtypedef) 
## ProtectedQueryOutputTypeDef

```python
# ProtectedQueryOutputTypeDef definition

class ProtectedQueryOutputTypeDef(TypedDict):
    s3: NotRequired[ProtectedQueryS3OutputTypeDef],  # (1)
    memberList: NotRequired[List[ProtectedQuerySingleMemberOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: ProtectedQueryS3OutputTypeDef](./type_defs.md#protectedquerys3outputtypedef) 
2. See [:material-code-braces: ProtectedQuerySingleMemberOutputTypeDef](./type_defs.md#protectedquerysinglememberoutputtypedef) 
## CreateAnalysisTemplateOutputTypeDef

```python
# CreateAnalysisTemplateOutputTypeDef definition

class CreateAnalysisTemplateOutputTypeDef(TypedDict):
    analysisTemplate: AnalysisTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalysisTemplateTypeDef](./type_defs.md#analysistemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAnalysisTemplateOutputTypeDef

```python
# GetAnalysisTemplateOutputTypeDef definition

class GetAnalysisTemplateOutputTypeDef(TypedDict):
    analysisTemplate: AnalysisTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalysisTemplateTypeDef](./type_defs.md#analysistemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAnalysisTemplateOutputTypeDef

```python
# UpdateAnalysisTemplateOutputTypeDef definition

class UpdateAnalysisTemplateOutputTypeDef(TypedDict):
    analysisTemplate: AnalysisTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalysisTemplateTypeDef](./type_defs.md#analysistemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetCollaborationAnalysisTemplateOutputTypeDef

```python
# BatchGetCollaborationAnalysisTemplateOutputTypeDef definition

class BatchGetCollaborationAnalysisTemplateOutputTypeDef(TypedDict):
    collaborationAnalysisTemplates: List[CollaborationAnalysisTemplateTypeDef],  # (1)
    errors: List[BatchGetCollaborationAnalysisTemplateErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CollaborationAnalysisTemplateTypeDef](./type_defs.md#collaborationanalysistemplatetypedef) 
2. See [:material-code-braces: BatchGetCollaborationAnalysisTemplateErrorTypeDef](./type_defs.md#batchgetcollaborationanalysistemplateerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCollaborationAnalysisTemplateOutputTypeDef

```python
# GetCollaborationAnalysisTemplateOutputTypeDef definition

class GetCollaborationAnalysisTemplateOutputTypeDef(TypedDict):
    collaborationAnalysisTemplate: CollaborationAnalysisTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CollaborationAnalysisTemplateTypeDef](./type_defs.md#collaborationanalysistemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCollaborationOutputTypeDef

```python
# CreateCollaborationOutputTypeDef definition

class CreateCollaborationOutputTypeDef(TypedDict):
    collaboration: CollaborationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CollaborationTypeDef](./type_defs.md#collaborationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCollaborationOutputTypeDef

```python
# GetCollaborationOutputTypeDef definition

class GetCollaborationOutputTypeDef(TypedDict):
    collaboration: CollaborationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CollaborationTypeDef](./type_defs.md#collaborationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCollaborationOutputTypeDef

```python
# UpdateCollaborationOutputTypeDef definition

class UpdateCollaborationOutputTypeDef(TypedDict):
    collaboration: CollaborationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CollaborationTypeDef](./type_defs.md#collaborationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetSchemaOutputTypeDef

```python
# BatchGetSchemaOutputTypeDef definition

class BatchGetSchemaOutputTypeDef(TypedDict):
    schemas: List[SchemaTypeDef],  # (1)
    errors: List[BatchGetSchemaErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SchemaTypeDef](./type_defs.md#schematypedef) 
2. See [:material-code-braces: BatchGetSchemaErrorTypeDef](./type_defs.md#batchgetschemaerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSchemaOutputTypeDef

```python
# GetSchemaOutputTypeDef definition

class GetSchemaOutputTypeDef(TypedDict):
    schema: SchemaTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaTypeDef](./type_defs.md#schematypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AnalysisRuleCustomTypeDef

```python
# AnalysisRuleCustomTypeDef definition

class AnalysisRuleCustomTypeDef(TypedDict):
    allowedAnalyses: Sequence[str],
    allowedAnalysisProviders: NotRequired[Sequence[str]],
    differentialPrivacy: NotRequired[DifferentialPrivacyConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: DifferentialPrivacyConfigurationTypeDef](./type_defs.md#differentialprivacyconfigurationtypedef) 
## PrivacyImpactTypeDef

```python
# PrivacyImpactTypeDef definition

class PrivacyImpactTypeDef(TypedDict):
    differentialPrivacy: NotRequired[DifferentialPrivacyPrivacyImpactTypeDef],  # (1)
```

1. See [:material-code-braces: DifferentialPrivacyPrivacyImpactTypeDef](./type_defs.md#differentialprivacyprivacyimpacttypedef) 
## PreviewPrivacyImpactInputRequestTypeDef

```python
# PreviewPrivacyImpactInputRequestTypeDef definition

class PreviewPrivacyImpactInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    parameters: PreviewPrivacyImpactParametersInputTypeDef,  # (1)
```

1. See [:material-code-braces: PreviewPrivacyImpactParametersInputTypeDef](./type_defs.md#previewprivacyimpactparametersinputtypedef) 
## PrivacyBudgetTypeDef

```python
# PrivacyBudgetTypeDef definition

class PrivacyBudgetTypeDef(TypedDict):
    differentialPrivacy: NotRequired[DifferentialPrivacyPrivacyBudgetTypeDef],  # (1)
```

1. See [:material-code-braces: DifferentialPrivacyPrivacyBudgetTypeDef](./type_defs.md#differentialprivacyprivacybudgettypedef) 
## CreatePrivacyBudgetTemplateInputRequestTypeDef

```python
# CreatePrivacyBudgetTemplateInputRequestTypeDef definition

class CreatePrivacyBudgetTemplateInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    autoRefresh: PrivacyBudgetTemplateAutoRefreshType,  # (1)
    privacyBudgetType: PrivacyBudgetTypeType,  # (2)
    parameters: PrivacyBudgetTemplateParametersInputTypeDef,  # (3)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: PrivacyBudgetTemplateAutoRefreshType](./literals.md#privacybudgettemplateautorefreshtype) 
2. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
3. See [:material-code-braces: PrivacyBudgetTemplateParametersInputTypeDef](./type_defs.md#privacybudgettemplateparametersinputtypedef) 
## CollaborationPrivacyBudgetTemplateTypeDef

```python
# CollaborationPrivacyBudgetTemplateTypeDef definition

class CollaborationPrivacyBudgetTemplateTypeDef(TypedDict):
    id: str,
    arn: str,
    collaborationId: str,
    collaborationArn: str,
    creatorAccountId: str,
    createTime: datetime,
    updateTime: datetime,
    privacyBudgetType: PrivacyBudgetTypeType,  # (1)
    autoRefresh: PrivacyBudgetTemplateAutoRefreshType,  # (2)
    parameters: PrivacyBudgetTemplateParametersOutputTypeDef,  # (3)
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
2. See [:material-code-brackets: PrivacyBudgetTemplateAutoRefreshType](./literals.md#privacybudgettemplateautorefreshtype) 
3. See [:material-code-braces: PrivacyBudgetTemplateParametersOutputTypeDef](./type_defs.md#privacybudgettemplateparametersoutputtypedef) 
## PrivacyBudgetTemplateTypeDef

```python
# PrivacyBudgetTemplateTypeDef definition

class PrivacyBudgetTemplateTypeDef(TypedDict):
    id: str,
    arn: str,
    membershipId: str,
    membershipArn: str,
    collaborationId: str,
    collaborationArn: str,
    createTime: datetime,
    updateTime: datetime,
    privacyBudgetType: PrivacyBudgetTypeType,  # (1)
    autoRefresh: PrivacyBudgetTemplateAutoRefreshType,  # (2)
    parameters: PrivacyBudgetTemplateParametersOutputTypeDef,  # (3)
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
2. See [:material-code-brackets: PrivacyBudgetTemplateAutoRefreshType](./literals.md#privacybudgettemplateautorefreshtype) 
3. See [:material-code-braces: PrivacyBudgetTemplateParametersOutputTypeDef](./type_defs.md#privacybudgettemplateparametersoutputtypedef) 
## UpdatePrivacyBudgetTemplateInputRequestTypeDef

```python
# UpdatePrivacyBudgetTemplateInputRequestTypeDef definition

class UpdatePrivacyBudgetTemplateInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    privacyBudgetTemplateIdentifier: str,
    privacyBudgetType: PrivacyBudgetTypeType,  # (1)
    parameters: NotRequired[PrivacyBudgetTemplateUpdateParametersTypeDef],  # (2)
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
2. See [:material-code-braces: PrivacyBudgetTemplateUpdateParametersTypeDef](./type_defs.md#privacybudgettemplateupdateparameterstypedef) 
## ConfiguredTableTypeDef

```python
# ConfiguredTableTypeDef definition

class ConfiguredTableTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    tableReference: TableReferenceTypeDef,  # (1)
    createTime: datetime,
    updateTime: datetime,
    analysisRuleTypes: List[ConfiguredTableAnalysisRuleTypeType],  # (2)
    analysisMethod: AnalysisMethodType,  # (3)
    allowedColumns: List[str],
    description: NotRequired[str],
```

1. See [:material-code-braces: TableReferenceTypeDef](./type_defs.md#tablereferencetypedef) 
2. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
3. See [:material-code-brackets: AnalysisMethodType](./literals.md#analysismethodtype) 
## CreateConfiguredTableInputRequestTypeDef

```python
# CreateConfiguredTableInputRequestTypeDef definition

class CreateConfiguredTableInputRequestTypeDef(TypedDict):
    name: str,
    tableReference: TableReferenceTypeDef,  # (1)
    allowedColumns: Sequence[str],
    analysisMethod: AnalysisMethodType,  # (2)
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: TableReferenceTypeDef](./type_defs.md#tablereferencetypedef) 
2. See [:material-code-brackets: AnalysisMethodType](./literals.md#analysismethodtype) 
## MembershipSummaryTypeDef

```python
# MembershipSummaryTypeDef definition

class MembershipSummaryTypeDef(TypedDict):
    id: str,
    arn: str,
    collaborationArn: str,
    collaborationId: str,
    collaborationCreatorAccountId: str,
    collaborationCreatorDisplayName: str,
    collaborationName: str,
    createTime: datetime,
    updateTime: datetime,
    status: MembershipStatusType,  # (1)
    memberAbilities: List[MemberAbilityType],  # (2)
    paymentConfiguration: MembershipPaymentConfigurationTypeDef,  # (3)
```

1. See [:material-code-brackets: MembershipStatusType](./literals.md#membershipstatustype) 
2. See [:material-code-brackets: MemberAbilityType](./literals.md#memberabilitytype) 
3. See [:material-code-braces: MembershipPaymentConfigurationTypeDef](./type_defs.md#membershippaymentconfigurationtypedef) 
## MembershipProtectedQueryResultConfigurationTypeDef

```python
# MembershipProtectedQueryResultConfigurationTypeDef definition

class MembershipProtectedQueryResultConfigurationTypeDef(TypedDict):
    outputConfiguration: MembershipProtectedQueryOutputConfigurationTypeDef,  # (1)
    roleArn: NotRequired[str],
```

1. See [:material-code-braces: MembershipProtectedQueryOutputConfigurationTypeDef](./type_defs.md#membershipprotectedqueryoutputconfigurationtypedef) 
## ProtectedQueryResultConfigurationTypeDef

```python
# ProtectedQueryResultConfigurationTypeDef definition

class ProtectedQueryResultConfigurationTypeDef(TypedDict):
    outputConfiguration: ProtectedQueryOutputConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: ProtectedQueryOutputConfigurationTypeDef](./type_defs.md#protectedqueryoutputconfigurationtypedef) 
## MemberSpecificationTypeDef

```python
# MemberSpecificationTypeDef definition

class MemberSpecificationTypeDef(TypedDict):
    accountId: str,
    memberAbilities: Sequence[MemberAbilityType],  # (1)
    displayName: str,
    paymentConfiguration: NotRequired[PaymentConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: MemberAbilityType](./literals.md#memberabilitytype) 
2. See [:material-code-braces: PaymentConfigurationTypeDef](./type_defs.md#paymentconfigurationtypedef) 
## MemberSummaryTypeDef

```python
# MemberSummaryTypeDef definition

class MemberSummaryTypeDef(TypedDict):
    accountId: str,
    status: MemberStatusType,  # (1)
    displayName: str,
    abilities: List[MemberAbilityType],  # (2)
    createTime: datetime,
    updateTime: datetime,
    paymentConfiguration: PaymentConfigurationTypeDef,  # (3)
    membershipId: NotRequired[str],
    membershipArn: NotRequired[str],
```

1. See [:material-code-brackets: MemberStatusType](./literals.md#memberstatustype) 
2. See [:material-code-brackets: MemberAbilityType](./literals.md#memberabilitytype) 
3. See [:material-code-braces: PaymentConfigurationTypeDef](./type_defs.md#paymentconfigurationtypedef) 
## ProtectedQueryResultTypeDef

```python
# ProtectedQueryResultTypeDef definition

class ProtectedQueryResultTypeDef(TypedDict):
    output: ProtectedQueryOutputTypeDef,  # (1)
```

1. See [:material-code-braces: ProtectedQueryOutputTypeDef](./type_defs.md#protectedqueryoutputtypedef) 
## AnalysisRulePolicyV1TypeDef

```python
# AnalysisRulePolicyV1TypeDef definition

class AnalysisRulePolicyV1TypeDef(TypedDict):
    list: NotRequired[AnalysisRuleListTypeDef],  # (1)
    aggregation: NotRequired[AnalysisRuleAggregationTypeDef],  # (2)
    custom: NotRequired[AnalysisRuleCustomTypeDef],  # (3)
```

1. See [:material-code-braces: AnalysisRuleListTypeDef](./type_defs.md#analysisrulelisttypedef) 
2. See [:material-code-braces: AnalysisRuleAggregationTypeDef](./type_defs.md#analysisruleaggregationtypedef) 
3. See [:material-code-braces: AnalysisRuleCustomTypeDef](./type_defs.md#analysisrulecustomtypedef) 
## ConfiguredTableAnalysisRulePolicyV1TypeDef

```python
# ConfiguredTableAnalysisRulePolicyV1TypeDef definition

class ConfiguredTableAnalysisRulePolicyV1TypeDef(TypedDict):
    list: NotRequired[AnalysisRuleListTypeDef],  # (1)
    aggregation: NotRequired[AnalysisRuleAggregationTypeDef],  # (2)
    custom: NotRequired[AnalysisRuleCustomTypeDef],  # (3)
```

1. See [:material-code-braces: AnalysisRuleListTypeDef](./type_defs.md#analysisrulelisttypedef) 
2. See [:material-code-braces: AnalysisRuleAggregationTypeDef](./type_defs.md#analysisruleaggregationtypedef) 
3. See [:material-code-braces: AnalysisRuleCustomTypeDef](./type_defs.md#analysisrulecustomtypedef) 
## PreviewPrivacyImpactOutputTypeDef

```python
# PreviewPrivacyImpactOutputTypeDef definition

class PreviewPrivacyImpactOutputTypeDef(TypedDict):
    privacyImpact: PrivacyImpactTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PrivacyImpactTypeDef](./type_defs.md#privacyimpacttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CollaborationPrivacyBudgetSummaryTypeDef

```python
# CollaborationPrivacyBudgetSummaryTypeDef definition

class CollaborationPrivacyBudgetSummaryTypeDef(TypedDict):
    id: str,
    privacyBudgetTemplateId: str,
    privacyBudgetTemplateArn: str,
    collaborationId: str,
    collaborationArn: str,
    creatorAccountId: str,
    type: PrivacyBudgetTypeType,  # (1)
    createTime: datetime,
    updateTime: datetime,
    budget: PrivacyBudgetTypeDef,  # (2)
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
2. See [:material-code-braces: PrivacyBudgetTypeDef](./type_defs.md#privacybudgettypedef) 
## PrivacyBudgetSummaryTypeDef

```python
# PrivacyBudgetSummaryTypeDef definition

class PrivacyBudgetSummaryTypeDef(TypedDict):
    id: str,
    privacyBudgetTemplateId: str,
    privacyBudgetTemplateArn: str,
    membershipId: str,
    membershipArn: str,
    collaborationId: str,
    collaborationArn: str,
    type: PrivacyBudgetTypeType,  # (1)
    createTime: datetime,
    updateTime: datetime,
    budget: PrivacyBudgetTypeDef,  # (2)
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
2. See [:material-code-braces: PrivacyBudgetTypeDef](./type_defs.md#privacybudgettypedef) 
## GetCollaborationPrivacyBudgetTemplateOutputTypeDef

```python
# GetCollaborationPrivacyBudgetTemplateOutputTypeDef definition

class GetCollaborationPrivacyBudgetTemplateOutputTypeDef(TypedDict):
    collaborationPrivacyBudgetTemplate: CollaborationPrivacyBudgetTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CollaborationPrivacyBudgetTemplateTypeDef](./type_defs.md#collaborationprivacybudgettemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePrivacyBudgetTemplateOutputTypeDef

```python
# CreatePrivacyBudgetTemplateOutputTypeDef definition

class CreatePrivacyBudgetTemplateOutputTypeDef(TypedDict):
    privacyBudgetTemplate: PrivacyBudgetTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PrivacyBudgetTemplateTypeDef](./type_defs.md#privacybudgettemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPrivacyBudgetTemplateOutputTypeDef

```python
# GetPrivacyBudgetTemplateOutputTypeDef definition

class GetPrivacyBudgetTemplateOutputTypeDef(TypedDict):
    privacyBudgetTemplate: PrivacyBudgetTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PrivacyBudgetTemplateTypeDef](./type_defs.md#privacybudgettemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePrivacyBudgetTemplateOutputTypeDef

```python
# UpdatePrivacyBudgetTemplateOutputTypeDef definition

class UpdatePrivacyBudgetTemplateOutputTypeDef(TypedDict):
    privacyBudgetTemplate: PrivacyBudgetTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PrivacyBudgetTemplateTypeDef](./type_defs.md#privacybudgettemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfiguredTableOutputTypeDef

```python
# CreateConfiguredTableOutputTypeDef definition

class CreateConfiguredTableOutputTypeDef(TypedDict):
    configuredTable: ConfiguredTableTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableTypeDef](./type_defs.md#configuredtabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConfiguredTableOutputTypeDef

```python
# GetConfiguredTableOutputTypeDef definition

class GetConfiguredTableOutputTypeDef(TypedDict):
    configuredTable: ConfiguredTableTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableTypeDef](./type_defs.md#configuredtabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConfiguredTableOutputTypeDef

```python
# UpdateConfiguredTableOutputTypeDef definition

class UpdateConfiguredTableOutputTypeDef(TypedDict):
    configuredTable: ConfiguredTableTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableTypeDef](./type_defs.md#configuredtabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMembershipsOutputTypeDef

```python
# ListMembershipsOutputTypeDef definition

class ListMembershipsOutputTypeDef(TypedDict):
    nextToken: str,
    membershipSummaries: List[MembershipSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MembershipSummaryTypeDef](./type_defs.md#membershipsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMembershipInputRequestTypeDef

```python
# CreateMembershipInputRequestTypeDef definition

class CreateMembershipInputRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    queryLogStatus: MembershipQueryLogStatusType,  # (1)
    tags: NotRequired[Mapping[str, str]],
    defaultResultConfiguration: NotRequired[MembershipProtectedQueryResultConfigurationTypeDef],  # (2)
    paymentConfiguration: NotRequired[MembershipPaymentConfigurationTypeDef],  # (3)
```

1. See [:material-code-brackets: MembershipQueryLogStatusType](./literals.md#membershipquerylogstatustype) 
2. See [:material-code-braces: MembershipProtectedQueryResultConfigurationTypeDef](./type_defs.md#membershipprotectedqueryresultconfigurationtypedef) 
3. See [:material-code-braces: MembershipPaymentConfigurationTypeDef](./type_defs.md#membershippaymentconfigurationtypedef) 
## MembershipTypeDef

```python
# MembershipTypeDef definition

class MembershipTypeDef(TypedDict):
    id: str,
    arn: str,
    collaborationArn: str,
    collaborationId: str,
    collaborationCreatorAccountId: str,
    collaborationCreatorDisplayName: str,
    collaborationName: str,
    createTime: datetime,
    updateTime: datetime,
    status: MembershipStatusType,  # (1)
    memberAbilities: List[MemberAbilityType],  # (2)
    queryLogStatus: MembershipQueryLogStatusType,  # (3)
    paymentConfiguration: MembershipPaymentConfigurationTypeDef,  # (5)
    defaultResultConfiguration: NotRequired[MembershipProtectedQueryResultConfigurationTypeDef],  # (4)
```

1. See [:material-code-brackets: MembershipStatusType](./literals.md#membershipstatustype) 
2. See [:material-code-brackets: MemberAbilityType](./literals.md#memberabilitytype) 
3. See [:material-code-brackets: MembershipQueryLogStatusType](./literals.md#membershipquerylogstatustype) 
4. See [:material-code-braces: MembershipProtectedQueryResultConfigurationTypeDef](./type_defs.md#membershipprotectedqueryresultconfigurationtypedef) 
5. See [:material-code-braces: MembershipPaymentConfigurationTypeDef](./type_defs.md#membershippaymentconfigurationtypedef) 
## UpdateMembershipInputRequestTypeDef

```python
# UpdateMembershipInputRequestTypeDef definition

class UpdateMembershipInputRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    queryLogStatus: NotRequired[MembershipQueryLogStatusType],  # (1)
    defaultResultConfiguration: NotRequired[MembershipProtectedQueryResultConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: MembershipQueryLogStatusType](./literals.md#membershipquerylogstatustype) 
2. See [:material-code-braces: MembershipProtectedQueryResultConfigurationTypeDef](./type_defs.md#membershipprotectedqueryresultconfigurationtypedef) 
## StartProtectedQueryInputRequestTypeDef

```python
# StartProtectedQueryInputRequestTypeDef definition

class StartProtectedQueryInputRequestTypeDef(TypedDict):
    type: ProtectedQueryTypeType,  # (1)
    membershipIdentifier: str,
    sqlParameters: ProtectedQuerySQLParametersTypeDef,  # (2)
    resultConfiguration: NotRequired[ProtectedQueryResultConfigurationTypeDef],  # (3)
```

1. See [:material-code-brackets: ProtectedQueryTypeType](./literals.md#protectedquerytypetype) 
2. See [:material-code-braces: ProtectedQuerySQLParametersTypeDef](./type_defs.md#protectedquerysqlparameterstypedef) 
3. See [:material-code-braces: ProtectedQueryResultConfigurationTypeDef](./type_defs.md#protectedqueryresultconfigurationtypedef) 
## CreateCollaborationInputRequestTypeDef

```python
# CreateCollaborationInputRequestTypeDef definition

class CreateCollaborationInputRequestTypeDef(TypedDict):
    members: Sequence[MemberSpecificationTypeDef],  # (1)
    name: str,
    description: str,
    creatorMemberAbilities: Sequence[MemberAbilityType],  # (2)
    creatorDisplayName: str,
    queryLogStatus: CollaborationQueryLogStatusType,  # (3)
    dataEncryptionMetadata: NotRequired[DataEncryptionMetadataTypeDef],  # (4)
    tags: NotRequired[Mapping[str, str]],
    creatorPaymentConfiguration: NotRequired[PaymentConfigurationTypeDef],  # (5)
```

1. See [:material-code-braces: MemberSpecificationTypeDef](./type_defs.md#memberspecificationtypedef) 
2. See [:material-code-brackets: MemberAbilityType](./literals.md#memberabilitytype) 
3. See [:material-code-brackets: CollaborationQueryLogStatusType](./literals.md#collaborationquerylogstatustype) 
4. See [:material-code-braces: DataEncryptionMetadataTypeDef](./type_defs.md#dataencryptionmetadatatypedef) 
5. See [:material-code-braces: PaymentConfigurationTypeDef](./type_defs.md#paymentconfigurationtypedef) 
## ListMembersOutputTypeDef

```python
# ListMembersOutputTypeDef definition

class ListMembersOutputTypeDef(TypedDict):
    nextToken: str,
    memberSummaries: List[MemberSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MemberSummaryTypeDef](./type_defs.md#membersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProtectedQueryTypeDef

```python
# ProtectedQueryTypeDef definition

class ProtectedQueryTypeDef(TypedDict):
    id: str,
    membershipId: str,
    membershipArn: str,
    createTime: datetime,
    status: ProtectedQueryStatusType,  # (2)
    sqlParameters: NotRequired[ProtectedQuerySQLParametersTypeDef],  # (1)
    resultConfiguration: NotRequired[ProtectedQueryResultConfigurationTypeDef],  # (3)
    statistics: NotRequired[ProtectedQueryStatisticsTypeDef],  # (4)
    result: NotRequired[ProtectedQueryResultTypeDef],  # (5)
    error: NotRequired[ProtectedQueryErrorTypeDef],  # (6)
    differentialPrivacy: NotRequired[DifferentialPrivacyParametersTypeDef],  # (7)
```

1. See [:material-code-braces: ProtectedQuerySQLParametersTypeDef](./type_defs.md#protectedquerysqlparameterstypedef) 
2. See [:material-code-brackets: ProtectedQueryStatusType](./literals.md#protectedquerystatustype) 
3. See [:material-code-braces: ProtectedQueryResultConfigurationTypeDef](./type_defs.md#protectedqueryresultconfigurationtypedef) 
4. See [:material-code-braces: ProtectedQueryStatisticsTypeDef](./type_defs.md#protectedquerystatisticstypedef) 
5. See [:material-code-braces: ProtectedQueryResultTypeDef](./type_defs.md#protectedqueryresulttypedef) 
6. See [:material-code-braces: ProtectedQueryErrorTypeDef](./type_defs.md#protectedqueryerrortypedef) 
7. See [:material-code-braces: DifferentialPrivacyParametersTypeDef](./type_defs.md#differentialprivacyparameterstypedef) 
## AnalysisRulePolicyTypeDef

```python
# AnalysisRulePolicyTypeDef definition

class AnalysisRulePolicyTypeDef(TypedDict):
    v1: NotRequired[AnalysisRulePolicyV1TypeDef],  # (1)
```

1. See [:material-code-braces: AnalysisRulePolicyV1TypeDef](./type_defs.md#analysisrulepolicyv1typedef) 
## ConfiguredTableAnalysisRulePolicyTypeDef

```python
# ConfiguredTableAnalysisRulePolicyTypeDef definition

class ConfiguredTableAnalysisRulePolicyTypeDef(TypedDict):
    v1: NotRequired[ConfiguredTableAnalysisRulePolicyV1TypeDef],  # (1)
```

1. See [:material-code-braces: ConfiguredTableAnalysisRulePolicyV1TypeDef](./type_defs.md#configuredtableanalysisrulepolicyv1typedef) 
## ListCollaborationPrivacyBudgetsOutputTypeDef

```python
# ListCollaborationPrivacyBudgetsOutputTypeDef definition

class ListCollaborationPrivacyBudgetsOutputTypeDef(TypedDict):
    collaborationPrivacyBudgetSummaries: List[CollaborationPrivacyBudgetSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CollaborationPrivacyBudgetSummaryTypeDef](./type_defs.md#collaborationprivacybudgetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPrivacyBudgetsOutputTypeDef

```python
# ListPrivacyBudgetsOutputTypeDef definition

class ListPrivacyBudgetsOutputTypeDef(TypedDict):
    privacyBudgetSummaries: List[PrivacyBudgetSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PrivacyBudgetSummaryTypeDef](./type_defs.md#privacybudgetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMembershipOutputTypeDef

```python
# CreateMembershipOutputTypeDef definition

class CreateMembershipOutputTypeDef(TypedDict):
    membership: MembershipTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MembershipTypeDef](./type_defs.md#membershiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMembershipOutputTypeDef

```python
# GetMembershipOutputTypeDef definition

class GetMembershipOutputTypeDef(TypedDict):
    membership: MembershipTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MembershipTypeDef](./type_defs.md#membershiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMembershipOutputTypeDef

```python
# UpdateMembershipOutputTypeDef definition

class UpdateMembershipOutputTypeDef(TypedDict):
    membership: MembershipTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MembershipTypeDef](./type_defs.md#membershiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProtectedQueryOutputTypeDef

```python
# GetProtectedQueryOutputTypeDef definition

class GetProtectedQueryOutputTypeDef(TypedDict):
    protectedQuery: ProtectedQueryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProtectedQueryTypeDef](./type_defs.md#protectedquerytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartProtectedQueryOutputTypeDef

```python
# StartProtectedQueryOutputTypeDef definition

class StartProtectedQueryOutputTypeDef(TypedDict):
    protectedQuery: ProtectedQueryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProtectedQueryTypeDef](./type_defs.md#protectedquerytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProtectedQueryOutputTypeDef

```python
# UpdateProtectedQueryOutputTypeDef definition

class UpdateProtectedQueryOutputTypeDef(TypedDict):
    protectedQuery: ProtectedQueryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProtectedQueryTypeDef](./type_defs.md#protectedquerytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AnalysisRuleTypeDef

```python
# AnalysisRuleTypeDef definition

class AnalysisRuleTypeDef(TypedDict):
    collaborationId: str,
    type: AnalysisRuleTypeType,  # (1)
    name: str,
    createTime: datetime,
    updateTime: datetime,
    policy: AnalysisRulePolicyTypeDef,  # (2)
```

1. See [:material-code-brackets: AnalysisRuleTypeType](./literals.md#analysisruletypetype) 
2. See [:material-code-braces: AnalysisRulePolicyTypeDef](./type_defs.md#analysisrulepolicytypedef) 
## ConfiguredTableAnalysisRuleTypeDef

```python
# ConfiguredTableAnalysisRuleTypeDef definition

class ConfiguredTableAnalysisRuleTypeDef(TypedDict):
    configuredTableId: str,
    configuredTableArn: str,
    policy: ConfiguredTableAnalysisRulePolicyTypeDef,  # (1)
    type: ConfiguredTableAnalysisRuleTypeType,  # (2)
    createTime: datetime,
    updateTime: datetime,
```

1. See [:material-code-braces: ConfiguredTableAnalysisRulePolicyTypeDef](./type_defs.md#configuredtableanalysisrulepolicytypedef) 
2. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
## CreateConfiguredTableAnalysisRuleInputRequestTypeDef

```python
# CreateConfiguredTableAnalysisRuleInputRequestTypeDef definition

class CreateConfiguredTableAnalysisRuleInputRequestTypeDef(TypedDict):
    configuredTableIdentifier: str,
    analysisRuleType: ConfiguredTableAnalysisRuleTypeType,  # (1)
    analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef,  # (2)
```

1. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
2. See [:material-code-braces: ConfiguredTableAnalysisRulePolicyTypeDef](./type_defs.md#configuredtableanalysisrulepolicytypedef) 
## UpdateConfiguredTableAnalysisRuleInputRequestTypeDef

```python
# UpdateConfiguredTableAnalysisRuleInputRequestTypeDef definition

class UpdateConfiguredTableAnalysisRuleInputRequestTypeDef(TypedDict):
    configuredTableIdentifier: str,
    analysisRuleType: ConfiguredTableAnalysisRuleTypeType,  # (1)
    analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef,  # (2)
```

1. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
2. See [:material-code-braces: ConfiguredTableAnalysisRulePolicyTypeDef](./type_defs.md#configuredtableanalysisrulepolicytypedef) 
## GetSchemaAnalysisRuleOutputTypeDef

```python
# GetSchemaAnalysisRuleOutputTypeDef definition

class GetSchemaAnalysisRuleOutputTypeDef(TypedDict):
    analysisRule: AnalysisRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalysisRuleTypeDef](./type_defs.md#analysisruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfiguredTableAnalysisRuleOutputTypeDef

```python
# CreateConfiguredTableAnalysisRuleOutputTypeDef definition

class CreateConfiguredTableAnalysisRuleOutputTypeDef(TypedDict):
    analysisRule: ConfiguredTableAnalysisRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableAnalysisRuleTypeDef](./type_defs.md#configuredtableanalysisruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConfiguredTableAnalysisRuleOutputTypeDef

```python
# GetConfiguredTableAnalysisRuleOutputTypeDef definition

class GetConfiguredTableAnalysisRuleOutputTypeDef(TypedDict):
    analysisRule: ConfiguredTableAnalysisRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableAnalysisRuleTypeDef](./type_defs.md#configuredtableanalysisruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConfiguredTableAnalysisRuleOutputTypeDef

```python
# UpdateConfiguredTableAnalysisRuleOutputTypeDef definition

class UpdateConfiguredTableAnalysisRuleOutputTypeDef(TypedDict):
    analysisRule: ConfiguredTableAnalysisRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableAnalysisRuleTypeDef](./type_defs.md#configuredtableanalysisruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
