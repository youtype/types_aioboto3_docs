# Type definitions

> [Index](../README.md) > [Greengrass](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Greengrass](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#greengrass)
    type annotations stubs module [types-aiobotocore-greengrass](https://pypi.org/project/types-aiobotocore-greengrass/).

## ConnectorUnionTypeDef

```python
# ConnectorUnionTypeDef definition

ConnectorUnionTypeDef = Union[
    ConnectorTypeDef,  # (1)
    ConnectorOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConnectorTypeDef](./type_defs.md#connectortypedef) 
2. See [:material-code-braces: ConnectorOutputTypeDef](./type_defs.md#connectoroutputtypedef) 

## SecretsManagerSecretResourceDataUnionTypeDef

```python
# SecretsManagerSecretResourceDataUnionTypeDef definition

SecretsManagerSecretResourceDataUnionTypeDef = Union[
    SecretsManagerSecretResourceDataTypeDef,  # (1)
    SecretsManagerSecretResourceDataOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SecretsManagerSecretResourceDataTypeDef](./type_defs.md#secretsmanagersecretresourcedatatypedef) 
2. See [:material-code-braces: SecretsManagerSecretResourceDataOutputTypeDef](./type_defs.md#secretsmanagersecretresourcedataoutputtypedef) 

## FunctionConfigurationEnvironmentUnionTypeDef

```python
# FunctionConfigurationEnvironmentUnionTypeDef definition

FunctionConfigurationEnvironmentUnionTypeDef = Union[
    FunctionConfigurationEnvironmentTypeDef,  # (1)
    FunctionConfigurationEnvironmentOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FunctionConfigurationEnvironmentTypeDef](./type_defs.md#functionconfigurationenvironmenttypedef) 
2. See [:material-code-braces: FunctionConfigurationEnvironmentOutputTypeDef](./type_defs.md#functionconfigurationenvironmentoutputtypedef) 

## ResourceDataContainerUnionTypeDef

```python
# ResourceDataContainerUnionTypeDef definition

ResourceDataContainerUnionTypeDef = Union[
    ResourceDataContainerTypeDef,  # (1)
    ResourceDataContainerOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ResourceDataContainerTypeDef](./type_defs.md#resourcedatacontainertypedef) 
2. See [:material-code-braces: ResourceDataContainerOutputTypeDef](./type_defs.md#resourcedatacontaineroutputtypedef) 

## FunctionConfigurationUnionTypeDef

```python
# FunctionConfigurationUnionTypeDef definition

FunctionConfigurationUnionTypeDef = Union[
    FunctionConfigurationTypeDef,  # (1)
    FunctionConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FunctionConfigurationTypeDef](./type_defs.md#functionconfigurationtypedef) 
2. See [:material-code-braces: FunctionConfigurationOutputTypeDef](./type_defs.md#functionconfigurationoutputtypedef) 

## ResourceUnionTypeDef

```python
# ResourceUnionTypeDef definition

ResourceUnionTypeDef = Union[
    ResourceTypeDef,  # (1)
    ResourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef) 

## FunctionUnionTypeDef

```python
# FunctionUnionTypeDef definition

FunctionUnionTypeDef = Union[
    FunctionTypeDef,  # (1)
    FunctionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FunctionTypeDef](./type_defs.md#functiontypedef) 
2. See [:material-code-braces: FunctionOutputTypeDef](./type_defs.md#functionoutputtypedef) 



## AssociateRoleToGroupRequestRequestTypeDef

```python
# AssociateRoleToGroupRequestRequestTypeDef definition

class AssociateRoleToGroupRequestRequestTypeDef(TypedDict):
    GroupId: str,
    RoleArn: str,
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

## AssociateServiceRoleToAccountRequestRequestTypeDef

```python
# AssociateServiceRoleToAccountRequestRequestTypeDef definition

class AssociateServiceRoleToAccountRequestRequestTypeDef(TypedDict):
    RoleArn: str,
```

## BulkDeploymentMetricsTypeDef

```python
# BulkDeploymentMetricsTypeDef definition

class BulkDeploymentMetricsTypeDef(TypedDict):
    InvalidInputRecords: NotRequired[int],
    RecordsProcessed: NotRequired[int],
    RetryAttempts: NotRequired[int],
```

## ErrorDetailTypeDef

```python
# ErrorDetailTypeDef definition

class ErrorDetailTypeDef(TypedDict):
    DetailedErrorCode: NotRequired[str],
    DetailedErrorMessage: NotRequired[str],
```

## BulkDeploymentTypeDef

```python
# BulkDeploymentTypeDef definition

class BulkDeploymentTypeDef(TypedDict):
    BulkDeploymentArn: NotRequired[str],
    BulkDeploymentId: NotRequired[str],
    CreatedAt: NotRequired[str],
```

## ConnectivityInfoTypeDef

```python
# ConnectivityInfoTypeDef definition

class ConnectivityInfoTypeDef(TypedDict):
    HostAddress: NotRequired[str],
    Id: NotRequired[str],
    Metadata: NotRequired[str],
    PortNumber: NotRequired[int],
```

## ConnectorOutputTypeDef

```python
# ConnectorOutputTypeDef definition

class ConnectorOutputTypeDef(TypedDict):
    ConnectorArn: str,
    Id: str,
    Parameters: NotRequired[dict[str, str]],
```

## ConnectorTypeDef

```python
# ConnectorTypeDef definition

class ConnectorTypeDef(TypedDict):
    ConnectorArn: str,
    Id: str,
    Parameters: NotRequired[Mapping[str, str]],
```

## CoreTypeDef

```python
# CoreTypeDef definition

class CoreTypeDef(TypedDict):
    CertificateArn: str,
    Id: str,
    ThingArn: str,
    SyncShadow: NotRequired[bool],
```

## CreateDeploymentRequestRequestTypeDef

```python
# CreateDeploymentRequestRequestTypeDef definition

class CreateDeploymentRequestRequestTypeDef(TypedDict):
    DeploymentType: DeploymentTypeType,  # (1)
    GroupId: str,
    AmznClientToken: NotRequired[str],
    DeploymentId: NotRequired[str],
    GroupVersionId: NotRequired[str],
```

1. See [:material-code-brackets: DeploymentTypeType](./literals.md#deploymenttypetype) 
## DeviceTypeDef

```python
# DeviceTypeDef definition

class DeviceTypeDef(TypedDict):
    CertificateArn: str,
    Id: str,
    ThingArn: str,
    SyncShadow: NotRequired[bool],
```

## CreateGroupCertificateAuthorityRequestRequestTypeDef

```python
# CreateGroupCertificateAuthorityRequestRequestTypeDef definition

class CreateGroupCertificateAuthorityRequestRequestTypeDef(TypedDict):
    GroupId: str,
    AmznClientToken: NotRequired[str],
```

## GroupVersionTypeDef

```python
# GroupVersionTypeDef definition

class GroupVersionTypeDef(TypedDict):
    ConnectorDefinitionVersionArn: NotRequired[str],
    CoreDefinitionVersionArn: NotRequired[str],
    DeviceDefinitionVersionArn: NotRequired[str],
    FunctionDefinitionVersionArn: NotRequired[str],
    LoggerDefinitionVersionArn: NotRequired[str],
    ResourceDefinitionVersionArn: NotRequired[str],
    SubscriptionDefinitionVersionArn: NotRequired[str],
```

## CreateGroupVersionRequestRequestTypeDef

```python
# CreateGroupVersionRequestRequestTypeDef definition

class CreateGroupVersionRequestRequestTypeDef(TypedDict):
    GroupId: str,
    AmznClientToken: NotRequired[str],
    ConnectorDefinitionVersionArn: NotRequired[str],
    CoreDefinitionVersionArn: NotRequired[str],
    DeviceDefinitionVersionArn: NotRequired[str],
    FunctionDefinitionVersionArn: NotRequired[str],
    LoggerDefinitionVersionArn: NotRequired[str],
    ResourceDefinitionVersionArn: NotRequired[str],
    SubscriptionDefinitionVersionArn: NotRequired[str],
```

## LoggerTypeDef

```python
# LoggerTypeDef definition

class LoggerTypeDef(TypedDict):
    Component: LoggerComponentType,  # (1)
    Id: str,
    Level: LoggerLevelType,  # (2)
    Type: LoggerTypeType,  # (3)
    Space: NotRequired[int],
```

1. See [:material-code-brackets: LoggerComponentType](./literals.md#loggercomponenttype) 
2. See [:material-code-brackets: LoggerLevelType](./literals.md#loggerleveltype) 
3. See [:material-code-brackets: LoggerTypeType](./literals.md#loggertypetype) 
## CreateSoftwareUpdateJobRequestRequestTypeDef

```python
# CreateSoftwareUpdateJobRequestRequestTypeDef definition

class CreateSoftwareUpdateJobRequestRequestTypeDef(TypedDict):
    S3UrlSignerRole: str,
    SoftwareToUpdate: SoftwareToUpdateType,  # (1)
    UpdateTargets: Sequence[str],
    UpdateTargetsArchitecture: UpdateTargetsArchitectureType,  # (2)
    UpdateTargetsOperatingSystem: UpdateTargetsOperatingSystemType,  # (3)
    AmznClientToken: NotRequired[str],
    UpdateAgentLogLevel: NotRequired[UpdateAgentLogLevelType],  # (4)
```

1. See [:material-code-brackets: SoftwareToUpdateType](./literals.md#softwaretoupdatetype) 
2. See [:material-code-brackets: UpdateTargetsArchitectureType](./literals.md#updatetargetsarchitecturetype) 
3. See [:material-code-brackets: UpdateTargetsOperatingSystemType](./literals.md#updatetargetsoperatingsystemtype) 
4. See [:material-code-brackets: UpdateAgentLogLevelType](./literals.md#updateagentlogleveltype) 
## SubscriptionTypeDef

```python
# SubscriptionTypeDef definition

class SubscriptionTypeDef(TypedDict):
    Id: str,
    Source: str,
    Subject: str,
    Target: str,
```

## DefinitionInformationTypeDef

```python
# DefinitionInformationTypeDef definition

class DefinitionInformationTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreationTimestamp: NotRequired[str],
    Id: NotRequired[str],
    LastUpdatedTimestamp: NotRequired[str],
    LatestVersion: NotRequired[str],
    LatestVersionArn: NotRequired[str],
    Name: NotRequired[str],
    Tags: NotRequired[dict[str, str]],
```

## DeleteConnectorDefinitionRequestRequestTypeDef

```python
# DeleteConnectorDefinitionRequestRequestTypeDef definition

class DeleteConnectorDefinitionRequestRequestTypeDef(TypedDict):
    ConnectorDefinitionId: str,
```

## DeleteCoreDefinitionRequestRequestTypeDef

```python
# DeleteCoreDefinitionRequestRequestTypeDef definition

class DeleteCoreDefinitionRequestRequestTypeDef(TypedDict):
    CoreDefinitionId: str,
```

## DeleteDeviceDefinitionRequestRequestTypeDef

```python
# DeleteDeviceDefinitionRequestRequestTypeDef definition

class DeleteDeviceDefinitionRequestRequestTypeDef(TypedDict):
    DeviceDefinitionId: str,
```

## DeleteFunctionDefinitionRequestRequestTypeDef

```python
# DeleteFunctionDefinitionRequestRequestTypeDef definition

class DeleteFunctionDefinitionRequestRequestTypeDef(TypedDict):
    FunctionDefinitionId: str,
```

## DeleteGroupRequestRequestTypeDef

```python
# DeleteGroupRequestRequestTypeDef definition

class DeleteGroupRequestRequestTypeDef(TypedDict):
    GroupId: str,
```

## DeleteLoggerDefinitionRequestRequestTypeDef

```python
# DeleteLoggerDefinitionRequestRequestTypeDef definition

class DeleteLoggerDefinitionRequestRequestTypeDef(TypedDict):
    LoggerDefinitionId: str,
```

## DeleteResourceDefinitionRequestRequestTypeDef

```python
# DeleteResourceDefinitionRequestRequestTypeDef definition

class DeleteResourceDefinitionRequestRequestTypeDef(TypedDict):
    ResourceDefinitionId: str,
```

## DeleteSubscriptionDefinitionRequestRequestTypeDef

```python
# DeleteSubscriptionDefinitionRequestRequestTypeDef definition

class DeleteSubscriptionDefinitionRequestRequestTypeDef(TypedDict):
    SubscriptionDefinitionId: str,
```

## DeploymentTypeDef

```python
# DeploymentTypeDef definition

class DeploymentTypeDef(TypedDict):
    CreatedAt: NotRequired[str],
    DeploymentArn: NotRequired[str],
    DeploymentId: NotRequired[str],
    DeploymentType: NotRequired[DeploymentTypeType],  # (1)
    GroupArn: NotRequired[str],
```

1. See [:material-code-brackets: DeploymentTypeType](./literals.md#deploymenttypetype) 
## DisassociateRoleFromGroupRequestRequestTypeDef

```python
# DisassociateRoleFromGroupRequestRequestTypeDef definition

class DisassociateRoleFromGroupRequestRequestTypeDef(TypedDict):
    GroupId: str,
```

## ResourceAccessPolicyTypeDef

```python
# ResourceAccessPolicyTypeDef definition

class ResourceAccessPolicyTypeDef(TypedDict):
    ResourceId: str,
    Permission: NotRequired[PermissionType],  # (1)
```

1. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
## FunctionRunAsConfigTypeDef

```python
# FunctionRunAsConfigTypeDef definition

class FunctionRunAsConfigTypeDef(TypedDict):
    Gid: NotRequired[int],
    Uid: NotRequired[int],
```

## GetAssociatedRoleRequestRequestTypeDef

```python
# GetAssociatedRoleRequestRequestTypeDef definition

class GetAssociatedRoleRequestRequestTypeDef(TypedDict):
    GroupId: str,
```

## GetBulkDeploymentStatusRequestRequestTypeDef

```python
# GetBulkDeploymentStatusRequestRequestTypeDef definition

class GetBulkDeploymentStatusRequestRequestTypeDef(TypedDict):
    BulkDeploymentId: str,
```

## GetConnectivityInfoRequestRequestTypeDef

```python
# GetConnectivityInfoRequestRequestTypeDef definition

class GetConnectivityInfoRequestRequestTypeDef(TypedDict):
    ThingName: str,
```

## GetConnectorDefinitionRequestRequestTypeDef

```python
# GetConnectorDefinitionRequestRequestTypeDef definition

class GetConnectorDefinitionRequestRequestTypeDef(TypedDict):
    ConnectorDefinitionId: str,
```

## GetConnectorDefinitionVersionRequestRequestTypeDef

```python
# GetConnectorDefinitionVersionRequestRequestTypeDef definition

class GetConnectorDefinitionVersionRequestRequestTypeDef(TypedDict):
    ConnectorDefinitionId: str,
    ConnectorDefinitionVersionId: str,
    NextToken: NotRequired[str],
```

## GetCoreDefinitionRequestRequestTypeDef

```python
# GetCoreDefinitionRequestRequestTypeDef definition

class GetCoreDefinitionRequestRequestTypeDef(TypedDict):
    CoreDefinitionId: str,
```

## GetCoreDefinitionVersionRequestRequestTypeDef

```python
# GetCoreDefinitionVersionRequestRequestTypeDef definition

class GetCoreDefinitionVersionRequestRequestTypeDef(TypedDict):
    CoreDefinitionId: str,
    CoreDefinitionVersionId: str,
```

## GetDeploymentStatusRequestRequestTypeDef

```python
# GetDeploymentStatusRequestRequestTypeDef definition

class GetDeploymentStatusRequestRequestTypeDef(TypedDict):
    DeploymentId: str,
    GroupId: str,
```

## GetDeviceDefinitionRequestRequestTypeDef

```python
# GetDeviceDefinitionRequestRequestTypeDef definition

class GetDeviceDefinitionRequestRequestTypeDef(TypedDict):
    DeviceDefinitionId: str,
```

## GetDeviceDefinitionVersionRequestRequestTypeDef

```python
# GetDeviceDefinitionVersionRequestRequestTypeDef definition

class GetDeviceDefinitionVersionRequestRequestTypeDef(TypedDict):
    DeviceDefinitionId: str,
    DeviceDefinitionVersionId: str,
    NextToken: NotRequired[str],
```

## GetFunctionDefinitionRequestRequestTypeDef

```python
# GetFunctionDefinitionRequestRequestTypeDef definition

class GetFunctionDefinitionRequestRequestTypeDef(TypedDict):
    FunctionDefinitionId: str,
```

## GetFunctionDefinitionVersionRequestRequestTypeDef

```python
# GetFunctionDefinitionVersionRequestRequestTypeDef definition

class GetFunctionDefinitionVersionRequestRequestTypeDef(TypedDict):
    FunctionDefinitionId: str,
    FunctionDefinitionVersionId: str,
    NextToken: NotRequired[str],
```

## GetGroupCertificateAuthorityRequestRequestTypeDef

```python
# GetGroupCertificateAuthorityRequestRequestTypeDef definition

class GetGroupCertificateAuthorityRequestRequestTypeDef(TypedDict):
    CertificateAuthorityId: str,
    GroupId: str,
```

## GetGroupCertificateConfigurationRequestRequestTypeDef

```python
# GetGroupCertificateConfigurationRequestRequestTypeDef definition

class GetGroupCertificateConfigurationRequestRequestTypeDef(TypedDict):
    GroupId: str,
```

## GetGroupRequestRequestTypeDef

```python
# GetGroupRequestRequestTypeDef definition

class GetGroupRequestRequestTypeDef(TypedDict):
    GroupId: str,
```

## GetGroupVersionRequestRequestTypeDef

```python
# GetGroupVersionRequestRequestTypeDef definition

class GetGroupVersionRequestRequestTypeDef(TypedDict):
    GroupId: str,
    GroupVersionId: str,
```

## GetLoggerDefinitionRequestRequestTypeDef

```python
# GetLoggerDefinitionRequestRequestTypeDef definition

class GetLoggerDefinitionRequestRequestTypeDef(TypedDict):
    LoggerDefinitionId: str,
```

## GetLoggerDefinitionVersionRequestRequestTypeDef

```python
# GetLoggerDefinitionVersionRequestRequestTypeDef definition

class GetLoggerDefinitionVersionRequestRequestTypeDef(TypedDict):
    LoggerDefinitionId: str,
    LoggerDefinitionVersionId: str,
    NextToken: NotRequired[str],
```

## GetResourceDefinitionRequestRequestTypeDef

```python
# GetResourceDefinitionRequestRequestTypeDef definition

class GetResourceDefinitionRequestRequestTypeDef(TypedDict):
    ResourceDefinitionId: str,
```

## GetResourceDefinitionVersionRequestRequestTypeDef

```python
# GetResourceDefinitionVersionRequestRequestTypeDef definition

class GetResourceDefinitionVersionRequestRequestTypeDef(TypedDict):
    ResourceDefinitionId: str,
    ResourceDefinitionVersionId: str,
```

## GetSubscriptionDefinitionRequestRequestTypeDef

```python
# GetSubscriptionDefinitionRequestRequestTypeDef definition

class GetSubscriptionDefinitionRequestRequestTypeDef(TypedDict):
    SubscriptionDefinitionId: str,
```

## GetSubscriptionDefinitionVersionRequestRequestTypeDef

```python
# GetSubscriptionDefinitionVersionRequestRequestTypeDef definition

class GetSubscriptionDefinitionVersionRequestRequestTypeDef(TypedDict):
    SubscriptionDefinitionId: str,
    SubscriptionDefinitionVersionId: str,
    NextToken: NotRequired[str],
```

## GetThingRuntimeConfigurationRequestRequestTypeDef

```python
# GetThingRuntimeConfigurationRequestRequestTypeDef definition

class GetThingRuntimeConfigurationRequestRequestTypeDef(TypedDict):
    ThingName: str,
```

## GroupCertificateAuthorityPropertiesTypeDef

```python
# GroupCertificateAuthorityPropertiesTypeDef definition

class GroupCertificateAuthorityPropertiesTypeDef(TypedDict):
    GroupCertificateAuthorityArn: NotRequired[str],
    GroupCertificateAuthorityId: NotRequired[str],
```

## GroupInformationTypeDef

```python
# GroupInformationTypeDef definition

class GroupInformationTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreationTimestamp: NotRequired[str],
    Id: NotRequired[str],
    LastUpdatedTimestamp: NotRequired[str],
    LatestVersion: NotRequired[str],
    LatestVersionArn: NotRequired[str],
    Name: NotRequired[str],
```

## GroupOwnerSettingTypeDef

```python
# GroupOwnerSettingTypeDef definition

class GroupOwnerSettingTypeDef(TypedDict):
    AutoAddGroupOwner: NotRequired[bool],
    GroupOwner: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListBulkDeploymentDetailedReportsRequestRequestTypeDef

```python
# ListBulkDeploymentDetailedReportsRequestRequestTypeDef definition

class ListBulkDeploymentDetailedReportsRequestRequestTypeDef(TypedDict):
    BulkDeploymentId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## ListBulkDeploymentsRequestRequestTypeDef

```python
# ListBulkDeploymentsRequestRequestTypeDef definition

class ListBulkDeploymentsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## ListConnectorDefinitionVersionsRequestRequestTypeDef

```python
# ListConnectorDefinitionVersionsRequestRequestTypeDef definition

class ListConnectorDefinitionVersionsRequestRequestTypeDef(TypedDict):
    ConnectorDefinitionId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## VersionInformationTypeDef

```python
# VersionInformationTypeDef definition

class VersionInformationTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreationTimestamp: NotRequired[str],
    Id: NotRequired[str],
    Version: NotRequired[str],
```

## ListConnectorDefinitionsRequestRequestTypeDef

```python
# ListConnectorDefinitionsRequestRequestTypeDef definition

class ListConnectorDefinitionsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## ListCoreDefinitionVersionsRequestRequestTypeDef

```python
# ListCoreDefinitionVersionsRequestRequestTypeDef definition

class ListCoreDefinitionVersionsRequestRequestTypeDef(TypedDict):
    CoreDefinitionId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## ListCoreDefinitionsRequestRequestTypeDef

```python
# ListCoreDefinitionsRequestRequestTypeDef definition

class ListCoreDefinitionsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## ListDeploymentsRequestRequestTypeDef

```python
# ListDeploymentsRequestRequestTypeDef definition

class ListDeploymentsRequestRequestTypeDef(TypedDict):
    GroupId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## ListDeviceDefinitionVersionsRequestRequestTypeDef

```python
# ListDeviceDefinitionVersionsRequestRequestTypeDef definition

class ListDeviceDefinitionVersionsRequestRequestTypeDef(TypedDict):
    DeviceDefinitionId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## ListDeviceDefinitionsRequestRequestTypeDef

```python
# ListDeviceDefinitionsRequestRequestTypeDef definition

class ListDeviceDefinitionsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## ListFunctionDefinitionVersionsRequestRequestTypeDef

```python
# ListFunctionDefinitionVersionsRequestRequestTypeDef definition

class ListFunctionDefinitionVersionsRequestRequestTypeDef(TypedDict):
    FunctionDefinitionId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## ListFunctionDefinitionsRequestRequestTypeDef

```python
# ListFunctionDefinitionsRequestRequestTypeDef definition

class ListFunctionDefinitionsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## ListGroupCertificateAuthoritiesRequestRequestTypeDef

```python
# ListGroupCertificateAuthoritiesRequestRequestTypeDef definition

class ListGroupCertificateAuthoritiesRequestRequestTypeDef(TypedDict):
    GroupId: str,
```

## ListGroupVersionsRequestRequestTypeDef

```python
# ListGroupVersionsRequestRequestTypeDef definition

class ListGroupVersionsRequestRequestTypeDef(TypedDict):
    GroupId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## ListGroupsRequestRequestTypeDef

```python
# ListGroupsRequestRequestTypeDef definition

class ListGroupsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## ListLoggerDefinitionVersionsRequestRequestTypeDef

```python
# ListLoggerDefinitionVersionsRequestRequestTypeDef definition

class ListLoggerDefinitionVersionsRequestRequestTypeDef(TypedDict):
    LoggerDefinitionId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## ListLoggerDefinitionsRequestRequestTypeDef

```python
# ListLoggerDefinitionsRequestRequestTypeDef definition

class ListLoggerDefinitionsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## ListResourceDefinitionVersionsRequestRequestTypeDef

```python
# ListResourceDefinitionVersionsRequestRequestTypeDef definition

class ListResourceDefinitionVersionsRequestRequestTypeDef(TypedDict):
    ResourceDefinitionId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## ListResourceDefinitionsRequestRequestTypeDef

```python
# ListResourceDefinitionsRequestRequestTypeDef definition

class ListResourceDefinitionsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## ListSubscriptionDefinitionVersionsRequestRequestTypeDef

```python
# ListSubscriptionDefinitionVersionsRequestRequestTypeDef definition

class ListSubscriptionDefinitionVersionsRequestRequestTypeDef(TypedDict):
    SubscriptionDefinitionId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## ListSubscriptionDefinitionsRequestRequestTypeDef

```python
# ListSubscriptionDefinitionsRequestRequestTypeDef definition

class ListSubscriptionDefinitionsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ResetDeploymentsRequestRequestTypeDef

```python
# ResetDeploymentsRequestRequestTypeDef definition

class ResetDeploymentsRequestRequestTypeDef(TypedDict):
    GroupId: str,
    AmznClientToken: NotRequired[str],
    Force: NotRequired[bool],
```

## SecretsManagerSecretResourceDataOutputTypeDef

```python
# SecretsManagerSecretResourceDataOutputTypeDef definition

class SecretsManagerSecretResourceDataOutputTypeDef(TypedDict):
    ARN: NotRequired[str],
    AdditionalStagingLabelsToDownload: NotRequired[list[str]],
```

## ResourceDownloadOwnerSettingTypeDef

```python
# ResourceDownloadOwnerSettingTypeDef definition

class ResourceDownloadOwnerSettingTypeDef(TypedDict):
    GroupOwner: str,
    GroupPermission: PermissionType,  # (1)
```

1. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
## TelemetryConfigurationTypeDef

```python
# TelemetryConfigurationTypeDef definition

class TelemetryConfigurationTypeDef(TypedDict):
    Telemetry: TelemetryType,  # (2)
    ConfigurationSyncStatus: NotRequired[ConfigurationSyncStatusType],  # (1)
```

1. See [:material-code-brackets: ConfigurationSyncStatusType](./literals.md#configurationsyncstatustype) 
2. See [:material-code-brackets: TelemetryType](./literals.md#telemetrytype) 
## SecretsManagerSecretResourceDataTypeDef

```python
# SecretsManagerSecretResourceDataTypeDef definition

class SecretsManagerSecretResourceDataTypeDef(TypedDict):
    ARN: NotRequired[str],
    AdditionalStagingLabelsToDownload: NotRequired[Sequence[str]],
```

## StartBulkDeploymentRequestRequestTypeDef

```python
# StartBulkDeploymentRequestRequestTypeDef definition

class StartBulkDeploymentRequestRequestTypeDef(TypedDict):
    ExecutionRoleArn: str,
    InputFileUri: str,
    AmznClientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## StopBulkDeploymentRequestRequestTypeDef

```python
# StopBulkDeploymentRequestRequestTypeDef definition

class StopBulkDeploymentRequestRequestTypeDef(TypedDict):
    BulkDeploymentId: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    tags: NotRequired[Mapping[str, str]],
```

## TelemetryConfigurationUpdateTypeDef

```python
# TelemetryConfigurationUpdateTypeDef definition

class TelemetryConfigurationUpdateTypeDef(TypedDict):
    Telemetry: TelemetryType,  # (1)
```

1. See [:material-code-brackets: TelemetryType](./literals.md#telemetrytype) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateConnectorDefinitionRequestRequestTypeDef

```python
# UpdateConnectorDefinitionRequestRequestTypeDef definition

class UpdateConnectorDefinitionRequestRequestTypeDef(TypedDict):
    ConnectorDefinitionId: str,
    Name: NotRequired[str],
```

## UpdateCoreDefinitionRequestRequestTypeDef

```python
# UpdateCoreDefinitionRequestRequestTypeDef definition

class UpdateCoreDefinitionRequestRequestTypeDef(TypedDict):
    CoreDefinitionId: str,
    Name: NotRequired[str],
```

## UpdateDeviceDefinitionRequestRequestTypeDef

```python
# UpdateDeviceDefinitionRequestRequestTypeDef definition

class UpdateDeviceDefinitionRequestRequestTypeDef(TypedDict):
    DeviceDefinitionId: str,
    Name: NotRequired[str],
```

## UpdateFunctionDefinitionRequestRequestTypeDef

```python
# UpdateFunctionDefinitionRequestRequestTypeDef definition

class UpdateFunctionDefinitionRequestRequestTypeDef(TypedDict):
    FunctionDefinitionId: str,
    Name: NotRequired[str],
```

## UpdateGroupCertificateConfigurationRequestRequestTypeDef

```python
# UpdateGroupCertificateConfigurationRequestRequestTypeDef definition

class UpdateGroupCertificateConfigurationRequestRequestTypeDef(TypedDict):
    GroupId: str,
    CertificateExpiryInMilliseconds: NotRequired[str],
```

## UpdateGroupRequestRequestTypeDef

```python
# UpdateGroupRequestRequestTypeDef definition

class UpdateGroupRequestRequestTypeDef(TypedDict):
    GroupId: str,
    Name: NotRequired[str],
```

## UpdateLoggerDefinitionRequestRequestTypeDef

```python
# UpdateLoggerDefinitionRequestRequestTypeDef definition

class UpdateLoggerDefinitionRequestRequestTypeDef(TypedDict):
    LoggerDefinitionId: str,
    Name: NotRequired[str],
```

## UpdateResourceDefinitionRequestRequestTypeDef

```python
# UpdateResourceDefinitionRequestRequestTypeDef definition

class UpdateResourceDefinitionRequestRequestTypeDef(TypedDict):
    ResourceDefinitionId: str,
    Name: NotRequired[str],
```

## UpdateSubscriptionDefinitionRequestRequestTypeDef

```python
# UpdateSubscriptionDefinitionRequestRequestTypeDef definition

class UpdateSubscriptionDefinitionRequestRequestTypeDef(TypedDict):
    SubscriptionDefinitionId: str,
    Name: NotRequired[str],
```

## AssociateRoleToGroupResponseTypeDef

```python
# AssociateRoleToGroupResponseTypeDef definition

class AssociateRoleToGroupResponseTypeDef(TypedDict):
    AssociatedAt: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateServiceRoleToAccountResponseTypeDef

```python
# AssociateServiceRoleToAccountResponseTypeDef definition

class AssociateServiceRoleToAccountResponseTypeDef(TypedDict):
    AssociatedAt: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConnectorDefinitionResponseTypeDef

```python
# CreateConnectorDefinitionResponseTypeDef definition

class CreateConnectorDefinitionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Id: str,
    LastUpdatedTimestamp: str,
    LatestVersion: str,
    LatestVersionArn: str,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConnectorDefinitionVersionResponseTypeDef

```python
# CreateConnectorDefinitionVersionResponseTypeDef definition

class CreateConnectorDefinitionVersionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Id: str,
    Version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCoreDefinitionResponseTypeDef

```python
# CreateCoreDefinitionResponseTypeDef definition

class CreateCoreDefinitionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Id: str,
    LastUpdatedTimestamp: str,
    LatestVersion: str,
    LatestVersionArn: str,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCoreDefinitionVersionResponseTypeDef

```python
# CreateCoreDefinitionVersionResponseTypeDef definition

class CreateCoreDefinitionVersionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Id: str,
    Version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDeploymentResponseTypeDef

```python
# CreateDeploymentResponseTypeDef definition

class CreateDeploymentResponseTypeDef(TypedDict):
    DeploymentArn: str,
    DeploymentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDeviceDefinitionResponseTypeDef

```python
# CreateDeviceDefinitionResponseTypeDef definition

class CreateDeviceDefinitionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Id: str,
    LastUpdatedTimestamp: str,
    LatestVersion: str,
    LatestVersionArn: str,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDeviceDefinitionVersionResponseTypeDef

```python
# CreateDeviceDefinitionVersionResponseTypeDef definition

class CreateDeviceDefinitionVersionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Id: str,
    Version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFunctionDefinitionResponseTypeDef

```python
# CreateFunctionDefinitionResponseTypeDef definition

class CreateFunctionDefinitionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Id: str,
    LastUpdatedTimestamp: str,
    LatestVersion: str,
    LatestVersionArn: str,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFunctionDefinitionVersionResponseTypeDef

```python
# CreateFunctionDefinitionVersionResponseTypeDef definition

class CreateFunctionDefinitionVersionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Id: str,
    Version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGroupCertificateAuthorityResponseTypeDef

```python
# CreateGroupCertificateAuthorityResponseTypeDef definition

class CreateGroupCertificateAuthorityResponseTypeDef(TypedDict):
    GroupCertificateAuthorityArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGroupResponseTypeDef

```python
# CreateGroupResponseTypeDef definition

class CreateGroupResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Id: str,
    LastUpdatedTimestamp: str,
    LatestVersion: str,
    LatestVersionArn: str,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGroupVersionResponseTypeDef

```python
# CreateGroupVersionResponseTypeDef definition

class CreateGroupVersionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Id: str,
    Version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLoggerDefinitionResponseTypeDef

```python
# CreateLoggerDefinitionResponseTypeDef definition

class CreateLoggerDefinitionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Id: str,
    LastUpdatedTimestamp: str,
    LatestVersion: str,
    LatestVersionArn: str,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLoggerDefinitionVersionResponseTypeDef

```python
# CreateLoggerDefinitionVersionResponseTypeDef definition

class CreateLoggerDefinitionVersionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Id: str,
    Version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateResourceDefinitionResponseTypeDef

```python
# CreateResourceDefinitionResponseTypeDef definition

class CreateResourceDefinitionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Id: str,
    LastUpdatedTimestamp: str,
    LatestVersion: str,
    LatestVersionArn: str,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateResourceDefinitionVersionResponseTypeDef

```python
# CreateResourceDefinitionVersionResponseTypeDef definition

class CreateResourceDefinitionVersionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Id: str,
    Version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSoftwareUpdateJobResponseTypeDef

```python
# CreateSoftwareUpdateJobResponseTypeDef definition

class CreateSoftwareUpdateJobResponseTypeDef(TypedDict):
    IotJobArn: str,
    IotJobId: str,
    PlatformSoftwareVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSubscriptionDefinitionResponseTypeDef

```python
# CreateSubscriptionDefinitionResponseTypeDef definition

class CreateSubscriptionDefinitionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Id: str,
    LastUpdatedTimestamp: str,
    LatestVersion: str,
    LatestVersionArn: str,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSubscriptionDefinitionVersionResponseTypeDef

```python
# CreateSubscriptionDefinitionVersionResponseTypeDef definition

class CreateSubscriptionDefinitionVersionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Id: str,
    Version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateRoleFromGroupResponseTypeDef

```python
# DisassociateRoleFromGroupResponseTypeDef definition

class DisassociateRoleFromGroupResponseTypeDef(TypedDict):
    DisassociatedAt: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateServiceRoleFromAccountResponseTypeDef

```python
# DisassociateServiceRoleFromAccountResponseTypeDef definition

class DisassociateServiceRoleFromAccountResponseTypeDef(TypedDict):
    DisassociatedAt: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAssociatedRoleResponseTypeDef

```python
# GetAssociatedRoleResponseTypeDef definition

class GetAssociatedRoleResponseTypeDef(TypedDict):
    AssociatedAt: str,
    RoleArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConnectorDefinitionResponseTypeDef

```python
# GetConnectorDefinitionResponseTypeDef definition

class GetConnectorDefinitionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Id: str,
    LastUpdatedTimestamp: str,
    LatestVersion: str,
    LatestVersionArn: str,
    Name: str,
    tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCoreDefinitionResponseTypeDef

```python
# GetCoreDefinitionResponseTypeDef definition

class GetCoreDefinitionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Id: str,
    LastUpdatedTimestamp: str,
    LatestVersion: str,
    LatestVersionArn: str,
    Name: str,
    tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeviceDefinitionResponseTypeDef

```python
# GetDeviceDefinitionResponseTypeDef definition

class GetDeviceDefinitionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Id: str,
    LastUpdatedTimestamp: str,
    LatestVersion: str,
    LatestVersionArn: str,
    Name: str,
    tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFunctionDefinitionResponseTypeDef

```python
# GetFunctionDefinitionResponseTypeDef definition

class GetFunctionDefinitionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Id: str,
    LastUpdatedTimestamp: str,
    LatestVersion: str,
    LatestVersionArn: str,
    Name: str,
    tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGroupCertificateAuthorityResponseTypeDef

```python
# GetGroupCertificateAuthorityResponseTypeDef definition

class GetGroupCertificateAuthorityResponseTypeDef(TypedDict):
    GroupCertificateAuthorityArn: str,
    GroupCertificateAuthorityId: str,
    PemEncodedCertificate: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGroupCertificateConfigurationResponseTypeDef

```python
# GetGroupCertificateConfigurationResponseTypeDef definition

class GetGroupCertificateConfigurationResponseTypeDef(TypedDict):
    CertificateAuthorityExpiryInMilliseconds: str,
    CertificateExpiryInMilliseconds: str,
    GroupId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGroupResponseTypeDef

```python
# GetGroupResponseTypeDef definition

class GetGroupResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Id: str,
    LastUpdatedTimestamp: str,
    LatestVersion: str,
    LatestVersionArn: str,
    Name: str,
    tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLoggerDefinitionResponseTypeDef

```python
# GetLoggerDefinitionResponseTypeDef definition

class GetLoggerDefinitionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Id: str,
    LastUpdatedTimestamp: str,
    LatestVersion: str,
    LatestVersionArn: str,
    Name: str,
    tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourceDefinitionResponseTypeDef

```python
# GetResourceDefinitionResponseTypeDef definition

class GetResourceDefinitionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Id: str,
    LastUpdatedTimestamp: str,
    LatestVersion: str,
    LatestVersionArn: str,
    Name: str,
    tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceRoleForAccountResponseTypeDef

```python
# GetServiceRoleForAccountResponseTypeDef definition

class GetServiceRoleForAccountResponseTypeDef(TypedDict):
    AssociatedAt: str,
    RoleArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSubscriptionDefinitionResponseTypeDef

```python
# GetSubscriptionDefinitionResponseTypeDef definition

class GetSubscriptionDefinitionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Id: str,
    LastUpdatedTimestamp: str,
    LatestVersion: str,
    LatestVersionArn: str,
    Name: str,
    tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResetDeploymentsResponseTypeDef

```python
# ResetDeploymentsResponseTypeDef definition

class ResetDeploymentsResponseTypeDef(TypedDict):
    DeploymentArn: str,
    DeploymentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartBulkDeploymentResponseTypeDef

```python
# StartBulkDeploymentResponseTypeDef definition

class StartBulkDeploymentResponseTypeDef(TypedDict):
    BulkDeploymentArn: str,
    BulkDeploymentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConnectivityInfoResponseTypeDef

```python
# UpdateConnectivityInfoResponseTypeDef definition

class UpdateConnectivityInfoResponseTypeDef(TypedDict):
    Message: str,
    Version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGroupCertificateConfigurationResponseTypeDef

```python
# UpdateGroupCertificateConfigurationResponseTypeDef definition

class UpdateGroupCertificateConfigurationResponseTypeDef(TypedDict):
    CertificateAuthorityExpiryInMilliseconds: str,
    CertificateExpiryInMilliseconds: str,
    GroupId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BulkDeploymentResultTypeDef

```python
# BulkDeploymentResultTypeDef definition

class BulkDeploymentResultTypeDef(TypedDict):
    CreatedAt: NotRequired[str],
    DeploymentArn: NotRequired[str],
    DeploymentId: NotRequired[str],
    DeploymentStatus: NotRequired[str],
    DeploymentType: NotRequired[DeploymentTypeType],  # (1)
    ErrorDetails: NotRequired[list[ErrorDetailTypeDef]],  # (2)
    ErrorMessage: NotRequired[str],
    GroupArn: NotRequired[str],
```

1. See [:material-code-brackets: DeploymentTypeType](./literals.md#deploymenttypetype) 
2. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## GetBulkDeploymentStatusResponseTypeDef

```python
# GetBulkDeploymentStatusResponseTypeDef definition

class GetBulkDeploymentStatusResponseTypeDef(TypedDict):
    BulkDeploymentMetrics: BulkDeploymentMetricsTypeDef,  # (1)
    BulkDeploymentStatus: BulkDeploymentStatusType,  # (2)
    CreatedAt: str,
    ErrorDetails: list[ErrorDetailTypeDef],  # (3)
    ErrorMessage: str,
    tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: BulkDeploymentMetricsTypeDef](./type_defs.md#bulkdeploymentmetricstypedef) 
2. See [:material-code-brackets: BulkDeploymentStatusType](./literals.md#bulkdeploymentstatustype) 
3. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeploymentStatusResponseTypeDef

```python
# GetDeploymentStatusResponseTypeDef definition

class GetDeploymentStatusResponseTypeDef(TypedDict):
    DeploymentStatus: str,
    DeploymentType: DeploymentTypeType,  # (1)
    ErrorDetails: list[ErrorDetailTypeDef],  # (2)
    ErrorMessage: str,
    UpdatedAt: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: DeploymentTypeType](./literals.md#deploymenttypetype) 
2. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBulkDeploymentsResponseTypeDef

```python
# ListBulkDeploymentsResponseTypeDef definition

class ListBulkDeploymentsResponseTypeDef(TypedDict):
    BulkDeployments: list[BulkDeploymentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BulkDeploymentTypeDef](./type_defs.md#bulkdeploymenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConnectivityInfoResponseTypeDef

```python
# GetConnectivityInfoResponseTypeDef definition

class GetConnectivityInfoResponseTypeDef(TypedDict):
    ConnectivityInfo: list[ConnectivityInfoTypeDef],  # (1)
    Message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConnectivityInfoTypeDef](./type_defs.md#connectivityinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConnectivityInfoRequestRequestTypeDef

```python
# UpdateConnectivityInfoRequestRequestTypeDef definition

class UpdateConnectivityInfoRequestRequestTypeDef(TypedDict):
    ThingName: str,
    ConnectivityInfo: NotRequired[Sequence[ConnectivityInfoTypeDef]],  # (1)
```

1. See [:material-code-braces: ConnectivityInfoTypeDef](./type_defs.md#connectivityinfotypedef) 
## ConnectorDefinitionVersionOutputTypeDef

```python
# ConnectorDefinitionVersionOutputTypeDef definition

class ConnectorDefinitionVersionOutputTypeDef(TypedDict):
    Connectors: NotRequired[list[ConnectorOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: ConnectorOutputTypeDef](./type_defs.md#connectoroutputtypedef) 
## CoreDefinitionVersionOutputTypeDef

```python
# CoreDefinitionVersionOutputTypeDef definition

class CoreDefinitionVersionOutputTypeDef(TypedDict):
    Cores: NotRequired[list[CoreTypeDef]],  # (1)
```

1. See [:material-code-braces: CoreTypeDef](./type_defs.md#coretypedef) 
## CoreDefinitionVersionTypeDef

```python
# CoreDefinitionVersionTypeDef definition

class CoreDefinitionVersionTypeDef(TypedDict):
    Cores: NotRequired[Sequence[CoreTypeDef]],  # (1)
```

1. See [:material-code-braces: CoreTypeDef](./type_defs.md#coretypedef) 
## CreateCoreDefinitionVersionRequestRequestTypeDef

```python
# CreateCoreDefinitionVersionRequestRequestTypeDef definition

class CreateCoreDefinitionVersionRequestRequestTypeDef(TypedDict):
    CoreDefinitionId: str,
    AmznClientToken: NotRequired[str],
    Cores: NotRequired[Sequence[CoreTypeDef]],  # (1)
```

1. See [:material-code-braces: CoreTypeDef](./type_defs.md#coretypedef) 
## CreateDeviceDefinitionVersionRequestRequestTypeDef

```python
# CreateDeviceDefinitionVersionRequestRequestTypeDef definition

class CreateDeviceDefinitionVersionRequestRequestTypeDef(TypedDict):
    DeviceDefinitionId: str,
    AmznClientToken: NotRequired[str],
    Devices: NotRequired[Sequence[DeviceTypeDef]],  # (1)
```

1. See [:material-code-braces: DeviceTypeDef](./type_defs.md#devicetypedef) 
## DeviceDefinitionVersionOutputTypeDef

```python
# DeviceDefinitionVersionOutputTypeDef definition

class DeviceDefinitionVersionOutputTypeDef(TypedDict):
    Devices: NotRequired[list[DeviceTypeDef]],  # (1)
```

1. See [:material-code-braces: DeviceTypeDef](./type_defs.md#devicetypedef) 
## DeviceDefinitionVersionTypeDef

```python
# DeviceDefinitionVersionTypeDef definition

class DeviceDefinitionVersionTypeDef(TypedDict):
    Devices: NotRequired[Sequence[DeviceTypeDef]],  # (1)
```

1. See [:material-code-braces: DeviceTypeDef](./type_defs.md#devicetypedef) 
## CreateGroupRequestRequestTypeDef

```python
# CreateGroupRequestRequestTypeDef definition

class CreateGroupRequestRequestTypeDef(TypedDict):
    Name: str,
    AmznClientToken: NotRequired[str],
    InitialVersion: NotRequired[GroupVersionTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: GroupVersionTypeDef](./type_defs.md#groupversiontypedef) 
## GetGroupVersionResponseTypeDef

```python
# GetGroupVersionResponseTypeDef definition

class GetGroupVersionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Definition: GroupVersionTypeDef,  # (1)
    Id: str,
    Version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupVersionTypeDef](./type_defs.md#groupversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLoggerDefinitionVersionRequestRequestTypeDef

```python
# CreateLoggerDefinitionVersionRequestRequestTypeDef definition

class CreateLoggerDefinitionVersionRequestRequestTypeDef(TypedDict):
    LoggerDefinitionId: str,
    AmznClientToken: NotRequired[str],
    Loggers: NotRequired[Sequence[LoggerTypeDef]],  # (1)
```

1. See [:material-code-braces: LoggerTypeDef](./type_defs.md#loggertypedef) 
## LoggerDefinitionVersionOutputTypeDef

```python
# LoggerDefinitionVersionOutputTypeDef definition

class LoggerDefinitionVersionOutputTypeDef(TypedDict):
    Loggers: NotRequired[list[LoggerTypeDef]],  # (1)
```

1. See [:material-code-braces: LoggerTypeDef](./type_defs.md#loggertypedef) 
## LoggerDefinitionVersionTypeDef

```python
# LoggerDefinitionVersionTypeDef definition

class LoggerDefinitionVersionTypeDef(TypedDict):
    Loggers: NotRequired[Sequence[LoggerTypeDef]],  # (1)
```

1. See [:material-code-braces: LoggerTypeDef](./type_defs.md#loggertypedef) 
## CreateSubscriptionDefinitionVersionRequestRequestTypeDef

```python
# CreateSubscriptionDefinitionVersionRequestRequestTypeDef definition

class CreateSubscriptionDefinitionVersionRequestRequestTypeDef(TypedDict):
    SubscriptionDefinitionId: str,
    AmznClientToken: NotRequired[str],
    Subscriptions: NotRequired[Sequence[SubscriptionTypeDef]],  # (1)
```

1. See [:material-code-braces: SubscriptionTypeDef](./type_defs.md#subscriptiontypedef) 
## SubscriptionDefinitionVersionOutputTypeDef

```python
# SubscriptionDefinitionVersionOutputTypeDef definition

class SubscriptionDefinitionVersionOutputTypeDef(TypedDict):
    Subscriptions: NotRequired[list[SubscriptionTypeDef]],  # (1)
```

1. See [:material-code-braces: SubscriptionTypeDef](./type_defs.md#subscriptiontypedef) 
## SubscriptionDefinitionVersionTypeDef

```python
# SubscriptionDefinitionVersionTypeDef definition

class SubscriptionDefinitionVersionTypeDef(TypedDict):
    Subscriptions: NotRequired[Sequence[SubscriptionTypeDef]],  # (1)
```

1. See [:material-code-braces: SubscriptionTypeDef](./type_defs.md#subscriptiontypedef) 
## ListConnectorDefinitionsResponseTypeDef

```python
# ListConnectorDefinitionsResponseTypeDef definition

class ListConnectorDefinitionsResponseTypeDef(TypedDict):
    Definitions: list[DefinitionInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DefinitionInformationTypeDef](./type_defs.md#definitioninformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCoreDefinitionsResponseTypeDef

```python
# ListCoreDefinitionsResponseTypeDef definition

class ListCoreDefinitionsResponseTypeDef(TypedDict):
    Definitions: list[DefinitionInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DefinitionInformationTypeDef](./type_defs.md#definitioninformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeviceDefinitionsResponseTypeDef

```python
# ListDeviceDefinitionsResponseTypeDef definition

class ListDeviceDefinitionsResponseTypeDef(TypedDict):
    Definitions: list[DefinitionInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DefinitionInformationTypeDef](./type_defs.md#definitioninformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFunctionDefinitionsResponseTypeDef

```python
# ListFunctionDefinitionsResponseTypeDef definition

class ListFunctionDefinitionsResponseTypeDef(TypedDict):
    Definitions: list[DefinitionInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DefinitionInformationTypeDef](./type_defs.md#definitioninformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLoggerDefinitionsResponseTypeDef

```python
# ListLoggerDefinitionsResponseTypeDef definition

class ListLoggerDefinitionsResponseTypeDef(TypedDict):
    Definitions: list[DefinitionInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DefinitionInformationTypeDef](./type_defs.md#definitioninformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourceDefinitionsResponseTypeDef

```python
# ListResourceDefinitionsResponseTypeDef definition

class ListResourceDefinitionsResponseTypeDef(TypedDict):
    Definitions: list[DefinitionInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DefinitionInformationTypeDef](./type_defs.md#definitioninformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSubscriptionDefinitionsResponseTypeDef

```python
# ListSubscriptionDefinitionsResponseTypeDef definition

class ListSubscriptionDefinitionsResponseTypeDef(TypedDict):
    Definitions: list[DefinitionInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DefinitionInformationTypeDef](./type_defs.md#definitioninformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeploymentsResponseTypeDef

```python
# ListDeploymentsResponseTypeDef definition

class ListDeploymentsResponseTypeDef(TypedDict):
    Deployments: list[DeploymentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DeploymentTypeDef](./type_defs.md#deploymenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FunctionDefaultExecutionConfigTypeDef

```python
# FunctionDefaultExecutionConfigTypeDef definition

class FunctionDefaultExecutionConfigTypeDef(TypedDict):
    IsolationMode: NotRequired[FunctionIsolationModeType],  # (1)
    RunAs: NotRequired[FunctionRunAsConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: FunctionIsolationModeType](./literals.md#functionisolationmodetype) 
2. See [:material-code-braces: FunctionRunAsConfigTypeDef](./type_defs.md#functionrunasconfigtypedef) 
## FunctionExecutionConfigTypeDef

```python
# FunctionExecutionConfigTypeDef definition

class FunctionExecutionConfigTypeDef(TypedDict):
    IsolationMode: NotRequired[FunctionIsolationModeType],  # (1)
    RunAs: NotRequired[FunctionRunAsConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: FunctionIsolationModeType](./literals.md#functionisolationmodetype) 
2. See [:material-code-braces: FunctionRunAsConfigTypeDef](./type_defs.md#functionrunasconfigtypedef) 
## ListGroupCertificateAuthoritiesResponseTypeDef

```python
# ListGroupCertificateAuthoritiesResponseTypeDef definition

class ListGroupCertificateAuthoritiesResponseTypeDef(TypedDict):
    GroupCertificateAuthorities: list[GroupCertificateAuthorityPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupCertificateAuthorityPropertiesTypeDef](./type_defs.md#groupcertificateauthoritypropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGroupsResponseTypeDef

```python
# ListGroupsResponseTypeDef definition

class ListGroupsResponseTypeDef(TypedDict):
    Groups: list[GroupInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GroupInformationTypeDef](./type_defs.md#groupinformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LocalDeviceResourceDataTypeDef

```python
# LocalDeviceResourceDataTypeDef definition

class LocalDeviceResourceDataTypeDef(TypedDict):
    GroupOwnerSetting: NotRequired[GroupOwnerSettingTypeDef],  # (1)
    SourcePath: NotRequired[str],
```

1. See [:material-code-braces: GroupOwnerSettingTypeDef](./type_defs.md#groupownersettingtypedef) 
## LocalVolumeResourceDataTypeDef

```python
# LocalVolumeResourceDataTypeDef definition

class LocalVolumeResourceDataTypeDef(TypedDict):
    DestinationPath: NotRequired[str],
    GroupOwnerSetting: NotRequired[GroupOwnerSettingTypeDef],  # (1)
    SourcePath: NotRequired[str],
```

1. See [:material-code-braces: GroupOwnerSettingTypeDef](./type_defs.md#groupownersettingtypedef) 
## ListBulkDeploymentDetailedReportsRequestPaginateTypeDef

```python
# ListBulkDeploymentDetailedReportsRequestPaginateTypeDef definition

class ListBulkDeploymentDetailedReportsRequestPaginateTypeDef(TypedDict):
    BulkDeploymentId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBulkDeploymentsRequestPaginateTypeDef

```python
# ListBulkDeploymentsRequestPaginateTypeDef definition

class ListBulkDeploymentsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConnectorDefinitionVersionsRequestPaginateTypeDef

```python
# ListConnectorDefinitionVersionsRequestPaginateTypeDef definition

class ListConnectorDefinitionVersionsRequestPaginateTypeDef(TypedDict):
    ConnectorDefinitionId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConnectorDefinitionsRequestPaginateTypeDef

```python
# ListConnectorDefinitionsRequestPaginateTypeDef definition

class ListConnectorDefinitionsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCoreDefinitionVersionsRequestPaginateTypeDef

```python
# ListCoreDefinitionVersionsRequestPaginateTypeDef definition

class ListCoreDefinitionVersionsRequestPaginateTypeDef(TypedDict):
    CoreDefinitionId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCoreDefinitionsRequestPaginateTypeDef

```python
# ListCoreDefinitionsRequestPaginateTypeDef definition

class ListCoreDefinitionsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDeploymentsRequestPaginateTypeDef

```python
# ListDeploymentsRequestPaginateTypeDef definition

class ListDeploymentsRequestPaginateTypeDef(TypedDict):
    GroupId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDeviceDefinitionVersionsRequestPaginateTypeDef

```python
# ListDeviceDefinitionVersionsRequestPaginateTypeDef definition

class ListDeviceDefinitionVersionsRequestPaginateTypeDef(TypedDict):
    DeviceDefinitionId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDeviceDefinitionsRequestPaginateTypeDef

```python
# ListDeviceDefinitionsRequestPaginateTypeDef definition

class ListDeviceDefinitionsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFunctionDefinitionVersionsRequestPaginateTypeDef

```python
# ListFunctionDefinitionVersionsRequestPaginateTypeDef definition

class ListFunctionDefinitionVersionsRequestPaginateTypeDef(TypedDict):
    FunctionDefinitionId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFunctionDefinitionsRequestPaginateTypeDef

```python
# ListFunctionDefinitionsRequestPaginateTypeDef definition

class ListFunctionDefinitionsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroupVersionsRequestPaginateTypeDef

```python
# ListGroupVersionsRequestPaginateTypeDef definition

class ListGroupVersionsRequestPaginateTypeDef(TypedDict):
    GroupId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroupsRequestPaginateTypeDef

```python
# ListGroupsRequestPaginateTypeDef definition

class ListGroupsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLoggerDefinitionVersionsRequestPaginateTypeDef

```python
# ListLoggerDefinitionVersionsRequestPaginateTypeDef definition

class ListLoggerDefinitionVersionsRequestPaginateTypeDef(TypedDict):
    LoggerDefinitionId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLoggerDefinitionsRequestPaginateTypeDef

```python
# ListLoggerDefinitionsRequestPaginateTypeDef definition

class ListLoggerDefinitionsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourceDefinitionVersionsRequestPaginateTypeDef

```python
# ListResourceDefinitionVersionsRequestPaginateTypeDef definition

class ListResourceDefinitionVersionsRequestPaginateTypeDef(TypedDict):
    ResourceDefinitionId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourceDefinitionsRequestPaginateTypeDef

```python
# ListResourceDefinitionsRequestPaginateTypeDef definition

class ListResourceDefinitionsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSubscriptionDefinitionVersionsRequestPaginateTypeDef

```python
# ListSubscriptionDefinitionVersionsRequestPaginateTypeDef definition

class ListSubscriptionDefinitionVersionsRequestPaginateTypeDef(TypedDict):
    SubscriptionDefinitionId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSubscriptionDefinitionsRequestPaginateTypeDef

```python
# ListSubscriptionDefinitionsRequestPaginateTypeDef definition

class ListSubscriptionDefinitionsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConnectorDefinitionVersionsResponseTypeDef

```python
# ListConnectorDefinitionVersionsResponseTypeDef definition

class ListConnectorDefinitionVersionsResponseTypeDef(TypedDict):
    Versions: list[VersionInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: VersionInformationTypeDef](./type_defs.md#versioninformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCoreDefinitionVersionsResponseTypeDef

```python
# ListCoreDefinitionVersionsResponseTypeDef definition

class ListCoreDefinitionVersionsResponseTypeDef(TypedDict):
    Versions: list[VersionInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: VersionInformationTypeDef](./type_defs.md#versioninformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeviceDefinitionVersionsResponseTypeDef

```python
# ListDeviceDefinitionVersionsResponseTypeDef definition

class ListDeviceDefinitionVersionsResponseTypeDef(TypedDict):
    Versions: list[VersionInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: VersionInformationTypeDef](./type_defs.md#versioninformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFunctionDefinitionVersionsResponseTypeDef

```python
# ListFunctionDefinitionVersionsResponseTypeDef definition

class ListFunctionDefinitionVersionsResponseTypeDef(TypedDict):
    Versions: list[VersionInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: VersionInformationTypeDef](./type_defs.md#versioninformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGroupVersionsResponseTypeDef

```python
# ListGroupVersionsResponseTypeDef definition

class ListGroupVersionsResponseTypeDef(TypedDict):
    Versions: list[VersionInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: VersionInformationTypeDef](./type_defs.md#versioninformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLoggerDefinitionVersionsResponseTypeDef

```python
# ListLoggerDefinitionVersionsResponseTypeDef definition

class ListLoggerDefinitionVersionsResponseTypeDef(TypedDict):
    Versions: list[VersionInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: VersionInformationTypeDef](./type_defs.md#versioninformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourceDefinitionVersionsResponseTypeDef

```python
# ListResourceDefinitionVersionsResponseTypeDef definition

class ListResourceDefinitionVersionsResponseTypeDef(TypedDict):
    Versions: list[VersionInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: VersionInformationTypeDef](./type_defs.md#versioninformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSubscriptionDefinitionVersionsResponseTypeDef

```python
# ListSubscriptionDefinitionVersionsResponseTypeDef definition

class ListSubscriptionDefinitionVersionsResponseTypeDef(TypedDict):
    Versions: list[VersionInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: VersionInformationTypeDef](./type_defs.md#versioninformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## S3MachineLearningModelResourceDataTypeDef

```python
# S3MachineLearningModelResourceDataTypeDef definition

class S3MachineLearningModelResourceDataTypeDef(TypedDict):
    DestinationPath: NotRequired[str],
    OwnerSetting: NotRequired[ResourceDownloadOwnerSettingTypeDef],  # (1)
    S3Uri: NotRequired[str],
```

1. See [:material-code-braces: ResourceDownloadOwnerSettingTypeDef](./type_defs.md#resourcedownloadownersettingtypedef) 
## SageMakerMachineLearningModelResourceDataTypeDef

```python
# SageMakerMachineLearningModelResourceDataTypeDef definition

class SageMakerMachineLearningModelResourceDataTypeDef(TypedDict):
    DestinationPath: NotRequired[str],
    OwnerSetting: NotRequired[ResourceDownloadOwnerSettingTypeDef],  # (1)
    SageMakerJobArn: NotRequired[str],
```

1. See [:material-code-braces: ResourceDownloadOwnerSettingTypeDef](./type_defs.md#resourcedownloadownersettingtypedef) 
## RuntimeConfigurationTypeDef

```python
# RuntimeConfigurationTypeDef definition

class RuntimeConfigurationTypeDef(TypedDict):
    TelemetryConfiguration: NotRequired[TelemetryConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: TelemetryConfigurationTypeDef](./type_defs.md#telemetryconfigurationtypedef) 
## UpdateThingRuntimeConfigurationRequestRequestTypeDef

```python
# UpdateThingRuntimeConfigurationRequestRequestTypeDef definition

class UpdateThingRuntimeConfigurationRequestRequestTypeDef(TypedDict):
    ThingName: str,
    TelemetryConfiguration: NotRequired[TelemetryConfigurationUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: TelemetryConfigurationUpdateTypeDef](./type_defs.md#telemetryconfigurationupdatetypedef) 
## ListBulkDeploymentDetailedReportsResponseTypeDef

```python
# ListBulkDeploymentDetailedReportsResponseTypeDef definition

class ListBulkDeploymentDetailedReportsResponseTypeDef(TypedDict):
    Deployments: list[BulkDeploymentResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BulkDeploymentResultTypeDef](./type_defs.md#bulkdeploymentresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConnectorDefinitionVersionResponseTypeDef

```python
# GetConnectorDefinitionVersionResponseTypeDef definition

class GetConnectorDefinitionVersionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Definition: ConnectorDefinitionVersionOutputTypeDef,  # (1)
    Id: str,
    Version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConnectorDefinitionVersionOutputTypeDef](./type_defs.md#connectordefinitionversionoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConnectorDefinitionVersionTypeDef

```python
# ConnectorDefinitionVersionTypeDef definition

class ConnectorDefinitionVersionTypeDef(TypedDict):
    Connectors: NotRequired[Sequence[ConnectorUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: ConnectorTypeDef](./type_defs.md#connectortypedef) [:material-code-braces: ConnectorOutputTypeDef](./type_defs.md#connectoroutputtypedef) 
## CreateConnectorDefinitionVersionRequestRequestTypeDef

```python
# CreateConnectorDefinitionVersionRequestRequestTypeDef definition

class CreateConnectorDefinitionVersionRequestRequestTypeDef(TypedDict):
    ConnectorDefinitionId: str,
    AmznClientToken: NotRequired[str],
    Connectors: NotRequired[Sequence[ConnectorUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: ConnectorTypeDef](./type_defs.md#connectortypedef) [:material-code-braces: ConnectorOutputTypeDef](./type_defs.md#connectoroutputtypedef) 
## GetCoreDefinitionVersionResponseTypeDef

```python
# GetCoreDefinitionVersionResponseTypeDef definition

class GetCoreDefinitionVersionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Definition: CoreDefinitionVersionOutputTypeDef,  # (1)
    Id: str,
    Version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CoreDefinitionVersionOutputTypeDef](./type_defs.md#coredefinitionversionoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCoreDefinitionRequestRequestTypeDef

```python
# CreateCoreDefinitionRequestRequestTypeDef definition

class CreateCoreDefinitionRequestRequestTypeDef(TypedDict):
    AmznClientToken: NotRequired[str],
    InitialVersion: NotRequired[CoreDefinitionVersionTypeDef],  # (1)
    Name: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: CoreDefinitionVersionTypeDef](./type_defs.md#coredefinitionversiontypedef) 
## GetDeviceDefinitionVersionResponseTypeDef

```python
# GetDeviceDefinitionVersionResponseTypeDef definition

class GetDeviceDefinitionVersionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Definition: DeviceDefinitionVersionOutputTypeDef,  # (1)
    Id: str,
    Version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DeviceDefinitionVersionOutputTypeDef](./type_defs.md#devicedefinitionversionoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDeviceDefinitionRequestRequestTypeDef

```python
# CreateDeviceDefinitionRequestRequestTypeDef definition

class CreateDeviceDefinitionRequestRequestTypeDef(TypedDict):
    AmznClientToken: NotRequired[str],
    InitialVersion: NotRequired[DeviceDefinitionVersionTypeDef],  # (1)
    Name: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DeviceDefinitionVersionTypeDef](./type_defs.md#devicedefinitionversiontypedef) 
## GetLoggerDefinitionVersionResponseTypeDef

```python
# GetLoggerDefinitionVersionResponseTypeDef definition

class GetLoggerDefinitionVersionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Definition: LoggerDefinitionVersionOutputTypeDef,  # (1)
    Id: str,
    Version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggerDefinitionVersionOutputTypeDef](./type_defs.md#loggerdefinitionversionoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLoggerDefinitionRequestRequestTypeDef

```python
# CreateLoggerDefinitionRequestRequestTypeDef definition

class CreateLoggerDefinitionRequestRequestTypeDef(TypedDict):
    AmznClientToken: NotRequired[str],
    InitialVersion: NotRequired[LoggerDefinitionVersionTypeDef],  # (1)
    Name: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: LoggerDefinitionVersionTypeDef](./type_defs.md#loggerdefinitionversiontypedef) 
## GetSubscriptionDefinitionVersionResponseTypeDef

```python
# GetSubscriptionDefinitionVersionResponseTypeDef definition

class GetSubscriptionDefinitionVersionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Definition: SubscriptionDefinitionVersionOutputTypeDef,  # (1)
    Id: str,
    Version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SubscriptionDefinitionVersionOutputTypeDef](./type_defs.md#subscriptiondefinitionversionoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSubscriptionDefinitionRequestRequestTypeDef

```python
# CreateSubscriptionDefinitionRequestRequestTypeDef definition

class CreateSubscriptionDefinitionRequestRequestTypeDef(TypedDict):
    AmznClientToken: NotRequired[str],
    InitialVersion: NotRequired[SubscriptionDefinitionVersionTypeDef],  # (1)
    Name: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: SubscriptionDefinitionVersionTypeDef](./type_defs.md#subscriptiondefinitionversiontypedef) 
## FunctionDefaultConfigTypeDef

```python
# FunctionDefaultConfigTypeDef definition

class FunctionDefaultConfigTypeDef(TypedDict):
    Execution: NotRequired[FunctionDefaultExecutionConfigTypeDef],  # (1)
```

1. See [:material-code-braces: FunctionDefaultExecutionConfigTypeDef](./type_defs.md#functiondefaultexecutionconfigtypedef) 
## FunctionConfigurationEnvironmentOutputTypeDef

```python
# FunctionConfigurationEnvironmentOutputTypeDef definition

class FunctionConfigurationEnvironmentOutputTypeDef(TypedDict):
    AccessSysfs: NotRequired[bool],
    Execution: NotRequired[FunctionExecutionConfigTypeDef],  # (1)
    ResourceAccessPolicies: NotRequired[list[ResourceAccessPolicyTypeDef]],  # (2)
    Variables: NotRequired[dict[str, str]],
```

1. See [:material-code-braces: FunctionExecutionConfigTypeDef](./type_defs.md#functionexecutionconfigtypedef) 
2. See [:material-code-braces: ResourceAccessPolicyTypeDef](./type_defs.md#resourceaccesspolicytypedef) 
## FunctionConfigurationEnvironmentTypeDef

```python
# FunctionConfigurationEnvironmentTypeDef definition

class FunctionConfigurationEnvironmentTypeDef(TypedDict):
    AccessSysfs: NotRequired[bool],
    Execution: NotRequired[FunctionExecutionConfigTypeDef],  # (1)
    ResourceAccessPolicies: NotRequired[Sequence[ResourceAccessPolicyTypeDef]],  # (2)
    Variables: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: FunctionExecutionConfigTypeDef](./type_defs.md#functionexecutionconfigtypedef) 
2. See [:material-code-braces: ResourceAccessPolicyTypeDef](./type_defs.md#resourceaccesspolicytypedef) 
## ResourceDataContainerOutputTypeDef

```python
# ResourceDataContainerOutputTypeDef definition

class ResourceDataContainerOutputTypeDef(TypedDict):
    LocalDeviceResourceData: NotRequired[LocalDeviceResourceDataTypeDef],  # (1)
    LocalVolumeResourceData: NotRequired[LocalVolumeResourceDataTypeDef],  # (2)
    S3MachineLearningModelResourceData: NotRequired[S3MachineLearningModelResourceDataTypeDef],  # (3)
    SageMakerMachineLearningModelResourceData: NotRequired[SageMakerMachineLearningModelResourceDataTypeDef],  # (4)
    SecretsManagerSecretResourceData: NotRequired[SecretsManagerSecretResourceDataOutputTypeDef],  # (5)
```

1. See [:material-code-braces: LocalDeviceResourceDataTypeDef](./type_defs.md#localdeviceresourcedatatypedef) 
2. See [:material-code-braces: LocalVolumeResourceDataTypeDef](./type_defs.md#localvolumeresourcedatatypedef) 
3. See [:material-code-braces: S3MachineLearningModelResourceDataTypeDef](./type_defs.md#s3machinelearningmodelresourcedatatypedef) 
4. See [:material-code-braces: SageMakerMachineLearningModelResourceDataTypeDef](./type_defs.md#sagemakermachinelearningmodelresourcedatatypedef) 
5. See [:material-code-braces: SecretsManagerSecretResourceDataOutputTypeDef](./type_defs.md#secretsmanagersecretresourcedataoutputtypedef) 
## GetThingRuntimeConfigurationResponseTypeDef

```python
# GetThingRuntimeConfigurationResponseTypeDef definition

class GetThingRuntimeConfigurationResponseTypeDef(TypedDict):
    RuntimeConfiguration: RuntimeConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuntimeConfigurationTypeDef](./type_defs.md#runtimeconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResourceDataContainerTypeDef

```python
# ResourceDataContainerTypeDef definition

class ResourceDataContainerTypeDef(TypedDict):
    LocalDeviceResourceData: NotRequired[LocalDeviceResourceDataTypeDef],  # (1)
    LocalVolumeResourceData: NotRequired[LocalVolumeResourceDataTypeDef],  # (2)
    S3MachineLearningModelResourceData: NotRequired[S3MachineLearningModelResourceDataTypeDef],  # (3)
    SageMakerMachineLearningModelResourceData: NotRequired[SageMakerMachineLearningModelResourceDataTypeDef],  # (4)
    SecretsManagerSecretResourceData: NotRequired[SecretsManagerSecretResourceDataUnionTypeDef],  # (5)
```

1. See [:material-code-braces: LocalDeviceResourceDataTypeDef](./type_defs.md#localdeviceresourcedatatypedef) 
2. See [:material-code-braces: LocalVolumeResourceDataTypeDef](./type_defs.md#localvolumeresourcedatatypedef) 
3. See [:material-code-braces: S3MachineLearningModelResourceDataTypeDef](./type_defs.md#s3machinelearningmodelresourcedatatypedef) 
4. See [:material-code-braces: SageMakerMachineLearningModelResourceDataTypeDef](./type_defs.md#sagemakermachinelearningmodelresourcedatatypedef) 
5. See [:material-code-braces: SecretsManagerSecretResourceDataTypeDef](./type_defs.md#secretsmanagersecretresourcedatatypedef) [:material-code-braces: SecretsManagerSecretResourceDataOutputTypeDef](./type_defs.md#secretsmanagersecretresourcedataoutputtypedef) 
## CreateConnectorDefinitionRequestRequestTypeDef

```python
# CreateConnectorDefinitionRequestRequestTypeDef definition

class CreateConnectorDefinitionRequestRequestTypeDef(TypedDict):
    AmznClientToken: NotRequired[str],
    InitialVersion: NotRequired[ConnectorDefinitionVersionTypeDef],  # (1)
    Name: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ConnectorDefinitionVersionTypeDef](./type_defs.md#connectordefinitionversiontypedef) 
## FunctionConfigurationOutputTypeDef

```python
# FunctionConfigurationOutputTypeDef definition

class FunctionConfigurationOutputTypeDef(TypedDict):
    EncodingType: NotRequired[EncodingTypeType],  # (1)
    Environment: NotRequired[FunctionConfigurationEnvironmentOutputTypeDef],  # (2)
    ExecArgs: NotRequired[str],
    Executable: NotRequired[str],
    MemorySize: NotRequired[int],
    Pinned: NotRequired[bool],
    Timeout: NotRequired[int],
    FunctionRuntimeOverride: NotRequired[str],
```

1. See [:material-code-brackets: EncodingTypeType](./literals.md#encodingtypetype) 
2. See [:material-code-braces: FunctionConfigurationEnvironmentOutputTypeDef](./type_defs.md#functionconfigurationenvironmentoutputtypedef) 
## ResourceOutputTypeDef

```python
# ResourceOutputTypeDef definition

class ResourceOutputTypeDef(TypedDict):
    Id: str,
    Name: str,
    ResourceDataContainer: ResourceDataContainerOutputTypeDef,  # (1)
```

1. See [:material-code-braces: ResourceDataContainerOutputTypeDef](./type_defs.md#resourcedatacontaineroutputtypedef) 
## FunctionOutputTypeDef

```python
# FunctionOutputTypeDef definition

class FunctionOutputTypeDef(TypedDict):
    Id: str,
    FunctionArn: NotRequired[str],
    FunctionConfiguration: NotRequired[FunctionConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: FunctionConfigurationOutputTypeDef](./type_defs.md#functionconfigurationoutputtypedef) 
## FunctionConfigurationTypeDef

```python
# FunctionConfigurationTypeDef definition

class FunctionConfigurationTypeDef(TypedDict):
    EncodingType: NotRequired[EncodingTypeType],  # (1)
    Environment: NotRequired[FunctionConfigurationEnvironmentUnionTypeDef],  # (2)
    ExecArgs: NotRequired[str],
    Executable: NotRequired[str],
    MemorySize: NotRequired[int],
    Pinned: NotRequired[bool],
    Timeout: NotRequired[int],
    FunctionRuntimeOverride: NotRequired[str],
```

1. See [:material-code-brackets: EncodingTypeType](./literals.md#encodingtypetype) 
2. See [:material-code-braces: FunctionConfigurationEnvironmentTypeDef](./type_defs.md#functionconfigurationenvironmenttypedef) [:material-code-braces: FunctionConfigurationEnvironmentOutputTypeDef](./type_defs.md#functionconfigurationenvironmentoutputtypedef) 
## ResourceDefinitionVersionOutputTypeDef

```python
# ResourceDefinitionVersionOutputTypeDef definition

class ResourceDefinitionVersionOutputTypeDef(TypedDict):
    Resources: NotRequired[list[ResourceOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef) 
## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    Id: str,
    Name: str,
    ResourceDataContainer: ResourceDataContainerUnionTypeDef,  # (1)
```

1. See [:material-code-braces: ResourceDataContainerTypeDef](./type_defs.md#resourcedatacontainertypedef) [:material-code-braces: ResourceDataContainerOutputTypeDef](./type_defs.md#resourcedatacontaineroutputtypedef) 
## FunctionDefinitionVersionOutputTypeDef

```python
# FunctionDefinitionVersionOutputTypeDef definition

class FunctionDefinitionVersionOutputTypeDef(TypedDict):
    DefaultConfig: NotRequired[FunctionDefaultConfigTypeDef],  # (1)
    Functions: NotRequired[list[FunctionOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: FunctionDefaultConfigTypeDef](./type_defs.md#functiondefaultconfigtypedef) 
2. See [:material-code-braces: FunctionOutputTypeDef](./type_defs.md#functionoutputtypedef) 
## GetResourceDefinitionVersionResponseTypeDef

```python
# GetResourceDefinitionVersionResponseTypeDef definition

class GetResourceDefinitionVersionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Definition: ResourceDefinitionVersionOutputTypeDef,  # (1)
    Id: str,
    Version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceDefinitionVersionOutputTypeDef](./type_defs.md#resourcedefinitionversionoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFunctionDefinitionVersionResponseTypeDef

```python
# GetFunctionDefinitionVersionResponseTypeDef definition

class GetFunctionDefinitionVersionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTimestamp: str,
    Definition: FunctionDefinitionVersionOutputTypeDef,  # (1)
    Id: str,
    Version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FunctionDefinitionVersionOutputTypeDef](./type_defs.md#functiondefinitionversionoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FunctionTypeDef

```python
# FunctionTypeDef definition

class FunctionTypeDef(TypedDict):
    Id: str,
    FunctionArn: NotRequired[str],
    FunctionConfiguration: NotRequired[FunctionConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: FunctionConfigurationTypeDef](./type_defs.md#functionconfigurationtypedef) [:material-code-braces: FunctionConfigurationOutputTypeDef](./type_defs.md#functionconfigurationoutputtypedef) 
## CreateResourceDefinitionVersionRequestRequestTypeDef

```python
# CreateResourceDefinitionVersionRequestRequestTypeDef definition

class CreateResourceDefinitionVersionRequestRequestTypeDef(TypedDict):
    ResourceDefinitionId: str,
    AmznClientToken: NotRequired[str],
    Resources: NotRequired[Sequence[ResourceUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) [:material-code-braces: ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef) 
## ResourceDefinitionVersionTypeDef

```python
# ResourceDefinitionVersionTypeDef definition

class ResourceDefinitionVersionTypeDef(TypedDict):
    Resources: NotRequired[Sequence[ResourceUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) [:material-code-braces: ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef) 
## CreateResourceDefinitionRequestRequestTypeDef

```python
# CreateResourceDefinitionRequestRequestTypeDef definition

class CreateResourceDefinitionRequestRequestTypeDef(TypedDict):
    AmznClientToken: NotRequired[str],
    InitialVersion: NotRequired[ResourceDefinitionVersionTypeDef],  # (1)
    Name: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ResourceDefinitionVersionTypeDef](./type_defs.md#resourcedefinitionversiontypedef) 
## CreateFunctionDefinitionVersionRequestRequestTypeDef

```python
# CreateFunctionDefinitionVersionRequestRequestTypeDef definition

class CreateFunctionDefinitionVersionRequestRequestTypeDef(TypedDict):
    FunctionDefinitionId: str,
    AmznClientToken: NotRequired[str],
    DefaultConfig: NotRequired[FunctionDefaultConfigTypeDef],  # (1)
    Functions: NotRequired[Sequence[FunctionUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: FunctionDefaultConfigTypeDef](./type_defs.md#functiondefaultconfigtypedef) 
2. See [:material-code-braces: FunctionTypeDef](./type_defs.md#functiontypedef) [:material-code-braces: FunctionOutputTypeDef](./type_defs.md#functionoutputtypedef) 
## FunctionDefinitionVersionTypeDef

```python
# FunctionDefinitionVersionTypeDef definition

class FunctionDefinitionVersionTypeDef(TypedDict):
    DefaultConfig: NotRequired[FunctionDefaultConfigTypeDef],  # (1)
    Functions: NotRequired[Sequence[FunctionUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: FunctionDefaultConfigTypeDef](./type_defs.md#functiondefaultconfigtypedef) 
2. See [:material-code-braces: FunctionTypeDef](./type_defs.md#functiontypedef) [:material-code-braces: FunctionOutputTypeDef](./type_defs.md#functionoutputtypedef) 
## CreateFunctionDefinitionRequestRequestTypeDef

```python
# CreateFunctionDefinitionRequestRequestTypeDef definition

class CreateFunctionDefinitionRequestRequestTypeDef(TypedDict):
    AmznClientToken: NotRequired[str],
    InitialVersion: NotRequired[FunctionDefinitionVersionTypeDef],  # (1)
    Name: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: FunctionDefinitionVersionTypeDef](./type_defs.md#functiondefinitionversiontypedef) 