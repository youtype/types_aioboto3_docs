# Type definitions

> [Index](../README.md) > [FSx](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [FSx](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#fsx)
    type annotations stubs module [types-aiobotocore-fsx](https://pypi.org/project/types-aiobotocore-fsx/).

## AutoExportPolicyUnionTypeDef

```python
# AutoExportPolicyUnionTypeDef definition

AutoExportPolicyUnionTypeDef = Union[
    AutoExportPolicyTypeDef,  # (1)
    AutoExportPolicyOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AutoExportPolicyTypeDef](./type_defs.md#autoexportpolicytypedef) 
2. See [:material-code-braces: AutoExportPolicyOutputTypeDef](./type_defs.md#autoexportpolicyoutputtypedef) 

## AutoImportPolicyUnionTypeDef

```python
# AutoImportPolicyUnionTypeDef definition

AutoImportPolicyUnionTypeDef = Union[
    AutoImportPolicyTypeDef,  # (1)
    AutoImportPolicyOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AutoImportPolicyTypeDef](./type_defs.md#autoimportpolicytypedef) 
2. See [:material-code-braces: AutoImportPolicyOutputTypeDef](./type_defs.md#autoimportpolicyoutputtypedef) 

## LustreRootSquashConfigurationUnionTypeDef

```python
# LustreRootSquashConfigurationUnionTypeDef definition

LustreRootSquashConfigurationUnionTypeDef = Union[
    LustreRootSquashConfigurationTypeDef,  # (1)
    LustreRootSquashConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: LustreRootSquashConfigurationTypeDef](./type_defs.md#lustrerootsquashconfigurationtypedef) 
2. See [:material-code-braces: LustreRootSquashConfigurationOutputTypeDef](./type_defs.md#lustrerootsquashconfigurationoutputtypedef) 

## OpenZFSClientConfigurationUnionTypeDef

```python
# OpenZFSClientConfigurationUnionTypeDef definition

OpenZFSClientConfigurationUnionTypeDef = Union[
    OpenZFSClientConfigurationTypeDef,  # (1)
    OpenZFSClientConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OpenZFSClientConfigurationTypeDef](./type_defs.md#openzfsclientconfigurationtypedef) 
2. See [:material-code-braces: OpenZFSClientConfigurationOutputTypeDef](./type_defs.md#openzfsclientconfigurationoutputtypedef) 

## OpenZFSNfsExportUnionTypeDef

```python
# OpenZFSNfsExportUnionTypeDef definition

OpenZFSNfsExportUnionTypeDef = Union[
    OpenZFSNfsExportTypeDef,  # (1)
    OpenZFSNfsExportOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OpenZFSNfsExportTypeDef](./type_defs.md#openzfsnfsexporttypedef) 
2. See [:material-code-braces: OpenZFSNfsExportOutputTypeDef](./type_defs.md#openzfsnfsexportoutputtypedef) 



## ActiveDirectoryBackupAttributesTypeDef

```python
# ActiveDirectoryBackupAttributesTypeDef definition

class ActiveDirectoryBackupAttributesTypeDef(TypedDict):
    DomainName: NotRequired[str],
    ActiveDirectoryId: NotRequired[str],
    ResourceARN: NotRequired[str],
```

## AdministrativeActionFailureDetailsTypeDef

```python
# AdministrativeActionFailureDetailsTypeDef definition

class AdministrativeActionFailureDetailsTypeDef(TypedDict):
    Message: NotRequired[str],
```

## AggregateConfigurationTypeDef

```python
# AggregateConfigurationTypeDef definition

class AggregateConfigurationTypeDef(TypedDict):
    Aggregates: NotRequired[list[str]],
    TotalConstituents: NotRequired[int],
```

## AliasTypeDef

```python
# AliasTypeDef definition

class AliasTypeDef(TypedDict):
    Name: NotRequired[str],
    Lifecycle: NotRequired[AliasLifecycleType],  # (1)
```

1. See [:material-code-brackets: AliasLifecycleType](./literals.md#aliaslifecycletype) 
## AssociateFileSystemAliasesRequestRequestTypeDef

```python
# AssociateFileSystemAliasesRequestRequestTypeDef definition

class AssociateFileSystemAliasesRequestRequestTypeDef(TypedDict):
    FileSystemId: str,
    Aliases: Sequence[str],
    ClientRequestToken: NotRequired[str],
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

## AutoExportPolicyOutputTypeDef

```python
# AutoExportPolicyOutputTypeDef definition

class AutoExportPolicyOutputTypeDef(TypedDict):
    Events: NotRequired[list[EventTypeType]],  # (1)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
## AutoExportPolicyTypeDef

```python
# AutoExportPolicyTypeDef definition

class AutoExportPolicyTypeDef(TypedDict):
    Events: NotRequired[Sequence[EventTypeType]],  # (1)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
## AutoImportPolicyOutputTypeDef

```python
# AutoImportPolicyOutputTypeDef definition

class AutoImportPolicyOutputTypeDef(TypedDict):
    Events: NotRequired[list[EventTypeType]],  # (1)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
## AutoImportPolicyTypeDef

```python
# AutoImportPolicyTypeDef definition

class AutoImportPolicyTypeDef(TypedDict):
    Events: NotRequired[Sequence[EventTypeType]],  # (1)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
## AutocommitPeriodTypeDef

```python
# AutocommitPeriodTypeDef definition

class AutocommitPeriodTypeDef(TypedDict):
    Type: AutocommitPeriodTypeType,  # (1)
    Value: NotRequired[int],
```

1. See [:material-code-brackets: AutocommitPeriodTypeType](./literals.md#autocommitperiodtypetype) 
## BackupFailureDetailsTypeDef

```python
# BackupFailureDetailsTypeDef definition

class BackupFailureDetailsTypeDef(TypedDict):
    Message: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## CancelDataRepositoryTaskRequestRequestTypeDef

```python
# CancelDataRepositoryTaskRequestRequestTypeDef definition

class CancelDataRepositoryTaskRequestRequestTypeDef(TypedDict):
    TaskId: str,
```

## CompletionReportTypeDef

```python
# CompletionReportTypeDef definition

class CompletionReportTypeDef(TypedDict):
    Enabled: bool,
    Path: NotRequired[str],
    Format: NotRequired[ReportFormatType],  # (1)
    Scope: NotRequired[ReportScopeType],  # (2)
```

1. See [:material-code-brackets: ReportFormatType](./literals.md#reportformattype) 
2. See [:material-code-brackets: ReportScopeType](./literals.md#reportscopetype) 
## CopySnapshotAndUpdateVolumeRequestRequestTypeDef

```python
# CopySnapshotAndUpdateVolumeRequestRequestTypeDef definition

class CopySnapshotAndUpdateVolumeRequestRequestTypeDef(TypedDict):
    VolumeId: str,
    SourceSnapshotARN: str,
    ClientRequestToken: NotRequired[str],
    CopyStrategy: NotRequired[OpenZFSCopyStrategyType],  # (1)
    Options: NotRequired[Sequence[UpdateOpenZFSVolumeOptionType]],  # (2)
```

1. See [:material-code-brackets: OpenZFSCopyStrategyType](./literals.md#openzfscopystrategytype) 
2. See [:material-code-brackets: UpdateOpenZFSVolumeOptionType](./literals.md#updateopenzfsvolumeoptiontype) 
## CreateAggregateConfigurationTypeDef

```python
# CreateAggregateConfigurationTypeDef definition

class CreateAggregateConfigurationTypeDef(TypedDict):
    Aggregates: NotRequired[Sequence[str]],
    ConstituentsPerAggregate: NotRequired[int],
```

## FileCacheLustreMetadataConfigurationTypeDef

```python
# FileCacheLustreMetadataConfigurationTypeDef definition

class FileCacheLustreMetadataConfigurationTypeDef(TypedDict):
    StorageCapacity: int,
```

## CreateFileSystemLustreMetadataConfigurationTypeDef

```python
# CreateFileSystemLustreMetadataConfigurationTypeDef definition

class CreateFileSystemLustreMetadataConfigurationTypeDef(TypedDict):
    Mode: MetadataConfigurationModeType,  # (1)
    Iops: NotRequired[int],
```

1. See [:material-code-brackets: MetadataConfigurationModeType](./literals.md#metadataconfigurationmodetype) 
## LustreLogCreateConfigurationTypeDef

```python
# LustreLogCreateConfigurationTypeDef definition

class LustreLogCreateConfigurationTypeDef(TypedDict):
    Level: LustreAccessAuditLogLevelType,  # (1)
    Destination: NotRequired[str],
```

1. See [:material-code-brackets: LustreAccessAuditLogLevelType](./literals.md#lustreaccessauditlogleveltype) 
## DiskIopsConfigurationTypeDef

```python
# DiskIopsConfigurationTypeDef definition

class DiskIopsConfigurationTypeDef(TypedDict):
    Mode: NotRequired[DiskIopsConfigurationModeType],  # (1)
    Iops: NotRequired[int],
```

1. See [:material-code-brackets: DiskIopsConfigurationModeType](./literals.md#diskiopsconfigurationmodetype) 
## OpenZFSReadCacheConfigurationTypeDef

```python
# OpenZFSReadCacheConfigurationTypeDef definition

class OpenZFSReadCacheConfigurationTypeDef(TypedDict):
    SizingMode: NotRequired[OpenZFSReadCacheSizingModeType],  # (1)
    SizeGiB: NotRequired[int],
```

1. See [:material-code-brackets: OpenZFSReadCacheSizingModeType](./literals.md#openzfsreadcachesizingmodetype) 
## SelfManagedActiveDirectoryConfigurationTypeDef

```python
# SelfManagedActiveDirectoryConfigurationTypeDef definition

class SelfManagedActiveDirectoryConfigurationTypeDef(TypedDict):
    DomainName: str,
    UserName: str,
    Password: str,
    DnsIps: Sequence[str],
    OrganizationalUnitDistinguishedName: NotRequired[str],
    FileSystemAdministratorsGroup: NotRequired[str],
```

## WindowsAuditLogCreateConfigurationTypeDef

```python
# WindowsAuditLogCreateConfigurationTypeDef definition

class WindowsAuditLogCreateConfigurationTypeDef(TypedDict):
    FileAccessAuditLogLevel: WindowsAccessAuditLogLevelType,  # (1)
    FileShareAccessAuditLogLevel: WindowsAccessAuditLogLevelType,  # (1)
    AuditLogDestination: NotRequired[str],
```

1. See [:material-code-brackets: WindowsAccessAuditLogLevelType](./literals.md#windowsaccessauditlogleveltype) 
2. See [:material-code-brackets: WindowsAccessAuditLogLevelType](./literals.md#windowsaccessauditlogleveltype) 
## TieringPolicyTypeDef

```python
# TieringPolicyTypeDef definition

class TieringPolicyTypeDef(TypedDict):
    CoolingPeriod: NotRequired[int],
    Name: NotRequired[TieringPolicyNameType],  # (1)
```

1. See [:material-code-brackets: TieringPolicyNameType](./literals.md#tieringpolicynametype) 
## CreateOpenZFSOriginSnapshotConfigurationTypeDef

```python
# CreateOpenZFSOriginSnapshotConfigurationTypeDef definition

class CreateOpenZFSOriginSnapshotConfigurationTypeDef(TypedDict):
    SnapshotARN: str,
    CopyStrategy: OpenZFSCopyStrategyType,  # (1)
```

1. See [:material-code-brackets: OpenZFSCopyStrategyType](./literals.md#openzfscopystrategytype) 
## OpenZFSUserOrGroupQuotaTypeDef

```python
# OpenZFSUserOrGroupQuotaTypeDef definition

class OpenZFSUserOrGroupQuotaTypeDef(TypedDict):
    Type: OpenZFSQuotaTypeType,  # (1)
    Id: int,
    StorageCapacityQuotaGiB: int,
```

1. See [:material-code-brackets: OpenZFSQuotaTypeType](./literals.md#openzfsquotatypetype) 
## DataRepositoryFailureDetailsTypeDef

```python
# DataRepositoryFailureDetailsTypeDef definition

class DataRepositoryFailureDetailsTypeDef(TypedDict):
    Message: NotRequired[str],
```

## DataRepositoryTaskFailureDetailsTypeDef

```python
# DataRepositoryTaskFailureDetailsTypeDef definition

class DataRepositoryTaskFailureDetailsTypeDef(TypedDict):
    Message: NotRequired[str],
```

## DataRepositoryTaskFilterTypeDef

```python
# DataRepositoryTaskFilterTypeDef definition

class DataRepositoryTaskFilterTypeDef(TypedDict):
    Name: NotRequired[DataRepositoryTaskFilterNameType],  # (1)
    Values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: DataRepositoryTaskFilterNameType](./literals.md#datarepositorytaskfilternametype) 
## DataRepositoryTaskStatusTypeDef

```python
# DataRepositoryTaskStatusTypeDef definition

class DataRepositoryTaskStatusTypeDef(TypedDict):
    TotalCount: NotRequired[int],
    SucceededCount: NotRequired[int],
    FailedCount: NotRequired[int],
    LastUpdatedTime: NotRequired[datetime],
    ReleasedCapacity: NotRequired[int],
```

## DeleteBackupRequestRequestTypeDef

```python
# DeleteBackupRequestRequestTypeDef definition

class DeleteBackupRequestRequestTypeDef(TypedDict):
    BackupId: str,
    ClientRequestToken: NotRequired[str],
```

## DeleteDataRepositoryAssociationRequestRequestTypeDef

```python
# DeleteDataRepositoryAssociationRequestRequestTypeDef definition

class DeleteDataRepositoryAssociationRequestRequestTypeDef(TypedDict):
    AssociationId: str,
    ClientRequestToken: NotRequired[str],
    DeleteDataInFileSystem: NotRequired[bool],
```

## DeleteFileCacheRequestRequestTypeDef

```python
# DeleteFileCacheRequestRequestTypeDef definition

class DeleteFileCacheRequestRequestTypeDef(TypedDict):
    FileCacheId: str,
    ClientRequestToken: NotRequired[str],
```

## DeleteSnapshotRequestRequestTypeDef

```python
# DeleteSnapshotRequestRequestTypeDef definition

class DeleteSnapshotRequestRequestTypeDef(TypedDict):
    SnapshotId: str,
    ClientRequestToken: NotRequired[str],
```

## DeleteStorageVirtualMachineRequestRequestTypeDef

```python
# DeleteStorageVirtualMachineRequestRequestTypeDef definition

class DeleteStorageVirtualMachineRequestRequestTypeDef(TypedDict):
    StorageVirtualMachineId: str,
    ClientRequestToken: NotRequired[str],
```

## DeleteVolumeOpenZFSConfigurationTypeDef

```python
# DeleteVolumeOpenZFSConfigurationTypeDef definition

class DeleteVolumeOpenZFSConfigurationTypeDef(TypedDict):
    Options: NotRequired[Sequence[DeleteOpenZFSVolumeOptionType]],  # (1)
```

1. See [:material-code-brackets: DeleteOpenZFSVolumeOptionType](./literals.md#deleteopenzfsvolumeoptiontype) 
## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Name: NotRequired[FilterNameType],  # (1)
    Values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: FilterNameType](./literals.md#filternametype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeFileCachesRequestRequestTypeDef

```python
# DescribeFileCachesRequestRequestTypeDef definition

class DescribeFileCachesRequestRequestTypeDef(TypedDict):
    FileCacheIds: NotRequired[Sequence[str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeFileSystemAliasesRequestRequestTypeDef

```python
# DescribeFileSystemAliasesRequestRequestTypeDef definition

class DescribeFileSystemAliasesRequestRequestTypeDef(TypedDict):
    FileSystemId: str,
    ClientRequestToken: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeFileSystemsRequestRequestTypeDef

```python
# DescribeFileSystemsRequestRequestTypeDef definition

class DescribeFileSystemsRequestRequestTypeDef(TypedDict):
    FileSystemIds: NotRequired[Sequence[str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## SnapshotFilterTypeDef

```python
# SnapshotFilterTypeDef definition

class SnapshotFilterTypeDef(TypedDict):
    Name: NotRequired[SnapshotFilterNameType],  # (1)
    Values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: SnapshotFilterNameType](./literals.md#snapshotfilternametype) 
## StorageVirtualMachineFilterTypeDef

```python
# StorageVirtualMachineFilterTypeDef definition

class StorageVirtualMachineFilterTypeDef(TypedDict):
    Name: NotRequired[StorageVirtualMachineFilterNameType],  # (1)
    Values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: StorageVirtualMachineFilterNameType](./literals.md#storagevirtualmachinefilternametype) 
## VolumeFilterTypeDef

```python
# VolumeFilterTypeDef definition

class VolumeFilterTypeDef(TypedDict):
    Name: NotRequired[VolumeFilterNameType],  # (1)
    Values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: VolumeFilterNameType](./literals.md#volumefilternametype) 
## DisassociateFileSystemAliasesRequestRequestTypeDef

```python
# DisassociateFileSystemAliasesRequestRequestTypeDef definition

class DisassociateFileSystemAliasesRequestRequestTypeDef(TypedDict):
    FileSystemId: str,
    Aliases: Sequence[str],
    ClientRequestToken: NotRequired[str],
```

## DurationSinceLastAccessTypeDef

```python
# DurationSinceLastAccessTypeDef definition

class DurationSinceLastAccessTypeDef(TypedDict):
    Unit: NotRequired[UnitType],  # (1)
    Value: NotRequired[int],
```

1. See [:material-code-brackets: UnitType](./literals.md#unittype) 
## FileCacheFailureDetailsTypeDef

```python
# FileCacheFailureDetailsTypeDef definition

class FileCacheFailureDetailsTypeDef(TypedDict):
    Message: NotRequired[str],
```

## FileCacheNFSConfigurationTypeDef

```python
# FileCacheNFSConfigurationTypeDef definition

class FileCacheNFSConfigurationTypeDef(TypedDict):
    Version: NfsVersionType,  # (1)
    DnsIps: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: NfsVersionType](./literals.md#nfsversiontype) 
## LustreLogConfigurationTypeDef

```python
# LustreLogConfigurationTypeDef definition

class LustreLogConfigurationTypeDef(TypedDict):
    Level: LustreAccessAuditLogLevelType,  # (1)
    Destination: NotRequired[str],
```

1. See [:material-code-brackets: LustreAccessAuditLogLevelType](./literals.md#lustreaccessauditlogleveltype) 
## FileSystemEndpointTypeDef

```python
# FileSystemEndpointTypeDef definition

class FileSystemEndpointTypeDef(TypedDict):
    DNSName: NotRequired[str],
    IpAddresses: NotRequired[list[str]],
```

## FileSystemFailureDetailsTypeDef

```python
# FileSystemFailureDetailsTypeDef definition

class FileSystemFailureDetailsTypeDef(TypedDict):
    Message: NotRequired[str],
```

## FileSystemLustreMetadataConfigurationTypeDef

```python
# FileSystemLustreMetadataConfigurationTypeDef definition

class FileSystemLustreMetadataConfigurationTypeDef(TypedDict):
    Mode: MetadataConfigurationModeType,  # (1)
    Iops: NotRequired[int],
```

1. See [:material-code-brackets: MetadataConfigurationModeType](./literals.md#metadataconfigurationmodetype) 
## LifecycleTransitionReasonTypeDef

```python
# LifecycleTransitionReasonTypeDef definition

class LifecycleTransitionReasonTypeDef(TypedDict):
    Message: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## LustreRootSquashConfigurationOutputTypeDef

```python
# LustreRootSquashConfigurationOutputTypeDef definition

class LustreRootSquashConfigurationOutputTypeDef(TypedDict):
    RootSquash: NotRequired[str],
    NoSquashNids: NotRequired[list[str]],
```

## LustreRootSquashConfigurationTypeDef

```python
# LustreRootSquashConfigurationTypeDef definition

class LustreRootSquashConfigurationTypeDef(TypedDict):
    RootSquash: NotRequired[str],
    NoSquashNids: NotRequired[Sequence[str]],
```

## OpenZFSClientConfigurationOutputTypeDef

```python
# OpenZFSClientConfigurationOutputTypeDef definition

class OpenZFSClientConfigurationOutputTypeDef(TypedDict):
    Clients: str,
    Options: list[str],
```

## OpenZFSClientConfigurationTypeDef

```python
# OpenZFSClientConfigurationTypeDef definition

class OpenZFSClientConfigurationTypeDef(TypedDict):
    Clients: str,
    Options: Sequence[str],
```

## OpenZFSOriginSnapshotConfigurationTypeDef

```python
# OpenZFSOriginSnapshotConfigurationTypeDef definition

class OpenZFSOriginSnapshotConfigurationTypeDef(TypedDict):
    SnapshotARN: NotRequired[str],
    CopyStrategy: NotRequired[OpenZFSCopyStrategyType],  # (1)
```

1. See [:material-code-brackets: OpenZFSCopyStrategyType](./literals.md#openzfscopystrategytype) 
## ReleaseFileSystemNfsV3LocksRequestRequestTypeDef

```python
# ReleaseFileSystemNfsV3LocksRequestRequestTypeDef definition

class ReleaseFileSystemNfsV3LocksRequestRequestTypeDef(TypedDict):
    FileSystemId: str,
    ClientRequestToken: NotRequired[str],
```

## RestoreVolumeFromSnapshotRequestRequestTypeDef

```python
# RestoreVolumeFromSnapshotRequestRequestTypeDef definition

class RestoreVolumeFromSnapshotRequestRequestTypeDef(TypedDict):
    VolumeId: str,
    SnapshotId: str,
    ClientRequestToken: NotRequired[str],
    Options: NotRequired[Sequence[RestoreOpenZFSVolumeOptionType]],  # (1)
```

1. See [:material-code-brackets: RestoreOpenZFSVolumeOptionType](./literals.md#restoreopenzfsvolumeoptiontype) 
## RetentionPeriodTypeDef

```python
# RetentionPeriodTypeDef definition

class RetentionPeriodTypeDef(TypedDict):
    Type: RetentionPeriodTypeType,  # (1)
    Value: NotRequired[int],
```

1. See [:material-code-brackets: RetentionPeriodTypeType](./literals.md#retentionperiodtypetype) 
## SelfManagedActiveDirectoryAttributesTypeDef

```python
# SelfManagedActiveDirectoryAttributesTypeDef definition

class SelfManagedActiveDirectoryAttributesTypeDef(TypedDict):
    DomainName: NotRequired[str],
    OrganizationalUnitDistinguishedName: NotRequired[str],
    FileSystemAdministratorsGroup: NotRequired[str],
    UserName: NotRequired[str],
    DnsIps: NotRequired[list[str]],
```

## SelfManagedActiveDirectoryConfigurationUpdatesTypeDef

```python
# SelfManagedActiveDirectoryConfigurationUpdatesTypeDef definition

class SelfManagedActiveDirectoryConfigurationUpdatesTypeDef(TypedDict):
    UserName: NotRequired[str],
    Password: NotRequired[str],
    DnsIps: NotRequired[Sequence[str]],
    DomainName: NotRequired[str],
    OrganizationalUnitDistinguishedName: NotRequired[str],
    FileSystemAdministratorsGroup: NotRequired[str],
```

## StartMisconfiguredStateRecoveryRequestRequestTypeDef

```python
# StartMisconfiguredStateRecoveryRequestRequestTypeDef definition

class StartMisconfiguredStateRecoveryRequestRequestTypeDef(TypedDict):
    FileSystemId: str,
    ClientRequestToken: NotRequired[str],
```

## SvmEndpointTypeDef

```python
# SvmEndpointTypeDef definition

class SvmEndpointTypeDef(TypedDict):
    DNSName: NotRequired[str],
    IpAddresses: NotRequired[list[str]],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## UpdateFileCacheLustreConfigurationTypeDef

```python
# UpdateFileCacheLustreConfigurationTypeDef definition

class UpdateFileCacheLustreConfigurationTypeDef(TypedDict):
    WeeklyMaintenanceStartTime: NotRequired[str],
```

## UpdateFileSystemLustreMetadataConfigurationTypeDef

```python
# UpdateFileSystemLustreMetadataConfigurationTypeDef definition

class UpdateFileSystemLustreMetadataConfigurationTypeDef(TypedDict):
    Iops: NotRequired[int],
    Mode: NotRequired[MetadataConfigurationModeType],  # (1)
```

1. See [:material-code-brackets: MetadataConfigurationModeType](./literals.md#metadataconfigurationmodetype) 
## UpdateSharedVpcConfigurationRequestRequestTypeDef

```python
# UpdateSharedVpcConfigurationRequestRequestTypeDef definition

class UpdateSharedVpcConfigurationRequestRequestTypeDef(TypedDict):
    EnableFsxRouteTableUpdatesFromParticipantAccounts: NotRequired[str],
    ClientRequestToken: NotRequired[str],
```

## UpdateSnapshotRequestRequestTypeDef

```python
# UpdateSnapshotRequestRequestTypeDef definition

class UpdateSnapshotRequestRequestTypeDef(TypedDict):
    Name: str,
    SnapshotId: str,
    ClientRequestToken: NotRequired[str],
```

## WindowsAuditLogConfigurationTypeDef

```python
# WindowsAuditLogConfigurationTypeDef definition

class WindowsAuditLogConfigurationTypeDef(TypedDict):
    FileAccessAuditLogLevel: WindowsAccessAuditLogLevelType,  # (1)
    FileShareAccessAuditLogLevel: WindowsAccessAuditLogLevelType,  # (1)
    AuditLogDestination: NotRequired[str],
```

1. See [:material-code-brackets: WindowsAccessAuditLogLevelType](./literals.md#windowsaccessauditlogleveltype) 
2. See [:material-code-brackets: WindowsAccessAuditLogLevelType](./literals.md#windowsaccessauditlogleveltype) 
## AssociateFileSystemAliasesResponseTypeDef

```python
# AssociateFileSystemAliasesResponseTypeDef definition

class AssociateFileSystemAliasesResponseTypeDef(TypedDict):
    Aliases: list[AliasTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AliasTypeDef](./type_defs.md#aliastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelDataRepositoryTaskResponseTypeDef

```python
# CancelDataRepositoryTaskResponseTypeDef definition

class CancelDataRepositoryTaskResponseTypeDef(TypedDict):
    Lifecycle: DataRepositoryTaskLifecycleType,  # (1)
    TaskId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DataRepositoryTaskLifecycleType](./literals.md#datarepositorytasklifecycletype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBackupResponseTypeDef

```python
# DeleteBackupResponseTypeDef definition

class DeleteBackupResponseTypeDef(TypedDict):
    BackupId: str,
    Lifecycle: BackupLifecycleType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: BackupLifecycleType](./literals.md#backuplifecycletype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDataRepositoryAssociationResponseTypeDef

```python
# DeleteDataRepositoryAssociationResponseTypeDef definition

class DeleteDataRepositoryAssociationResponseTypeDef(TypedDict):
    AssociationId: str,
    Lifecycle: DataRepositoryLifecycleType,  # (1)
    DeleteDataInFileSystem: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DataRepositoryLifecycleType](./literals.md#datarepositorylifecycletype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteFileCacheResponseTypeDef

```python
# DeleteFileCacheResponseTypeDef definition

class DeleteFileCacheResponseTypeDef(TypedDict):
    FileCacheId: str,
    Lifecycle: FileCacheLifecycleType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: FileCacheLifecycleType](./literals.md#filecachelifecycletype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSnapshotResponseTypeDef

```python
# DeleteSnapshotResponseTypeDef definition

class DeleteSnapshotResponseTypeDef(TypedDict):
    SnapshotId: str,
    Lifecycle: SnapshotLifecycleType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: SnapshotLifecycleType](./literals.md#snapshotlifecycletype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteStorageVirtualMachineResponseTypeDef

```python
# DeleteStorageVirtualMachineResponseTypeDef definition

class DeleteStorageVirtualMachineResponseTypeDef(TypedDict):
    StorageVirtualMachineId: str,
    Lifecycle: StorageVirtualMachineLifecycleType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StorageVirtualMachineLifecycleType](./literals.md#storagevirtualmachinelifecycletype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFileSystemAliasesResponseTypeDef

```python
# DescribeFileSystemAliasesResponseTypeDef definition

class DescribeFileSystemAliasesResponseTypeDef(TypedDict):
    Aliases: list[AliasTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AliasTypeDef](./type_defs.md#aliastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSharedVpcConfigurationResponseTypeDef

```python
# DescribeSharedVpcConfigurationResponseTypeDef definition

class DescribeSharedVpcConfigurationResponseTypeDef(TypedDict):
    EnableFsxRouteTableUpdatesFromParticipantAccounts: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateFileSystemAliasesResponseTypeDef

```python
# DisassociateFileSystemAliasesResponseTypeDef definition

class DisassociateFileSystemAliasesResponseTypeDef(TypedDict):
    Aliases: list[AliasTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AliasTypeDef](./type_defs.md#aliastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSharedVpcConfigurationResponseTypeDef

```python
# UpdateSharedVpcConfigurationResponseTypeDef definition

class UpdateSharedVpcConfigurationResponseTypeDef(TypedDict):
    EnableFsxRouteTableUpdatesFromParticipantAccounts: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NFSDataRepositoryConfigurationTypeDef

```python
# NFSDataRepositoryConfigurationTypeDef definition

class NFSDataRepositoryConfigurationTypeDef(TypedDict):
    Version: NfsVersionType,  # (1)
    DnsIps: NotRequired[list[str]],
    AutoExportPolicy: NotRequired[AutoExportPolicyOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: NfsVersionType](./literals.md#nfsversiontype) 
2. See [:material-code-braces: AutoExportPolicyOutputTypeDef](./type_defs.md#autoexportpolicyoutputtypedef) 
## S3DataRepositoryConfigurationOutputTypeDef

```python
# S3DataRepositoryConfigurationOutputTypeDef definition

class S3DataRepositoryConfigurationOutputTypeDef(TypedDict):
    AutoImportPolicy: NotRequired[AutoImportPolicyOutputTypeDef],  # (1)
    AutoExportPolicy: NotRequired[AutoExportPolicyOutputTypeDef],  # (2)
```

1. See [:material-code-braces: AutoImportPolicyOutputTypeDef](./type_defs.md#autoimportpolicyoutputtypedef) 
2. See [:material-code-braces: AutoExportPolicyOutputTypeDef](./type_defs.md#autoexportpolicyoutputtypedef) 
## CopyBackupRequestRequestTypeDef

```python
# CopyBackupRequestRequestTypeDef definition

class CopyBackupRequestRequestTypeDef(TypedDict):
    SourceBackupId: str,
    ClientRequestToken: NotRequired[str],
    SourceRegion: NotRequired[str],
    KmsKeyId: NotRequired[str],
    CopyTags: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateBackupRequestRequestTypeDef

```python
# CreateBackupRequestRequestTypeDef definition

class CreateBackupRequestRequestTypeDef(TypedDict):
    FileSystemId: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    VolumeId: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateSnapshotRequestRequestTypeDef

```python
# CreateSnapshotRequestRequestTypeDef definition

class CreateSnapshotRequestRequestTypeDef(TypedDict):
    Name: str,
    VolumeId: str,
    ClientRequestToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DeleteFileSystemLustreConfigurationTypeDef

```python
# DeleteFileSystemLustreConfigurationTypeDef definition

class DeleteFileSystemLustreConfigurationTypeDef(TypedDict):
    SkipFinalBackup: NotRequired[bool],
    FinalBackupTags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DeleteFileSystemLustreResponseTypeDef

```python
# DeleteFileSystemLustreResponseTypeDef definition

class DeleteFileSystemLustreResponseTypeDef(TypedDict):
    FinalBackupId: NotRequired[str],
    FinalBackupTags: NotRequired[list[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DeleteFileSystemOpenZFSConfigurationTypeDef

```python
# DeleteFileSystemOpenZFSConfigurationTypeDef definition

class DeleteFileSystemOpenZFSConfigurationTypeDef(TypedDict):
    SkipFinalBackup: NotRequired[bool],
    FinalBackupTags: NotRequired[Sequence[TagTypeDef]],  # (1)
    Options: NotRequired[Sequence[DeleteFileSystemOpenZFSOptionType]],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-brackets: DeleteFileSystemOpenZFSOptionType](./literals.md#deletefilesystemopenzfsoptiontype) 
## DeleteFileSystemOpenZFSResponseTypeDef

```python
# DeleteFileSystemOpenZFSResponseTypeDef definition

class DeleteFileSystemOpenZFSResponseTypeDef(TypedDict):
    FinalBackupId: NotRequired[str],
    FinalBackupTags: NotRequired[list[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DeleteFileSystemWindowsConfigurationTypeDef

```python
# DeleteFileSystemWindowsConfigurationTypeDef definition

class DeleteFileSystemWindowsConfigurationTypeDef(TypedDict):
    SkipFinalBackup: NotRequired[bool],
    FinalBackupTags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DeleteFileSystemWindowsResponseTypeDef

```python
# DeleteFileSystemWindowsResponseTypeDef definition

class DeleteFileSystemWindowsResponseTypeDef(TypedDict):
    FinalBackupId: NotRequired[str],
    FinalBackupTags: NotRequired[list[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DeleteVolumeOntapConfigurationTypeDef

```python
# DeleteVolumeOntapConfigurationTypeDef definition

class DeleteVolumeOntapConfigurationTypeDef(TypedDict):
    SkipFinalBackup: NotRequired[bool],
    FinalBackupTags: NotRequired[Sequence[TagTypeDef]],  # (1)
    BypassSnaplockEnterpriseRetention: NotRequired[bool],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DeleteVolumeOntapResponseTypeDef

```python
# DeleteVolumeOntapResponseTypeDef definition

class DeleteVolumeOntapResponseTypeDef(TypedDict):
    FinalBackupId: NotRequired[str],
    FinalBackupTags: NotRequired[list[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: list[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateFileCacheLustreConfigurationTypeDef

```python
# CreateFileCacheLustreConfigurationTypeDef definition

class CreateFileCacheLustreConfigurationTypeDef(TypedDict):
    PerUnitStorageThroughput: int,
    DeploymentType: FileCacheLustreDeploymentTypeType,  # (1)
    MetadataConfiguration: FileCacheLustreMetadataConfigurationTypeDef,  # (2)
    WeeklyMaintenanceStartTime: NotRequired[str],
```

1. See [:material-code-brackets: FileCacheLustreDeploymentTypeType](./literals.md#filecachelustredeploymenttypetype) 
2. See [:material-code-braces: FileCacheLustreMetadataConfigurationTypeDef](./type_defs.md#filecachelustremetadataconfigurationtypedef) 
## CreateFileSystemOntapConfigurationTypeDef

```python
# CreateFileSystemOntapConfigurationTypeDef definition

class CreateFileSystemOntapConfigurationTypeDef(TypedDict):
    DeploymentType: OntapDeploymentTypeType,  # (1)
    AutomaticBackupRetentionDays: NotRequired[int],
    DailyAutomaticBackupStartTime: NotRequired[str],
    EndpointIpAddressRange: NotRequired[str],
    FsxAdminPassword: NotRequired[str],
    DiskIopsConfiguration: NotRequired[DiskIopsConfigurationTypeDef],  # (2)
    PreferredSubnetId: NotRequired[str],
    RouteTableIds: NotRequired[Sequence[str]],
    ThroughputCapacity: NotRequired[int],
    WeeklyMaintenanceStartTime: NotRequired[str],
    HAPairs: NotRequired[int],
    ThroughputCapacityPerHAPair: NotRequired[int],
```

1. See [:material-code-brackets: OntapDeploymentTypeType](./literals.md#ontapdeploymenttypetype) 
2. See [:material-code-braces: DiskIopsConfigurationTypeDef](./type_defs.md#diskiopsconfigurationtypedef) 
## UpdateFileSystemOntapConfigurationTypeDef

```python
# UpdateFileSystemOntapConfigurationTypeDef definition

class UpdateFileSystemOntapConfigurationTypeDef(TypedDict):
    AutomaticBackupRetentionDays: NotRequired[int],
    DailyAutomaticBackupStartTime: NotRequired[str],
    FsxAdminPassword: NotRequired[str],
    WeeklyMaintenanceStartTime: NotRequired[str],
    DiskIopsConfiguration: NotRequired[DiskIopsConfigurationTypeDef],  # (1)
    ThroughputCapacity: NotRequired[int],
    AddRouteTableIds: NotRequired[Sequence[str]],
    RemoveRouteTableIds: NotRequired[Sequence[str]],
    ThroughputCapacityPerHAPair: NotRequired[int],
    HAPairs: NotRequired[int],
```

1. See [:material-code-braces: DiskIopsConfigurationTypeDef](./type_defs.md#diskiopsconfigurationtypedef) 
## OpenZFSFileSystemConfigurationTypeDef

```python
# OpenZFSFileSystemConfigurationTypeDef definition

class OpenZFSFileSystemConfigurationTypeDef(TypedDict):
    AutomaticBackupRetentionDays: NotRequired[int],
    CopyTagsToBackups: NotRequired[bool],
    CopyTagsToVolumes: NotRequired[bool],
    DailyAutomaticBackupStartTime: NotRequired[str],
    DeploymentType: NotRequired[OpenZFSDeploymentTypeType],  # (1)
    ThroughputCapacity: NotRequired[int],
    WeeklyMaintenanceStartTime: NotRequired[str],
    DiskIopsConfiguration: NotRequired[DiskIopsConfigurationTypeDef],  # (2)
    RootVolumeId: NotRequired[str],
    PreferredSubnetId: NotRequired[str],
    EndpointIpAddressRange: NotRequired[str],
    RouteTableIds: NotRequired[list[str]],
    EndpointIpAddress: NotRequired[str],
    ReadCacheConfiguration: NotRequired[OpenZFSReadCacheConfigurationTypeDef],  # (3)
```

1. See [:material-code-brackets: OpenZFSDeploymentTypeType](./literals.md#openzfsdeploymenttypetype) 
2. See [:material-code-braces: DiskIopsConfigurationTypeDef](./type_defs.md#diskiopsconfigurationtypedef) 
3. See [:material-code-braces: OpenZFSReadCacheConfigurationTypeDef](./type_defs.md#openzfsreadcacheconfigurationtypedef) 
## UpdateFileSystemOpenZFSConfigurationTypeDef

```python
# UpdateFileSystemOpenZFSConfigurationTypeDef definition

class UpdateFileSystemOpenZFSConfigurationTypeDef(TypedDict):
    AutomaticBackupRetentionDays: NotRequired[int],
    CopyTagsToBackups: NotRequired[bool],
    CopyTagsToVolumes: NotRequired[bool],
    DailyAutomaticBackupStartTime: NotRequired[str],
    ThroughputCapacity: NotRequired[int],
    WeeklyMaintenanceStartTime: NotRequired[str],
    DiskIopsConfiguration: NotRequired[DiskIopsConfigurationTypeDef],  # (1)
    AddRouteTableIds: NotRequired[Sequence[str]],
    RemoveRouteTableIds: NotRequired[Sequence[str]],
    ReadCacheConfiguration: NotRequired[OpenZFSReadCacheConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: DiskIopsConfigurationTypeDef](./type_defs.md#diskiopsconfigurationtypedef) 
2. See [:material-code-braces: OpenZFSReadCacheConfigurationTypeDef](./type_defs.md#openzfsreadcacheconfigurationtypedef) 
## CreateSvmActiveDirectoryConfigurationTypeDef

```python
# CreateSvmActiveDirectoryConfigurationTypeDef definition

class CreateSvmActiveDirectoryConfigurationTypeDef(TypedDict):
    NetBiosName: str,
    SelfManagedActiveDirectoryConfiguration: NotRequired[SelfManagedActiveDirectoryConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: SelfManagedActiveDirectoryConfigurationTypeDef](./type_defs.md#selfmanagedactivedirectoryconfigurationtypedef) 
## CreateFileSystemWindowsConfigurationTypeDef

```python
# CreateFileSystemWindowsConfigurationTypeDef definition

class CreateFileSystemWindowsConfigurationTypeDef(TypedDict):
    ThroughputCapacity: int,
    ActiveDirectoryId: NotRequired[str],
    SelfManagedActiveDirectoryConfiguration: NotRequired[SelfManagedActiveDirectoryConfigurationTypeDef],  # (1)
    DeploymentType: NotRequired[WindowsDeploymentTypeType],  # (2)
    PreferredSubnetId: NotRequired[str],
    WeeklyMaintenanceStartTime: NotRequired[str],
    DailyAutomaticBackupStartTime: NotRequired[str],
    AutomaticBackupRetentionDays: NotRequired[int],
    CopyTagsToBackups: NotRequired[bool],
    Aliases: NotRequired[Sequence[str]],
    AuditLogConfiguration: NotRequired[WindowsAuditLogCreateConfigurationTypeDef],  # (3)
    DiskIopsConfiguration: NotRequired[DiskIopsConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: SelfManagedActiveDirectoryConfigurationTypeDef](./type_defs.md#selfmanagedactivedirectoryconfigurationtypedef) 
2. See [:material-code-brackets: WindowsDeploymentTypeType](./literals.md#windowsdeploymenttypetype) 
3. See [:material-code-braces: WindowsAuditLogCreateConfigurationTypeDef](./type_defs.md#windowsauditlogcreateconfigurationtypedef) 
4. See [:material-code-braces: DiskIopsConfigurationTypeDef](./type_defs.md#diskiopsconfigurationtypedef) 
## DataRepositoryConfigurationTypeDef

```python
# DataRepositoryConfigurationTypeDef definition

class DataRepositoryConfigurationTypeDef(TypedDict):
    Lifecycle: NotRequired[DataRepositoryLifecycleType],  # (1)
    ImportPath: NotRequired[str],
    ExportPath: NotRequired[str],
    ImportedFileChunkSize: NotRequired[int],
    AutoImportPolicy: NotRequired[AutoImportPolicyTypeType],  # (2)
    FailureDetails: NotRequired[DataRepositoryFailureDetailsTypeDef],  # (3)
```

1. See [:material-code-brackets: DataRepositoryLifecycleType](./literals.md#datarepositorylifecycletype) 
2. See [:material-code-brackets: AutoImportPolicyTypeType](./literals.md#autoimportpolicytypetype) 
3. See [:material-code-braces: DataRepositoryFailureDetailsTypeDef](./type_defs.md#datarepositoryfailuredetailstypedef) 
## DescribeDataRepositoryTasksRequestRequestTypeDef

```python
# DescribeDataRepositoryTasksRequestRequestTypeDef definition

class DescribeDataRepositoryTasksRequestRequestTypeDef(TypedDict):
    TaskIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[DataRepositoryTaskFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DataRepositoryTaskFilterTypeDef](./type_defs.md#datarepositorytaskfiltertypedef) 
## DescribeBackupsRequestRequestTypeDef

```python
# DescribeBackupsRequestRequestTypeDef definition

class DescribeBackupsRequestRequestTypeDef(TypedDict):
    BackupIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeDataRepositoryAssociationsRequestRequestTypeDef

```python
# DescribeDataRepositoryAssociationsRequestRequestTypeDef definition

class DescribeDataRepositoryAssociationsRequestRequestTypeDef(TypedDict):
    AssociationIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeBackupsRequestPaginateTypeDef

```python
# DescribeBackupsRequestPaginateTypeDef definition

class DescribeBackupsRequestPaginateTypeDef(TypedDict):
    BackupIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeFileSystemsRequestPaginateTypeDef

```python
# DescribeFileSystemsRequestPaginateTypeDef definition

class DescribeFileSystemsRequestPaginateTypeDef(TypedDict):
    FileSystemIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceRequestPaginateTypeDef

```python
# ListTagsForResourceRequestPaginateTypeDef definition

class ListTagsForResourceRequestPaginateTypeDef(TypedDict):
    ResourceARN: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSnapshotsRequestRequestTypeDef

```python
# DescribeSnapshotsRequestRequestTypeDef definition

class DescribeSnapshotsRequestRequestTypeDef(TypedDict):
    SnapshotIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[SnapshotFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    IncludeShared: NotRequired[bool],
```

1. See [:material-code-braces: SnapshotFilterTypeDef](./type_defs.md#snapshotfiltertypedef) 
## DescribeStorageVirtualMachinesRequestPaginateTypeDef

```python
# DescribeStorageVirtualMachinesRequestPaginateTypeDef definition

class DescribeStorageVirtualMachinesRequestPaginateTypeDef(TypedDict):
    StorageVirtualMachineIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[StorageVirtualMachineFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: StorageVirtualMachineFilterTypeDef](./type_defs.md#storagevirtualmachinefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeStorageVirtualMachinesRequestRequestTypeDef

```python
# DescribeStorageVirtualMachinesRequestRequestTypeDef definition

class DescribeStorageVirtualMachinesRequestRequestTypeDef(TypedDict):
    StorageVirtualMachineIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[StorageVirtualMachineFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: StorageVirtualMachineFilterTypeDef](./type_defs.md#storagevirtualmachinefiltertypedef) 
## DescribeVolumesRequestPaginateTypeDef

```python
# DescribeVolumesRequestPaginateTypeDef definition

class DescribeVolumesRequestPaginateTypeDef(TypedDict):
    VolumeIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[VolumeFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: VolumeFilterTypeDef](./type_defs.md#volumefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeVolumesRequestRequestTypeDef

```python
# DescribeVolumesRequestRequestTypeDef definition

class DescribeVolumesRequestRequestTypeDef(TypedDict):
    VolumeIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[VolumeFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: VolumeFilterTypeDef](./type_defs.md#volumefiltertypedef) 
## ReleaseConfigurationTypeDef

```python
# ReleaseConfigurationTypeDef definition

class ReleaseConfigurationTypeDef(TypedDict):
    DurationSinceLastAccess: NotRequired[DurationSinceLastAccessTypeDef],  # (1)
```

1. See [:material-code-braces: DurationSinceLastAccessTypeDef](./type_defs.md#durationsincelastaccesstypedef) 
## FileCacheDataRepositoryAssociationTypeDef

```python
# FileCacheDataRepositoryAssociationTypeDef definition

class FileCacheDataRepositoryAssociationTypeDef(TypedDict):
    FileCachePath: str,
    DataRepositoryPath: str,
    DataRepositorySubdirectories: NotRequired[Sequence[str]],
    NFS: NotRequired[FileCacheNFSConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: FileCacheNFSConfigurationTypeDef](./type_defs.md#filecachenfsconfigurationtypedef) 
## FileCacheLustreConfigurationTypeDef

```python
# FileCacheLustreConfigurationTypeDef definition

class FileCacheLustreConfigurationTypeDef(TypedDict):
    PerUnitStorageThroughput: NotRequired[int],
    DeploymentType: NotRequired[FileCacheLustreDeploymentTypeType],  # (1)
    MountName: NotRequired[str],
    WeeklyMaintenanceStartTime: NotRequired[str],
    MetadataConfiguration: NotRequired[FileCacheLustreMetadataConfigurationTypeDef],  # (2)
    LogConfiguration: NotRequired[LustreLogConfigurationTypeDef],  # (3)
```

1. See [:material-code-brackets: FileCacheLustreDeploymentTypeType](./literals.md#filecachelustredeploymenttypetype) 
2. See [:material-code-braces: FileCacheLustreMetadataConfigurationTypeDef](./type_defs.md#filecachelustremetadataconfigurationtypedef) 
3. See [:material-code-braces: LustreLogConfigurationTypeDef](./type_defs.md#lustrelogconfigurationtypedef) 
## FileSystemEndpointsTypeDef

```python
# FileSystemEndpointsTypeDef definition

class FileSystemEndpointsTypeDef(TypedDict):
    Intercluster: NotRequired[FileSystemEndpointTypeDef],  # (1)
    Management: NotRequired[FileSystemEndpointTypeDef],  # (1)
```

1. See [:material-code-braces: FileSystemEndpointTypeDef](./type_defs.md#filesystemendpointtypedef) 
2. See [:material-code-braces: FileSystemEndpointTypeDef](./type_defs.md#filesystemendpointtypedef) 
## SnapshotPaginatorTypeDef

```python
# SnapshotPaginatorTypeDef definition

class SnapshotPaginatorTypeDef(TypedDict):
    ResourceARN: NotRequired[str],
    SnapshotId: NotRequired[str],
    Name: NotRequired[str],
    VolumeId: NotRequired[str],
    CreationTime: NotRequired[datetime],
    Lifecycle: NotRequired[SnapshotLifecycleType],  # (1)
    LifecycleTransitionReason: NotRequired[LifecycleTransitionReasonTypeDef],  # (2)
    Tags: NotRequired[list[TagTypeDef]],  # (3)
    AdministrativeActions: NotRequired[list[dict[str, Any]]],
```

1. See [:material-code-brackets: SnapshotLifecycleType](./literals.md#snapshotlifecycletype) 
2. See [:material-code-braces: LifecycleTransitionReasonTypeDef](./type_defs.md#lifecycletransitionreasontypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## SnapshotTypeDef

```python
# SnapshotTypeDef definition

class SnapshotTypeDef(TypedDict):
    ResourceARN: NotRequired[str],
    SnapshotId: NotRequired[str],
    Name: NotRequired[str],
    VolumeId: NotRequired[str],
    CreationTime: NotRequired[datetime],
    Lifecycle: NotRequired[SnapshotLifecycleType],  # (1)
    LifecycleTransitionReason: NotRequired[LifecycleTransitionReasonTypeDef],  # (2)
    Tags: NotRequired[list[TagTypeDef]],  # (3)
    AdministrativeActions: NotRequired[list[dict[str, Any]]],
```

1. See [:material-code-brackets: SnapshotLifecycleType](./literals.md#snapshotlifecycletype) 
2. See [:material-code-braces: LifecycleTransitionReasonTypeDef](./type_defs.md#lifecycletransitionreasontypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## OpenZFSNfsExportOutputTypeDef

```python
# OpenZFSNfsExportOutputTypeDef definition

class OpenZFSNfsExportOutputTypeDef(TypedDict):
    ClientConfigurations: list[OpenZFSClientConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: OpenZFSClientConfigurationOutputTypeDef](./type_defs.md#openzfsclientconfigurationoutputtypedef) 
## SnaplockRetentionPeriodTypeDef

```python
# SnaplockRetentionPeriodTypeDef definition

class SnaplockRetentionPeriodTypeDef(TypedDict):
    DefaultRetention: RetentionPeriodTypeDef,  # (1)
    MinimumRetention: RetentionPeriodTypeDef,  # (1)
    MaximumRetention: RetentionPeriodTypeDef,  # (1)
```

1. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
2. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
3. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
## SvmActiveDirectoryConfigurationTypeDef

```python
# SvmActiveDirectoryConfigurationTypeDef definition

class SvmActiveDirectoryConfigurationTypeDef(TypedDict):
    NetBiosName: NotRequired[str],
    SelfManagedActiveDirectoryConfiguration: NotRequired[SelfManagedActiveDirectoryAttributesTypeDef],  # (1)
```

1. See [:material-code-braces: SelfManagedActiveDirectoryAttributesTypeDef](./type_defs.md#selfmanagedactivedirectoryattributestypedef) 
## UpdateFileSystemWindowsConfigurationTypeDef

```python
# UpdateFileSystemWindowsConfigurationTypeDef definition

class UpdateFileSystemWindowsConfigurationTypeDef(TypedDict):
    WeeklyMaintenanceStartTime: NotRequired[str],
    DailyAutomaticBackupStartTime: NotRequired[str],
    AutomaticBackupRetentionDays: NotRequired[int],
    ThroughputCapacity: NotRequired[int],
    SelfManagedActiveDirectoryConfiguration: NotRequired[SelfManagedActiveDirectoryConfigurationUpdatesTypeDef],  # (1)
    AuditLogConfiguration: NotRequired[WindowsAuditLogCreateConfigurationTypeDef],  # (2)
    DiskIopsConfiguration: NotRequired[DiskIopsConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: SelfManagedActiveDirectoryConfigurationUpdatesTypeDef](./type_defs.md#selfmanagedactivedirectoryconfigurationupdatestypedef) 
2. See [:material-code-braces: WindowsAuditLogCreateConfigurationTypeDef](./type_defs.md#windowsauditlogcreateconfigurationtypedef) 
3. See [:material-code-braces: DiskIopsConfigurationTypeDef](./type_defs.md#diskiopsconfigurationtypedef) 
## UpdateSvmActiveDirectoryConfigurationTypeDef

```python
# UpdateSvmActiveDirectoryConfigurationTypeDef definition

class UpdateSvmActiveDirectoryConfigurationTypeDef(TypedDict):
    SelfManagedActiveDirectoryConfiguration: NotRequired[SelfManagedActiveDirectoryConfigurationUpdatesTypeDef],  # (1)
    NetBiosName: NotRequired[str],
```

1. See [:material-code-braces: SelfManagedActiveDirectoryConfigurationUpdatesTypeDef](./type_defs.md#selfmanagedactivedirectoryconfigurationupdatestypedef) 
## SvmEndpointsTypeDef

```python
# SvmEndpointsTypeDef definition

class SvmEndpointsTypeDef(TypedDict):
    Iscsi: NotRequired[SvmEndpointTypeDef],  # (1)
    Management: NotRequired[SvmEndpointTypeDef],  # (1)
    Nfs: NotRequired[SvmEndpointTypeDef],  # (1)
    Smb: NotRequired[SvmEndpointTypeDef],  # (1)
```

1. See [:material-code-braces: SvmEndpointTypeDef](./type_defs.md#svmendpointtypedef) 
2. See [:material-code-braces: SvmEndpointTypeDef](./type_defs.md#svmendpointtypedef) 
3. See [:material-code-braces: SvmEndpointTypeDef](./type_defs.md#svmendpointtypedef) 
4. See [:material-code-braces: SvmEndpointTypeDef](./type_defs.md#svmendpointtypedef) 
## UpdateFileCacheRequestRequestTypeDef

```python
# UpdateFileCacheRequestRequestTypeDef definition

class UpdateFileCacheRequestRequestTypeDef(TypedDict):
    FileCacheId: str,
    ClientRequestToken: NotRequired[str],
    LustreConfiguration: NotRequired[UpdateFileCacheLustreConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: UpdateFileCacheLustreConfigurationTypeDef](./type_defs.md#updatefilecachelustreconfigurationtypedef) 
## WindowsFileSystemConfigurationTypeDef

```python
# WindowsFileSystemConfigurationTypeDef definition

class WindowsFileSystemConfigurationTypeDef(TypedDict):
    ActiveDirectoryId: NotRequired[str],
    SelfManagedActiveDirectoryConfiguration: NotRequired[SelfManagedActiveDirectoryAttributesTypeDef],  # (1)
    DeploymentType: NotRequired[WindowsDeploymentTypeType],  # (2)
    RemoteAdministrationEndpoint: NotRequired[str],
    PreferredSubnetId: NotRequired[str],
    PreferredFileServerIp: NotRequired[str],
    ThroughputCapacity: NotRequired[int],
    MaintenanceOperationsInProgress: NotRequired[list[FileSystemMaintenanceOperationType]],  # (3)
    WeeklyMaintenanceStartTime: NotRequired[str],
    DailyAutomaticBackupStartTime: NotRequired[str],
    AutomaticBackupRetentionDays: NotRequired[int],
    CopyTagsToBackups: NotRequired[bool],
    Aliases: NotRequired[list[AliasTypeDef]],  # (4)
    AuditLogConfiguration: NotRequired[WindowsAuditLogConfigurationTypeDef],  # (5)
    DiskIopsConfiguration: NotRequired[DiskIopsConfigurationTypeDef],  # (6)
```

1. See [:material-code-braces: SelfManagedActiveDirectoryAttributesTypeDef](./type_defs.md#selfmanagedactivedirectoryattributestypedef) 
2. See [:material-code-brackets: WindowsDeploymentTypeType](./literals.md#windowsdeploymenttypetype) 
3. See [:material-code-brackets: FileSystemMaintenanceOperationType](./literals.md#filesystemmaintenanceoperationtype) 
4. See [:material-code-braces: AliasTypeDef](./type_defs.md#aliastypedef) 
5. See [:material-code-braces: WindowsAuditLogConfigurationTypeDef](./type_defs.md#windowsauditlogconfigurationtypedef) 
6. See [:material-code-braces: DiskIopsConfigurationTypeDef](./type_defs.md#diskiopsconfigurationtypedef) 
## DataRepositoryAssociationTypeDef

```python
# DataRepositoryAssociationTypeDef definition

class DataRepositoryAssociationTypeDef(TypedDict):
    AssociationId: NotRequired[str],
    ResourceARN: NotRequired[str],
    FileSystemId: NotRequired[str],
    Lifecycle: NotRequired[DataRepositoryLifecycleType],  # (1)
    FailureDetails: NotRequired[DataRepositoryFailureDetailsTypeDef],  # (2)
    FileSystemPath: NotRequired[str],
    DataRepositoryPath: NotRequired[str],
    BatchImportMetaDataOnCreate: NotRequired[bool],
    ImportedFileChunkSize: NotRequired[int],
    S3: NotRequired[S3DataRepositoryConfigurationOutputTypeDef],  # (3)
    Tags: NotRequired[list[TagTypeDef]],  # (4)
    CreationTime: NotRequired[datetime],
    FileCacheId: NotRequired[str],
    FileCachePath: NotRequired[str],
    DataRepositorySubdirectories: NotRequired[list[str]],
    NFS: NotRequired[NFSDataRepositoryConfigurationTypeDef],  # (5)
```

1. See [:material-code-brackets: DataRepositoryLifecycleType](./literals.md#datarepositorylifecycletype) 
2. See [:material-code-braces: DataRepositoryFailureDetailsTypeDef](./type_defs.md#datarepositoryfailuredetailstypedef) 
3. See [:material-code-braces: S3DataRepositoryConfigurationOutputTypeDef](./type_defs.md#s3datarepositoryconfigurationoutputtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: NFSDataRepositoryConfigurationTypeDef](./type_defs.md#nfsdatarepositoryconfigurationtypedef) 
## S3DataRepositoryConfigurationTypeDef

```python
# S3DataRepositoryConfigurationTypeDef definition

class S3DataRepositoryConfigurationTypeDef(TypedDict):
    AutoImportPolicy: NotRequired[AutoImportPolicyUnionTypeDef],  # (1)
    AutoExportPolicy: NotRequired[AutoExportPolicyUnionTypeDef],  # (2)
```

1. See [:material-code-braces: AutoImportPolicyTypeDef](./type_defs.md#autoimportpolicytypedef) [:material-code-braces: AutoImportPolicyOutputTypeDef](./type_defs.md#autoimportpolicyoutputtypedef) 
2. See [:material-code-braces: AutoExportPolicyTypeDef](./type_defs.md#autoexportpolicytypedef) [:material-code-braces: AutoExportPolicyOutputTypeDef](./type_defs.md#autoexportpolicyoutputtypedef) 
## DeleteFileSystemRequestRequestTypeDef

```python
# DeleteFileSystemRequestRequestTypeDef definition

class DeleteFileSystemRequestRequestTypeDef(TypedDict):
    FileSystemId: str,
    ClientRequestToken: NotRequired[str],
    WindowsConfiguration: NotRequired[DeleteFileSystemWindowsConfigurationTypeDef],  # (1)
    LustreConfiguration: NotRequired[DeleteFileSystemLustreConfigurationTypeDef],  # (2)
    OpenZFSConfiguration: NotRequired[DeleteFileSystemOpenZFSConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: DeleteFileSystemWindowsConfigurationTypeDef](./type_defs.md#deletefilesystemwindowsconfigurationtypedef) 
2. See [:material-code-braces: DeleteFileSystemLustreConfigurationTypeDef](./type_defs.md#deletefilesystemlustreconfigurationtypedef) 
3. See [:material-code-braces: DeleteFileSystemOpenZFSConfigurationTypeDef](./type_defs.md#deletefilesystemopenzfsconfigurationtypedef) 
## DeleteFileSystemResponseTypeDef

```python
# DeleteFileSystemResponseTypeDef definition

class DeleteFileSystemResponseTypeDef(TypedDict):
    FileSystemId: str,
    Lifecycle: FileSystemLifecycleType,  # (1)
    WindowsResponse: DeleteFileSystemWindowsResponseTypeDef,  # (2)
    LustreResponse: DeleteFileSystemLustreResponseTypeDef,  # (3)
    OpenZFSResponse: DeleteFileSystemOpenZFSResponseTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: FileSystemLifecycleType](./literals.md#filesystemlifecycletype) 
2. See [:material-code-braces: DeleteFileSystemWindowsResponseTypeDef](./type_defs.md#deletefilesystemwindowsresponsetypedef) 
3. See [:material-code-braces: DeleteFileSystemLustreResponseTypeDef](./type_defs.md#deletefilesystemlustreresponsetypedef) 
4. See [:material-code-braces: DeleteFileSystemOpenZFSResponseTypeDef](./type_defs.md#deletefilesystemopenzfsresponsetypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteVolumeRequestRequestTypeDef

```python
# DeleteVolumeRequestRequestTypeDef definition

class DeleteVolumeRequestRequestTypeDef(TypedDict):
    VolumeId: str,
    ClientRequestToken: NotRequired[str],
    OntapConfiguration: NotRequired[DeleteVolumeOntapConfigurationTypeDef],  # (1)
    OpenZFSConfiguration: NotRequired[DeleteVolumeOpenZFSConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: DeleteVolumeOntapConfigurationTypeDef](./type_defs.md#deletevolumeontapconfigurationtypedef) 
2. See [:material-code-braces: DeleteVolumeOpenZFSConfigurationTypeDef](./type_defs.md#deletevolumeopenzfsconfigurationtypedef) 
## DeleteVolumeResponseTypeDef

```python
# DeleteVolumeResponseTypeDef definition

class DeleteVolumeResponseTypeDef(TypedDict):
    VolumeId: str,
    Lifecycle: VolumeLifecycleType,  # (1)
    OntapResponse: DeleteVolumeOntapResponseTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: VolumeLifecycleType](./literals.md#volumelifecycletype) 
2. See [:material-code-braces: DeleteVolumeOntapResponseTypeDef](./type_defs.md#deletevolumeontapresponsetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStorageVirtualMachineRequestRequestTypeDef

```python
# CreateStorageVirtualMachineRequestRequestTypeDef definition

class CreateStorageVirtualMachineRequestRequestTypeDef(TypedDict):
    FileSystemId: str,
    Name: str,
    ActiveDirectoryConfiguration: NotRequired[CreateSvmActiveDirectoryConfigurationTypeDef],  # (1)
    ClientRequestToken: NotRequired[str],
    SvmAdminPassword: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    RootVolumeSecurityStyle: NotRequired[StorageVirtualMachineRootVolumeSecurityStyleType],  # (3)
```

1. See [:material-code-braces: CreateSvmActiveDirectoryConfigurationTypeDef](./type_defs.md#createsvmactivedirectoryconfigurationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: StorageVirtualMachineRootVolumeSecurityStyleType](./literals.md#storagevirtualmachinerootvolumesecuritystyletype) 
## LustreFileSystemConfigurationTypeDef

```python
# LustreFileSystemConfigurationTypeDef definition

class LustreFileSystemConfigurationTypeDef(TypedDict):
    WeeklyMaintenanceStartTime: NotRequired[str],
    DataRepositoryConfiguration: NotRequired[DataRepositoryConfigurationTypeDef],  # (1)
    DeploymentType: NotRequired[LustreDeploymentTypeType],  # (2)
    PerUnitStorageThroughput: NotRequired[int],
    MountName: NotRequired[str],
    DailyAutomaticBackupStartTime: NotRequired[str],
    AutomaticBackupRetentionDays: NotRequired[int],
    CopyTagsToBackups: NotRequired[bool],
    DriveCacheType: NotRequired[DriveCacheTypeType],  # (3)
    DataCompressionType: NotRequired[DataCompressionTypeType],  # (4)
    LogConfiguration: NotRequired[LustreLogConfigurationTypeDef],  # (5)
    RootSquashConfiguration: NotRequired[LustreRootSquashConfigurationOutputTypeDef],  # (6)
    MetadataConfiguration: NotRequired[FileSystemLustreMetadataConfigurationTypeDef],  # (7)
    EfaEnabled: NotRequired[bool],
```

1. See [:material-code-braces: DataRepositoryConfigurationTypeDef](./type_defs.md#datarepositoryconfigurationtypedef) 
2. See [:material-code-brackets: LustreDeploymentTypeType](./literals.md#lustredeploymenttypetype) 
3. See [:material-code-brackets: DriveCacheTypeType](./literals.md#drivecachetypetype) 
4. See [:material-code-brackets: DataCompressionTypeType](./literals.md#datacompressiontypetype) 
5. See [:material-code-braces: LustreLogConfigurationTypeDef](./type_defs.md#lustrelogconfigurationtypedef) 
6. See [:material-code-braces: LustreRootSquashConfigurationOutputTypeDef](./type_defs.md#lustrerootsquashconfigurationoutputtypedef) 
7. See [:material-code-braces: FileSystemLustreMetadataConfigurationTypeDef](./type_defs.md#filesystemlustremetadataconfigurationtypedef) 
## CreateDataRepositoryTaskRequestRequestTypeDef

```python
# CreateDataRepositoryTaskRequestRequestTypeDef definition

class CreateDataRepositoryTaskRequestRequestTypeDef(TypedDict):
    Type: DataRepositoryTaskTypeType,  # (1)
    FileSystemId: str,
    Report: CompletionReportTypeDef,  # (2)
    Paths: NotRequired[Sequence[str]],
    ClientRequestToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    CapacityToRelease: NotRequired[int],
    ReleaseConfiguration: NotRequired[ReleaseConfigurationTypeDef],  # (4)
```

1. See [:material-code-brackets: DataRepositoryTaskTypeType](./literals.md#datarepositorytasktypetype) 
2. See [:material-code-braces: CompletionReportTypeDef](./type_defs.md#completionreporttypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: ReleaseConfigurationTypeDef](./type_defs.md#releaseconfigurationtypedef) 
## DataRepositoryTaskTypeDef

```python
# DataRepositoryTaskTypeDef definition

class DataRepositoryTaskTypeDef(TypedDict):
    TaskId: str,
    Lifecycle: DataRepositoryTaskLifecycleType,  # (1)
    Type: DataRepositoryTaskTypeType,  # (2)
    CreationTime: datetime,
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    ResourceARN: NotRequired[str],
    Tags: NotRequired[list[TagTypeDef]],  # (3)
    FileSystemId: NotRequired[str],
    Paths: NotRequired[list[str]],
    FailureDetails: NotRequired[DataRepositoryTaskFailureDetailsTypeDef],  # (4)
    Status: NotRequired[DataRepositoryTaskStatusTypeDef],  # (5)
    Report: NotRequired[CompletionReportTypeDef],  # (6)
    CapacityToRelease: NotRequired[int],
    FileCacheId: NotRequired[str],
    ReleaseConfiguration: NotRequired[ReleaseConfigurationTypeDef],  # (7)
```

1. See [:material-code-brackets: DataRepositoryTaskLifecycleType](./literals.md#datarepositorytasklifecycletype) 
2. See [:material-code-brackets: DataRepositoryTaskTypeType](./literals.md#datarepositorytasktypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: DataRepositoryTaskFailureDetailsTypeDef](./type_defs.md#datarepositorytaskfailuredetailstypedef) 
5. See [:material-code-braces: DataRepositoryTaskStatusTypeDef](./type_defs.md#datarepositorytaskstatustypedef) 
6. See [:material-code-braces: CompletionReportTypeDef](./type_defs.md#completionreporttypedef) 
7. See [:material-code-braces: ReleaseConfigurationTypeDef](./type_defs.md#releaseconfigurationtypedef) 
## CreateFileCacheRequestRequestTypeDef

```python
# CreateFileCacheRequestRequestTypeDef definition

class CreateFileCacheRequestRequestTypeDef(TypedDict):
    FileCacheType: FileCacheTypeType,  # (1)
    FileCacheTypeVersion: str,
    StorageCapacity: int,
    SubnetIds: Sequence[str],
    ClientRequestToken: NotRequired[str],
    SecurityGroupIds: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    CopyTagsToDataRepositoryAssociations: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    LustreConfiguration: NotRequired[CreateFileCacheLustreConfigurationTypeDef],  # (3)
    DataRepositoryAssociations: NotRequired[Sequence[FileCacheDataRepositoryAssociationTypeDef]],  # (4)
```

1. See [:material-code-brackets: FileCacheTypeType](./literals.md#filecachetypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateFileCacheLustreConfigurationTypeDef](./type_defs.md#createfilecachelustreconfigurationtypedef) 
4. See [:material-code-braces: FileCacheDataRepositoryAssociationTypeDef](./type_defs.md#filecachedatarepositoryassociationtypedef) 
## FileCacheCreatingTypeDef

```python
# FileCacheCreatingTypeDef definition

class FileCacheCreatingTypeDef(TypedDict):
    OwnerId: NotRequired[str],
    CreationTime: NotRequired[datetime],
    FileCacheId: NotRequired[str],
    FileCacheType: NotRequired[FileCacheTypeType],  # (1)
    FileCacheTypeVersion: NotRequired[str],
    Lifecycle: NotRequired[FileCacheLifecycleType],  # (2)
    FailureDetails: NotRequired[FileCacheFailureDetailsTypeDef],  # (3)
    StorageCapacity: NotRequired[int],
    VpcId: NotRequired[str],
    SubnetIds: NotRequired[list[str]],
    NetworkInterfaceIds: NotRequired[list[str]],
    DNSName: NotRequired[str],
    KmsKeyId: NotRequired[str],
    ResourceARN: NotRequired[str],
    Tags: NotRequired[list[TagTypeDef]],  # (4)
    CopyTagsToDataRepositoryAssociations: NotRequired[bool],
    LustreConfiguration: NotRequired[FileCacheLustreConfigurationTypeDef],  # (5)
    DataRepositoryAssociationIds: NotRequired[list[str]],
```

1. See [:material-code-brackets: FileCacheTypeType](./literals.md#filecachetypetype) 
2. See [:material-code-brackets: FileCacheLifecycleType](./literals.md#filecachelifecycletype) 
3. See [:material-code-braces: FileCacheFailureDetailsTypeDef](./type_defs.md#filecachefailuredetailstypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: FileCacheLustreConfigurationTypeDef](./type_defs.md#filecachelustreconfigurationtypedef) 
## FileCacheTypeDef

```python
# FileCacheTypeDef definition

class FileCacheTypeDef(TypedDict):
    OwnerId: NotRequired[str],
    CreationTime: NotRequired[datetime],
    FileCacheId: NotRequired[str],
    FileCacheType: NotRequired[FileCacheTypeType],  # (1)
    FileCacheTypeVersion: NotRequired[str],
    Lifecycle: NotRequired[FileCacheLifecycleType],  # (2)
    FailureDetails: NotRequired[FileCacheFailureDetailsTypeDef],  # (3)
    StorageCapacity: NotRequired[int],
    VpcId: NotRequired[str],
    SubnetIds: NotRequired[list[str]],
    NetworkInterfaceIds: NotRequired[list[str]],
    DNSName: NotRequired[str],
    KmsKeyId: NotRequired[str],
    ResourceARN: NotRequired[str],
    LustreConfiguration: NotRequired[FileCacheLustreConfigurationTypeDef],  # (4)
    DataRepositoryAssociationIds: NotRequired[list[str]],
```

1. See [:material-code-brackets: FileCacheTypeType](./literals.md#filecachetypetype) 
2. See [:material-code-brackets: FileCacheLifecycleType](./literals.md#filecachelifecycletype) 
3. See [:material-code-braces: FileCacheFailureDetailsTypeDef](./type_defs.md#filecachefailuredetailstypedef) 
4. See [:material-code-braces: FileCacheLustreConfigurationTypeDef](./type_defs.md#filecachelustreconfigurationtypedef) 
## OntapFileSystemConfigurationTypeDef

```python
# OntapFileSystemConfigurationTypeDef definition

class OntapFileSystemConfigurationTypeDef(TypedDict):
    AutomaticBackupRetentionDays: NotRequired[int],
    DailyAutomaticBackupStartTime: NotRequired[str],
    DeploymentType: NotRequired[OntapDeploymentTypeType],  # (1)
    EndpointIpAddressRange: NotRequired[str],
    Endpoints: NotRequired[FileSystemEndpointsTypeDef],  # (2)
    DiskIopsConfiguration: NotRequired[DiskIopsConfigurationTypeDef],  # (3)
    PreferredSubnetId: NotRequired[str],
    RouteTableIds: NotRequired[list[str]],
    ThroughputCapacity: NotRequired[int],
    WeeklyMaintenanceStartTime: NotRequired[str],
    FsxAdminPassword: NotRequired[str],
    HAPairs: NotRequired[int],
    ThroughputCapacityPerHAPair: NotRequired[int],
```

1. See [:material-code-brackets: OntapDeploymentTypeType](./literals.md#ontapdeploymenttypetype) 
2. See [:material-code-braces: FileSystemEndpointsTypeDef](./type_defs.md#filesystemendpointstypedef) 
3. See [:material-code-braces: DiskIopsConfigurationTypeDef](./type_defs.md#diskiopsconfigurationtypedef) 
## CreateSnapshotResponseTypeDef

```python
# CreateSnapshotResponseTypeDef definition

class CreateSnapshotResponseTypeDef(TypedDict):
    Snapshot: SnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSnapshotsResponseTypeDef

```python
# DescribeSnapshotsResponseTypeDef definition

class DescribeSnapshotsResponseTypeDef(TypedDict):
    Snapshots: list[SnapshotTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSnapshotResponseTypeDef

```python
# UpdateSnapshotResponseTypeDef definition

class UpdateSnapshotResponseTypeDef(TypedDict):
    Snapshot: SnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFileSystemLustreConfigurationTypeDef

```python
# CreateFileSystemLustreConfigurationTypeDef definition

class CreateFileSystemLustreConfigurationTypeDef(TypedDict):
    WeeklyMaintenanceStartTime: NotRequired[str],
    ImportPath: NotRequired[str],
    ExportPath: NotRequired[str],
    ImportedFileChunkSize: NotRequired[int],
    DeploymentType: NotRequired[LustreDeploymentTypeType],  # (1)
    AutoImportPolicy: NotRequired[AutoImportPolicyTypeType],  # (2)
    PerUnitStorageThroughput: NotRequired[int],
    DailyAutomaticBackupStartTime: NotRequired[str],
    AutomaticBackupRetentionDays: NotRequired[int],
    CopyTagsToBackups: NotRequired[bool],
    DriveCacheType: NotRequired[DriveCacheTypeType],  # (3)
    DataCompressionType: NotRequired[DataCompressionTypeType],  # (4)
    EfaEnabled: NotRequired[bool],
    LogConfiguration: NotRequired[LustreLogCreateConfigurationTypeDef],  # (5)
    RootSquashConfiguration: NotRequired[LustreRootSquashConfigurationUnionTypeDef],  # (6)
    MetadataConfiguration: NotRequired[CreateFileSystemLustreMetadataConfigurationTypeDef],  # (7)
```

1. See [:material-code-brackets: LustreDeploymentTypeType](./literals.md#lustredeploymenttypetype) 
2. See [:material-code-brackets: AutoImportPolicyTypeType](./literals.md#autoimportpolicytypetype) 
3. See [:material-code-brackets: DriveCacheTypeType](./literals.md#drivecachetypetype) 
4. See [:material-code-brackets: DataCompressionTypeType](./literals.md#datacompressiontypetype) 
5. See [:material-code-braces: LustreLogCreateConfigurationTypeDef](./type_defs.md#lustrelogcreateconfigurationtypedef) 
6. See [:material-code-braces: LustreRootSquashConfigurationTypeDef](./type_defs.md#lustrerootsquashconfigurationtypedef) [:material-code-braces: LustreRootSquashConfigurationOutputTypeDef](./type_defs.md#lustrerootsquashconfigurationoutputtypedef) 
7. See [:material-code-braces: CreateFileSystemLustreMetadataConfigurationTypeDef](./type_defs.md#createfilesystemlustremetadataconfigurationtypedef) 
## UpdateFileSystemLustreConfigurationTypeDef

```python
# UpdateFileSystemLustreConfigurationTypeDef definition

class UpdateFileSystemLustreConfigurationTypeDef(TypedDict):
    WeeklyMaintenanceStartTime: NotRequired[str],
    DailyAutomaticBackupStartTime: NotRequired[str],
    AutomaticBackupRetentionDays: NotRequired[int],
    AutoImportPolicy: NotRequired[AutoImportPolicyTypeType],  # (1)
    DataCompressionType: NotRequired[DataCompressionTypeType],  # (2)
    LogConfiguration: NotRequired[LustreLogCreateConfigurationTypeDef],  # (3)
    RootSquashConfiguration: NotRequired[LustreRootSquashConfigurationUnionTypeDef],  # (4)
    PerUnitStorageThroughput: NotRequired[int],
    MetadataConfiguration: NotRequired[UpdateFileSystemLustreMetadataConfigurationTypeDef],  # (5)
```

1. See [:material-code-brackets: AutoImportPolicyTypeType](./literals.md#autoimportpolicytypetype) 
2. See [:material-code-brackets: DataCompressionTypeType](./literals.md#datacompressiontypetype) 
3. See [:material-code-braces: LustreLogCreateConfigurationTypeDef](./type_defs.md#lustrelogcreateconfigurationtypedef) 
4. See [:material-code-braces: LustreRootSquashConfigurationTypeDef](./type_defs.md#lustrerootsquashconfigurationtypedef) [:material-code-braces: LustreRootSquashConfigurationOutputTypeDef](./type_defs.md#lustrerootsquashconfigurationoutputtypedef) 
5. See [:material-code-braces: UpdateFileSystemLustreMetadataConfigurationTypeDef](./type_defs.md#updatefilesystemlustremetadataconfigurationtypedef) 
## OpenZFSVolumeConfigurationTypeDef

```python
# OpenZFSVolumeConfigurationTypeDef definition

class OpenZFSVolumeConfigurationTypeDef(TypedDict):
    ParentVolumeId: NotRequired[str],
    VolumePath: NotRequired[str],
    StorageCapacityReservationGiB: NotRequired[int],
    StorageCapacityQuotaGiB: NotRequired[int],
    RecordSizeKiB: NotRequired[int],
    DataCompressionType: NotRequired[OpenZFSDataCompressionTypeType],  # (1)
    CopyTagsToSnapshots: NotRequired[bool],
    OriginSnapshot: NotRequired[OpenZFSOriginSnapshotConfigurationTypeDef],  # (2)
    ReadOnly: NotRequired[bool],
    NfsExports: NotRequired[list[OpenZFSNfsExportOutputTypeDef]],  # (3)
    UserAndGroupQuotas: NotRequired[list[OpenZFSUserOrGroupQuotaTypeDef]],  # (4)
    RestoreToSnapshot: NotRequired[str],
    DeleteIntermediateSnaphots: NotRequired[bool],
    DeleteClonedVolumes: NotRequired[bool],
    DeleteIntermediateData: NotRequired[bool],
    SourceSnapshotARN: NotRequired[str],
    DestinationSnapshot: NotRequired[str],
    CopyStrategy: NotRequired[OpenZFSCopyStrategyType],  # (5)
```

1. See [:material-code-brackets: OpenZFSDataCompressionTypeType](./literals.md#openzfsdatacompressiontypetype) 
2. See [:material-code-braces: OpenZFSOriginSnapshotConfigurationTypeDef](./type_defs.md#openzfsoriginsnapshotconfigurationtypedef) 
3. See [:material-code-braces: OpenZFSNfsExportOutputTypeDef](./type_defs.md#openzfsnfsexportoutputtypedef) 
4. See [:material-code-braces: OpenZFSUserOrGroupQuotaTypeDef](./type_defs.md#openzfsuserorgroupquotatypedef) 
5. See [:material-code-brackets: OpenZFSCopyStrategyType](./literals.md#openzfscopystrategytype) 
## OpenZFSNfsExportTypeDef

```python
# OpenZFSNfsExportTypeDef definition

class OpenZFSNfsExportTypeDef(TypedDict):
    ClientConfigurations: Sequence[OpenZFSClientConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: OpenZFSClientConfigurationTypeDef](./type_defs.md#openzfsclientconfigurationtypedef) [:material-code-braces: OpenZFSClientConfigurationOutputTypeDef](./type_defs.md#openzfsclientconfigurationoutputtypedef) 
## CreateSnaplockConfigurationTypeDef

```python
# CreateSnaplockConfigurationTypeDef definition

class CreateSnaplockConfigurationTypeDef(TypedDict):
    SnaplockType: SnaplockTypeType,  # (4)
    AuditLogVolume: NotRequired[bool],
    AutocommitPeriod: NotRequired[AutocommitPeriodTypeDef],  # (1)
    PrivilegedDelete: NotRequired[PrivilegedDeleteType],  # (2)
    RetentionPeriod: NotRequired[SnaplockRetentionPeriodTypeDef],  # (3)
    VolumeAppendModeEnabled: NotRequired[bool],
```

1. See [:material-code-braces: AutocommitPeriodTypeDef](./type_defs.md#autocommitperiodtypedef) 
2. See [:material-code-brackets: PrivilegedDeleteType](./literals.md#privilegeddeletetype) 
3. See [:material-code-braces: SnaplockRetentionPeriodTypeDef](./type_defs.md#snaplockretentionperiodtypedef) 
4. See [:material-code-brackets: SnaplockTypeType](./literals.md#snaplocktypetype) 
## SnaplockConfigurationTypeDef

```python
# SnaplockConfigurationTypeDef definition

class SnaplockConfigurationTypeDef(TypedDict):
    AuditLogVolume: NotRequired[bool],
    AutocommitPeriod: NotRequired[AutocommitPeriodTypeDef],  # (1)
    PrivilegedDelete: NotRequired[PrivilegedDeleteType],  # (2)
    RetentionPeriod: NotRequired[SnaplockRetentionPeriodTypeDef],  # (3)
    SnaplockType: NotRequired[SnaplockTypeType],  # (4)
    VolumeAppendModeEnabled: NotRequired[bool],
```

1. See [:material-code-braces: AutocommitPeriodTypeDef](./type_defs.md#autocommitperiodtypedef) 
2. See [:material-code-brackets: PrivilegedDeleteType](./literals.md#privilegeddeletetype) 
3. See [:material-code-braces: SnaplockRetentionPeriodTypeDef](./type_defs.md#snaplockretentionperiodtypedef) 
4. See [:material-code-brackets: SnaplockTypeType](./literals.md#snaplocktypetype) 
## UpdateSnaplockConfigurationTypeDef

```python
# UpdateSnaplockConfigurationTypeDef definition

class UpdateSnaplockConfigurationTypeDef(TypedDict):
    AuditLogVolume: NotRequired[bool],
    AutocommitPeriod: NotRequired[AutocommitPeriodTypeDef],  # (1)
    PrivilegedDelete: NotRequired[PrivilegedDeleteType],  # (2)
    RetentionPeriod: NotRequired[SnaplockRetentionPeriodTypeDef],  # (3)
    VolumeAppendModeEnabled: NotRequired[bool],
```

1. See [:material-code-braces: AutocommitPeriodTypeDef](./type_defs.md#autocommitperiodtypedef) 
2. See [:material-code-brackets: PrivilegedDeleteType](./literals.md#privilegeddeletetype) 
3. See [:material-code-braces: SnaplockRetentionPeriodTypeDef](./type_defs.md#snaplockretentionperiodtypedef) 
## UpdateStorageVirtualMachineRequestRequestTypeDef

```python
# UpdateStorageVirtualMachineRequestRequestTypeDef definition

class UpdateStorageVirtualMachineRequestRequestTypeDef(TypedDict):
    StorageVirtualMachineId: str,
    ActiveDirectoryConfiguration: NotRequired[UpdateSvmActiveDirectoryConfigurationTypeDef],  # (1)
    ClientRequestToken: NotRequired[str],
    SvmAdminPassword: NotRequired[str],
```

1. See [:material-code-braces: UpdateSvmActiveDirectoryConfigurationTypeDef](./type_defs.md#updatesvmactivedirectoryconfigurationtypedef) 
## StorageVirtualMachineTypeDef

```python
# StorageVirtualMachineTypeDef definition

class StorageVirtualMachineTypeDef(TypedDict):
    ActiveDirectoryConfiguration: NotRequired[SvmActiveDirectoryConfigurationTypeDef],  # (1)
    CreationTime: NotRequired[datetime],
    Endpoints: NotRequired[SvmEndpointsTypeDef],  # (2)
    FileSystemId: NotRequired[str],
    Lifecycle: NotRequired[StorageVirtualMachineLifecycleType],  # (3)
    Name: NotRequired[str],
    ResourceARN: NotRequired[str],
    StorageVirtualMachineId: NotRequired[str],
    Subtype: NotRequired[StorageVirtualMachineSubtypeType],  # (4)
    UUID: NotRequired[str],
    Tags: NotRequired[list[TagTypeDef]],  # (5)
    LifecycleTransitionReason: NotRequired[LifecycleTransitionReasonTypeDef],  # (6)
    RootVolumeSecurityStyle: NotRequired[StorageVirtualMachineRootVolumeSecurityStyleType],  # (7)
```

1. See [:material-code-braces: SvmActiveDirectoryConfigurationTypeDef](./type_defs.md#svmactivedirectoryconfigurationtypedef) 
2. See [:material-code-braces: SvmEndpointsTypeDef](./type_defs.md#svmendpointstypedef) 
3. See [:material-code-brackets: StorageVirtualMachineLifecycleType](./literals.md#storagevirtualmachinelifecycletype) 
4. See [:material-code-brackets: StorageVirtualMachineSubtypeType](./literals.md#storagevirtualmachinesubtypetype) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: LifecycleTransitionReasonTypeDef](./type_defs.md#lifecycletransitionreasontypedef) 
7. See [:material-code-brackets: StorageVirtualMachineRootVolumeSecurityStyleType](./literals.md#storagevirtualmachinerootvolumesecuritystyletype) 
## CreateDataRepositoryAssociationResponseTypeDef

```python
# CreateDataRepositoryAssociationResponseTypeDef definition

class CreateDataRepositoryAssociationResponseTypeDef(TypedDict):
    Association: DataRepositoryAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataRepositoryAssociationTypeDef](./type_defs.md#datarepositoryassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDataRepositoryAssociationsResponseTypeDef

```python
# DescribeDataRepositoryAssociationsResponseTypeDef definition

class DescribeDataRepositoryAssociationsResponseTypeDef(TypedDict):
    Associations: list[DataRepositoryAssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DataRepositoryAssociationTypeDef](./type_defs.md#datarepositoryassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDataRepositoryAssociationResponseTypeDef

```python
# UpdateDataRepositoryAssociationResponseTypeDef definition

class UpdateDataRepositoryAssociationResponseTypeDef(TypedDict):
    Association: DataRepositoryAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataRepositoryAssociationTypeDef](./type_defs.md#datarepositoryassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataRepositoryAssociationRequestRequestTypeDef

```python
# CreateDataRepositoryAssociationRequestRequestTypeDef definition

class CreateDataRepositoryAssociationRequestRequestTypeDef(TypedDict):
    FileSystemId: str,
    DataRepositoryPath: str,
    FileSystemPath: NotRequired[str],
    BatchImportMetaDataOnCreate: NotRequired[bool],
    ImportedFileChunkSize: NotRequired[int],
    S3: NotRequired[S3DataRepositoryConfigurationTypeDef],  # (1)
    ClientRequestToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: S3DataRepositoryConfigurationTypeDef](./type_defs.md#s3datarepositoryconfigurationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateDataRepositoryAssociationRequestRequestTypeDef

```python
# UpdateDataRepositoryAssociationRequestRequestTypeDef definition

class UpdateDataRepositoryAssociationRequestRequestTypeDef(TypedDict):
    AssociationId: str,
    ClientRequestToken: NotRequired[str],
    ImportedFileChunkSize: NotRequired[int],
    S3: NotRequired[S3DataRepositoryConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: S3DataRepositoryConfigurationTypeDef](./type_defs.md#s3datarepositoryconfigurationtypedef) 
## CreateDataRepositoryTaskResponseTypeDef

```python
# CreateDataRepositoryTaskResponseTypeDef definition

class CreateDataRepositoryTaskResponseTypeDef(TypedDict):
    DataRepositoryTask: DataRepositoryTaskTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataRepositoryTaskTypeDef](./type_defs.md#datarepositorytasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDataRepositoryTasksResponseTypeDef

```python
# DescribeDataRepositoryTasksResponseTypeDef definition

class DescribeDataRepositoryTasksResponseTypeDef(TypedDict):
    DataRepositoryTasks: list[DataRepositoryTaskTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DataRepositoryTaskTypeDef](./type_defs.md#datarepositorytasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFileCacheResponseTypeDef

```python
# CreateFileCacheResponseTypeDef definition

class CreateFileCacheResponseTypeDef(TypedDict):
    FileCache: FileCacheCreatingTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FileCacheCreatingTypeDef](./type_defs.md#filecachecreatingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFileCachesResponseTypeDef

```python
# DescribeFileCachesResponseTypeDef definition

class DescribeFileCachesResponseTypeDef(TypedDict):
    FileCaches: list[FileCacheTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FileCacheTypeDef](./type_defs.md#filecachetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFileCacheResponseTypeDef

```python
# UpdateFileCacheResponseTypeDef definition

class UpdateFileCacheResponseTypeDef(TypedDict):
    FileCache: FileCacheTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FileCacheTypeDef](./type_defs.md#filecachetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFileSystemRequestRequestTypeDef

```python
# UpdateFileSystemRequestRequestTypeDef definition

class UpdateFileSystemRequestRequestTypeDef(TypedDict):
    FileSystemId: str,
    ClientRequestToken: NotRequired[str],
    StorageCapacity: NotRequired[int],
    WindowsConfiguration: NotRequired[UpdateFileSystemWindowsConfigurationTypeDef],  # (1)
    LustreConfiguration: NotRequired[UpdateFileSystemLustreConfigurationTypeDef],  # (2)
    OntapConfiguration: NotRequired[UpdateFileSystemOntapConfigurationTypeDef],  # (3)
    OpenZFSConfiguration: NotRequired[UpdateFileSystemOpenZFSConfigurationTypeDef],  # (4)
    StorageType: NotRequired[StorageTypeType],  # (5)
```

1. See [:material-code-braces: UpdateFileSystemWindowsConfigurationTypeDef](./type_defs.md#updatefilesystemwindowsconfigurationtypedef) 
2. See [:material-code-braces: UpdateFileSystemLustreConfigurationTypeDef](./type_defs.md#updatefilesystemlustreconfigurationtypedef) 
3. See [:material-code-braces: UpdateFileSystemOntapConfigurationTypeDef](./type_defs.md#updatefilesystemontapconfigurationtypedef) 
4. See [:material-code-braces: UpdateFileSystemOpenZFSConfigurationTypeDef](./type_defs.md#updatefilesystemopenzfsconfigurationtypedef) 
5. See [:material-code-brackets: StorageTypeType](./literals.md#storagetypetype) 
## CreateOntapVolumeConfigurationTypeDef

```python
# CreateOntapVolumeConfigurationTypeDef definition

class CreateOntapVolumeConfigurationTypeDef(TypedDict):
    StorageVirtualMachineId: str,
    JunctionPath: NotRequired[str],
    SecurityStyle: NotRequired[SecurityStyleType],  # (1)
    SizeInMegabytes: NotRequired[int],
    StorageEfficiencyEnabled: NotRequired[bool],
    TieringPolicy: NotRequired[TieringPolicyTypeDef],  # (2)
    OntapVolumeType: NotRequired[InputOntapVolumeTypeType],  # (3)
    SnapshotPolicy: NotRequired[str],
    CopyTagsToBackups: NotRequired[bool],
    SnaplockConfiguration: NotRequired[CreateSnaplockConfigurationTypeDef],  # (4)
    VolumeStyle: NotRequired[VolumeStyleType],  # (5)
    AggregateConfiguration: NotRequired[CreateAggregateConfigurationTypeDef],  # (6)
    SizeInBytes: NotRequired[int],
```

1. See [:material-code-brackets: SecurityStyleType](./literals.md#securitystyletype) 
2. See [:material-code-braces: TieringPolicyTypeDef](./type_defs.md#tieringpolicytypedef) 
3. See [:material-code-brackets: InputOntapVolumeTypeType](./literals.md#inputontapvolumetypetype) 
4. See [:material-code-braces: CreateSnaplockConfigurationTypeDef](./type_defs.md#createsnaplockconfigurationtypedef) 
5. See [:material-code-brackets: VolumeStyleType](./literals.md#volumestyletype) 
6. See [:material-code-braces: CreateAggregateConfigurationTypeDef](./type_defs.md#createaggregateconfigurationtypedef) 
## OntapVolumeConfigurationTypeDef

```python
# OntapVolumeConfigurationTypeDef definition

class OntapVolumeConfigurationTypeDef(TypedDict):
    FlexCacheEndpointType: NotRequired[FlexCacheEndpointTypeType],  # (1)
    JunctionPath: NotRequired[str],
    SecurityStyle: NotRequired[SecurityStyleType],  # (2)
    SizeInMegabytes: NotRequired[int],
    StorageEfficiencyEnabled: NotRequired[bool],
    StorageVirtualMachineId: NotRequired[str],
    StorageVirtualMachineRoot: NotRequired[bool],
    TieringPolicy: NotRequired[TieringPolicyTypeDef],  # (3)
    UUID: NotRequired[str],
    OntapVolumeType: NotRequired[OntapVolumeTypeType],  # (4)
    SnapshotPolicy: NotRequired[str],
    CopyTagsToBackups: NotRequired[bool],
    SnaplockConfiguration: NotRequired[SnaplockConfigurationTypeDef],  # (5)
    VolumeStyle: NotRequired[VolumeStyleType],  # (6)
    AggregateConfiguration: NotRequired[AggregateConfigurationTypeDef],  # (7)
    SizeInBytes: NotRequired[int],
```

1. See [:material-code-brackets: FlexCacheEndpointTypeType](./literals.md#flexcacheendpointtypetype) 
2. See [:material-code-brackets: SecurityStyleType](./literals.md#securitystyletype) 
3. See [:material-code-braces: TieringPolicyTypeDef](./type_defs.md#tieringpolicytypedef) 
4. See [:material-code-brackets: OntapVolumeTypeType](./literals.md#ontapvolumetypetype) 
5. See [:material-code-braces: SnaplockConfigurationTypeDef](./type_defs.md#snaplockconfigurationtypedef) 
6. See [:material-code-brackets: VolumeStyleType](./literals.md#volumestyletype) 
7. See [:material-code-braces: AggregateConfigurationTypeDef](./type_defs.md#aggregateconfigurationtypedef) 
## UpdateOntapVolumeConfigurationTypeDef

```python
# UpdateOntapVolumeConfigurationTypeDef definition

class UpdateOntapVolumeConfigurationTypeDef(TypedDict):
    JunctionPath: NotRequired[str],
    SecurityStyle: NotRequired[SecurityStyleType],  # (1)
    SizeInMegabytes: NotRequired[int],
    StorageEfficiencyEnabled: NotRequired[bool],
    TieringPolicy: NotRequired[TieringPolicyTypeDef],  # (2)
    SnapshotPolicy: NotRequired[str],
    CopyTagsToBackups: NotRequired[bool],
    SnaplockConfiguration: NotRequired[UpdateSnaplockConfigurationTypeDef],  # (3)
    SizeInBytes: NotRequired[int],
```

1. See [:material-code-brackets: SecurityStyleType](./literals.md#securitystyletype) 
2. See [:material-code-braces: TieringPolicyTypeDef](./type_defs.md#tieringpolicytypedef) 
3. See [:material-code-braces: UpdateSnaplockConfigurationTypeDef](./type_defs.md#updatesnaplockconfigurationtypedef) 
## CreateStorageVirtualMachineResponseTypeDef

```python
# CreateStorageVirtualMachineResponseTypeDef definition

class CreateStorageVirtualMachineResponseTypeDef(TypedDict):
    StorageVirtualMachine: StorageVirtualMachineTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StorageVirtualMachineTypeDef](./type_defs.md#storagevirtualmachinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeStorageVirtualMachinesResponseTypeDef

```python
# DescribeStorageVirtualMachinesResponseTypeDef definition

class DescribeStorageVirtualMachinesResponseTypeDef(TypedDict):
    StorageVirtualMachines: list[StorageVirtualMachineTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: StorageVirtualMachineTypeDef](./type_defs.md#storagevirtualmachinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateStorageVirtualMachineResponseTypeDef

```python
# UpdateStorageVirtualMachineResponseTypeDef definition

class UpdateStorageVirtualMachineResponseTypeDef(TypedDict):
    StorageVirtualMachine: StorageVirtualMachineTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StorageVirtualMachineTypeDef](./type_defs.md#storagevirtualmachinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateOpenZFSVolumeConfigurationTypeDef

```python
# CreateOpenZFSVolumeConfigurationTypeDef definition

class CreateOpenZFSVolumeConfigurationTypeDef(TypedDict):
    ParentVolumeId: str,
    StorageCapacityReservationGiB: NotRequired[int],
    StorageCapacityQuotaGiB: NotRequired[int],
    RecordSizeKiB: NotRequired[int],
    DataCompressionType: NotRequired[OpenZFSDataCompressionTypeType],  # (1)
    CopyTagsToSnapshots: NotRequired[bool],
    OriginSnapshot: NotRequired[CreateOpenZFSOriginSnapshotConfigurationTypeDef],  # (2)
    ReadOnly: NotRequired[bool],
    NfsExports: NotRequired[Sequence[OpenZFSNfsExportUnionTypeDef]],  # (3)
    UserAndGroupQuotas: NotRequired[Sequence[OpenZFSUserOrGroupQuotaTypeDef]],  # (4)
```

1. See [:material-code-brackets: OpenZFSDataCompressionTypeType](./literals.md#openzfsdatacompressiontypetype) 
2. See [:material-code-braces: CreateOpenZFSOriginSnapshotConfigurationTypeDef](./type_defs.md#createopenzfsoriginsnapshotconfigurationtypedef) 
3. See [:material-code-braces: OpenZFSNfsExportTypeDef](./type_defs.md#openzfsnfsexporttypedef) [:material-code-braces: OpenZFSNfsExportOutputTypeDef](./type_defs.md#openzfsnfsexportoutputtypedef) 
4. See [:material-code-braces: OpenZFSUserOrGroupQuotaTypeDef](./type_defs.md#openzfsuserorgroupquotatypedef) 
## OpenZFSCreateRootVolumeConfigurationTypeDef

```python
# OpenZFSCreateRootVolumeConfigurationTypeDef definition

class OpenZFSCreateRootVolumeConfigurationTypeDef(TypedDict):
    RecordSizeKiB: NotRequired[int],
    DataCompressionType: NotRequired[OpenZFSDataCompressionTypeType],  # (1)
    NfsExports: NotRequired[Sequence[OpenZFSNfsExportUnionTypeDef]],  # (2)
    UserAndGroupQuotas: NotRequired[Sequence[OpenZFSUserOrGroupQuotaTypeDef]],  # (3)
    CopyTagsToSnapshots: NotRequired[bool],
    ReadOnly: NotRequired[bool],
```

1. See [:material-code-brackets: OpenZFSDataCompressionTypeType](./literals.md#openzfsdatacompressiontypetype) 
2. See [:material-code-braces: OpenZFSNfsExportTypeDef](./type_defs.md#openzfsnfsexporttypedef) [:material-code-braces: OpenZFSNfsExportOutputTypeDef](./type_defs.md#openzfsnfsexportoutputtypedef) 
3. See [:material-code-braces: OpenZFSUserOrGroupQuotaTypeDef](./type_defs.md#openzfsuserorgroupquotatypedef) 
## UpdateOpenZFSVolumeConfigurationTypeDef

```python
# UpdateOpenZFSVolumeConfigurationTypeDef definition

class UpdateOpenZFSVolumeConfigurationTypeDef(TypedDict):
    StorageCapacityReservationGiB: NotRequired[int],
    StorageCapacityQuotaGiB: NotRequired[int],
    RecordSizeKiB: NotRequired[int],
    DataCompressionType: NotRequired[OpenZFSDataCompressionTypeType],  # (1)
    NfsExports: NotRequired[Sequence[OpenZFSNfsExportUnionTypeDef]],  # (2)
    UserAndGroupQuotas: NotRequired[Sequence[OpenZFSUserOrGroupQuotaTypeDef]],  # (3)
    ReadOnly: NotRequired[bool],
```

1. See [:material-code-brackets: OpenZFSDataCompressionTypeType](./literals.md#openzfsdatacompressiontypetype) 
2. See [:material-code-braces: OpenZFSNfsExportTypeDef](./type_defs.md#openzfsnfsexporttypedef) [:material-code-braces: OpenZFSNfsExportOutputTypeDef](./type_defs.md#openzfsnfsexportoutputtypedef) 
3. See [:material-code-braces: OpenZFSUserOrGroupQuotaTypeDef](./type_defs.md#openzfsuserorgroupquotatypedef) 
## CreateVolumeFromBackupRequestRequestTypeDef

```python
# CreateVolumeFromBackupRequestRequestTypeDef definition

class CreateVolumeFromBackupRequestRequestTypeDef(TypedDict):
    BackupId: str,
    Name: str,
    ClientRequestToken: NotRequired[str],
    OntapConfiguration: NotRequired[CreateOntapVolumeConfigurationTypeDef],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: CreateOntapVolumeConfigurationTypeDef](./type_defs.md#createontapvolumeconfigurationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## VolumePaginatorTypeDef

```python
# VolumePaginatorTypeDef definition

class VolumePaginatorTypeDef(TypedDict):
    CreationTime: NotRequired[datetime],
    FileSystemId: NotRequired[str],
    Lifecycle: NotRequired[VolumeLifecycleType],  # (1)
    Name: NotRequired[str],
    OntapConfiguration: NotRequired[OntapVolumeConfigurationTypeDef],  # (2)
    ResourceARN: NotRequired[str],
    Tags: NotRequired[list[TagTypeDef]],  # (3)
    VolumeId: NotRequired[str],
    VolumeType: NotRequired[VolumeTypeType],  # (4)
    LifecycleTransitionReason: NotRequired[LifecycleTransitionReasonTypeDef],  # (5)
    AdministrativeActions: NotRequired[list[dict[str, Any]]],
    OpenZFSConfiguration: NotRequired[OpenZFSVolumeConfigurationTypeDef],  # (6)
```

1. See [:material-code-brackets: VolumeLifecycleType](./literals.md#volumelifecycletype) 
2. See [:material-code-braces: OntapVolumeConfigurationTypeDef](./type_defs.md#ontapvolumeconfigurationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-brackets: VolumeTypeType](./literals.md#volumetypetype) 
5. See [:material-code-braces: LifecycleTransitionReasonTypeDef](./type_defs.md#lifecycletransitionreasontypedef) 
6. See [:material-code-braces: OpenZFSVolumeConfigurationTypeDef](./type_defs.md#openzfsvolumeconfigurationtypedef) 
## VolumeTypeDef

```python
# VolumeTypeDef definition

class VolumeTypeDef(TypedDict):
    CreationTime: NotRequired[datetime],
    FileSystemId: NotRequired[str],
    Lifecycle: NotRequired[VolumeLifecycleType],  # (1)
    Name: NotRequired[str],
    OntapConfiguration: NotRequired[OntapVolumeConfigurationTypeDef],  # (2)
    ResourceARN: NotRequired[str],
    Tags: NotRequired[list[TagTypeDef]],  # (3)
    VolumeId: NotRequired[str],
    VolumeType: NotRequired[VolumeTypeType],  # (4)
    LifecycleTransitionReason: NotRequired[LifecycleTransitionReasonTypeDef],  # (5)
    AdministrativeActions: NotRequired[list[dict[str, Any]]],
    OpenZFSConfiguration: NotRequired[OpenZFSVolumeConfigurationTypeDef],  # (6)
```

1. See [:material-code-brackets: VolumeLifecycleType](./literals.md#volumelifecycletype) 
2. See [:material-code-braces: OntapVolumeConfigurationTypeDef](./type_defs.md#ontapvolumeconfigurationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-brackets: VolumeTypeType](./literals.md#volumetypetype) 
5. See [:material-code-braces: LifecycleTransitionReasonTypeDef](./type_defs.md#lifecycletransitionreasontypedef) 
6. See [:material-code-braces: OpenZFSVolumeConfigurationTypeDef](./type_defs.md#openzfsvolumeconfigurationtypedef) 
## CreateVolumeRequestRequestTypeDef

```python
# CreateVolumeRequestRequestTypeDef definition

class CreateVolumeRequestRequestTypeDef(TypedDict):
    VolumeType: VolumeTypeType,  # (1)
    Name: str,
    ClientRequestToken: NotRequired[str],
    OntapConfiguration: NotRequired[CreateOntapVolumeConfigurationTypeDef],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    OpenZFSConfiguration: NotRequired[CreateOpenZFSVolumeConfigurationTypeDef],  # (4)
```

1. See [:material-code-brackets: VolumeTypeType](./literals.md#volumetypetype) 
2. See [:material-code-braces: CreateOntapVolumeConfigurationTypeDef](./type_defs.md#createontapvolumeconfigurationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateOpenZFSVolumeConfigurationTypeDef](./type_defs.md#createopenzfsvolumeconfigurationtypedef) 
## CreateFileSystemOpenZFSConfigurationTypeDef

```python
# CreateFileSystemOpenZFSConfigurationTypeDef definition

class CreateFileSystemOpenZFSConfigurationTypeDef(TypedDict):
    DeploymentType: OpenZFSDeploymentTypeType,  # (1)
    ThroughputCapacity: int,
    AutomaticBackupRetentionDays: NotRequired[int],
    CopyTagsToBackups: NotRequired[bool],
    CopyTagsToVolumes: NotRequired[bool],
    DailyAutomaticBackupStartTime: NotRequired[str],
    WeeklyMaintenanceStartTime: NotRequired[str],
    DiskIopsConfiguration: NotRequired[DiskIopsConfigurationTypeDef],  # (2)
    RootVolumeConfiguration: NotRequired[OpenZFSCreateRootVolumeConfigurationTypeDef],  # (3)
    PreferredSubnetId: NotRequired[str],
    EndpointIpAddressRange: NotRequired[str],
    RouteTableIds: NotRequired[Sequence[str]],
    ReadCacheConfiguration: NotRequired[OpenZFSReadCacheConfigurationTypeDef],  # (4)
```

1. See [:material-code-brackets: OpenZFSDeploymentTypeType](./literals.md#openzfsdeploymenttypetype) 
2. See [:material-code-braces: DiskIopsConfigurationTypeDef](./type_defs.md#diskiopsconfigurationtypedef) 
3. See [:material-code-braces: OpenZFSCreateRootVolumeConfigurationTypeDef](./type_defs.md#openzfscreaterootvolumeconfigurationtypedef) 
4. See [:material-code-braces: OpenZFSReadCacheConfigurationTypeDef](./type_defs.md#openzfsreadcacheconfigurationtypedef) 
## UpdateVolumeRequestRequestTypeDef

```python
# UpdateVolumeRequestRequestTypeDef definition

class UpdateVolumeRequestRequestTypeDef(TypedDict):
    VolumeId: str,
    ClientRequestToken: NotRequired[str],
    OntapConfiguration: NotRequired[UpdateOntapVolumeConfigurationTypeDef],  # (1)
    Name: NotRequired[str],
    OpenZFSConfiguration: NotRequired[UpdateOpenZFSVolumeConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: UpdateOntapVolumeConfigurationTypeDef](./type_defs.md#updateontapvolumeconfigurationtypedef) 
2. See [:material-code-braces: UpdateOpenZFSVolumeConfigurationTypeDef](./type_defs.md#updateopenzfsvolumeconfigurationtypedef) 
## AdministrativeActionPaginatorTypeDef

```python
# AdministrativeActionPaginatorTypeDef definition

class AdministrativeActionPaginatorTypeDef(TypedDict):
    AdministrativeActionType: NotRequired[AdministrativeActionTypeType],  # (1)
    ProgressPercent: NotRequired[int],
    RequestTime: NotRequired[datetime],
    Status: NotRequired[StatusType],  # (2)
    TargetFileSystemValues: NotRequired[dict[str, Any]],
    FailureDetails: NotRequired[AdministrativeActionFailureDetailsTypeDef],  # (3)
    TargetVolumeValues: NotRequired[VolumePaginatorTypeDef],  # (4)
    TargetSnapshotValues: NotRequired[SnapshotPaginatorTypeDef],  # (5)
    TotalTransferBytes: NotRequired[int],
    RemainingTransferBytes: NotRequired[int],
```

1. See [:material-code-brackets: AdministrativeActionTypeType](./literals.md#administrativeactiontypetype) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
3. See [:material-code-braces: AdministrativeActionFailureDetailsTypeDef](./type_defs.md#administrativeactionfailuredetailstypedef) 
4. See [:material-code-braces: VolumePaginatorTypeDef](./type_defs.md#volumepaginatortypedef) 
5. See [:material-code-braces: SnapshotPaginatorTypeDef](./type_defs.md#snapshotpaginatortypedef) 
## DescribeVolumesResponsePaginatorTypeDef

```python
# DescribeVolumesResponsePaginatorTypeDef definition

class DescribeVolumesResponsePaginatorTypeDef(TypedDict):
    Volumes: list[VolumePaginatorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: VolumePaginatorTypeDef](./type_defs.md#volumepaginatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AdministrativeActionTypeDef

```python
# AdministrativeActionTypeDef definition

class AdministrativeActionTypeDef(TypedDict):
    AdministrativeActionType: NotRequired[AdministrativeActionTypeType],  # (1)
    ProgressPercent: NotRequired[int],
    RequestTime: NotRequired[datetime],
    Status: NotRequired[StatusType],  # (2)
    TargetFileSystemValues: NotRequired[dict[str, Any]],
    FailureDetails: NotRequired[AdministrativeActionFailureDetailsTypeDef],  # (3)
    TargetVolumeValues: NotRequired[VolumeTypeDef],  # (4)
    TargetSnapshotValues: NotRequired[SnapshotTypeDef],  # (5)
    TotalTransferBytes: NotRequired[int],
    RemainingTransferBytes: NotRequired[int],
```

1. See [:material-code-brackets: AdministrativeActionTypeType](./literals.md#administrativeactiontypetype) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
3. See [:material-code-braces: AdministrativeActionFailureDetailsTypeDef](./type_defs.md#administrativeactionfailuredetailstypedef) 
4. See [:material-code-braces: VolumeTypeDef](./type_defs.md#volumetypedef) 
5. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
## CreateVolumeFromBackupResponseTypeDef

```python
# CreateVolumeFromBackupResponseTypeDef definition

class CreateVolumeFromBackupResponseTypeDef(TypedDict):
    Volume: VolumeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VolumeTypeDef](./type_defs.md#volumetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVolumeResponseTypeDef

```python
# CreateVolumeResponseTypeDef definition

class CreateVolumeResponseTypeDef(TypedDict):
    Volume: VolumeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VolumeTypeDef](./type_defs.md#volumetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeVolumesResponseTypeDef

```python
# DescribeVolumesResponseTypeDef definition

class DescribeVolumesResponseTypeDef(TypedDict):
    Volumes: list[VolumeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: VolumeTypeDef](./type_defs.md#volumetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateVolumeResponseTypeDef

```python
# UpdateVolumeResponseTypeDef definition

class UpdateVolumeResponseTypeDef(TypedDict):
    Volume: VolumeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VolumeTypeDef](./type_defs.md#volumetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFileSystemFromBackupRequestRequestTypeDef

```python
# CreateFileSystemFromBackupRequestRequestTypeDef definition

class CreateFileSystemFromBackupRequestRequestTypeDef(TypedDict):
    BackupId: str,
    SubnetIds: Sequence[str],
    ClientRequestToken: NotRequired[str],
    SecurityGroupIds: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    WindowsConfiguration: NotRequired[CreateFileSystemWindowsConfigurationTypeDef],  # (2)
    LustreConfiguration: NotRequired[CreateFileSystemLustreConfigurationTypeDef],  # (3)
    StorageType: NotRequired[StorageTypeType],  # (4)
    KmsKeyId: NotRequired[str],
    FileSystemTypeVersion: NotRequired[str],
    OpenZFSConfiguration: NotRequired[CreateFileSystemOpenZFSConfigurationTypeDef],  # (5)
    StorageCapacity: NotRequired[int],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateFileSystemWindowsConfigurationTypeDef](./type_defs.md#createfilesystemwindowsconfigurationtypedef) 
3. See [:material-code-braces: CreateFileSystemLustreConfigurationTypeDef](./type_defs.md#createfilesystemlustreconfigurationtypedef) 
4. See [:material-code-brackets: StorageTypeType](./literals.md#storagetypetype) 
5. See [:material-code-braces: CreateFileSystemOpenZFSConfigurationTypeDef](./type_defs.md#createfilesystemopenzfsconfigurationtypedef) 
## CreateFileSystemRequestRequestTypeDef

```python
# CreateFileSystemRequestRequestTypeDef definition

class CreateFileSystemRequestRequestTypeDef(TypedDict):
    FileSystemType: FileSystemTypeType,  # (1)
    SubnetIds: Sequence[str],
    ClientRequestToken: NotRequired[str],
    StorageCapacity: NotRequired[int],
    StorageType: NotRequired[StorageTypeType],  # (2)
    SecurityGroupIds: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    KmsKeyId: NotRequired[str],
    WindowsConfiguration: NotRequired[CreateFileSystemWindowsConfigurationTypeDef],  # (4)
    LustreConfiguration: NotRequired[CreateFileSystemLustreConfigurationTypeDef],  # (5)
    OntapConfiguration: NotRequired[CreateFileSystemOntapConfigurationTypeDef],  # (6)
    FileSystemTypeVersion: NotRequired[str],
    OpenZFSConfiguration: NotRequired[CreateFileSystemOpenZFSConfigurationTypeDef],  # (7)
```

1. See [:material-code-brackets: FileSystemTypeType](./literals.md#filesystemtypetype) 
2. See [:material-code-brackets: StorageTypeType](./literals.md#storagetypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateFileSystemWindowsConfigurationTypeDef](./type_defs.md#createfilesystemwindowsconfigurationtypedef) 
5. See [:material-code-braces: CreateFileSystemLustreConfigurationTypeDef](./type_defs.md#createfilesystemlustreconfigurationtypedef) 
6. See [:material-code-braces: CreateFileSystemOntapConfigurationTypeDef](./type_defs.md#createfilesystemontapconfigurationtypedef) 
7. See [:material-code-braces: CreateFileSystemOpenZFSConfigurationTypeDef](./type_defs.md#createfilesystemopenzfsconfigurationtypedef) 
## FileSystemPaginatorTypeDef

```python
# FileSystemPaginatorTypeDef definition

class FileSystemPaginatorTypeDef(TypedDict):
    OwnerId: NotRequired[str],
    CreationTime: NotRequired[datetime],
    FileSystemId: NotRequired[str],
    FileSystemType: NotRequired[FileSystemTypeType],  # (1)
    Lifecycle: NotRequired[FileSystemLifecycleType],  # (2)
    FailureDetails: NotRequired[FileSystemFailureDetailsTypeDef],  # (3)
    StorageCapacity: NotRequired[int],
    StorageType: NotRequired[StorageTypeType],  # (4)
    VpcId: NotRequired[str],
    SubnetIds: NotRequired[list[str]],
    NetworkInterfaceIds: NotRequired[list[str]],
    DNSName: NotRequired[str],
    KmsKeyId: NotRequired[str],
    ResourceARN: NotRequired[str],
    Tags: NotRequired[list[TagTypeDef]],  # (5)
    WindowsConfiguration: NotRequired[WindowsFileSystemConfigurationTypeDef],  # (6)
    LustreConfiguration: NotRequired[LustreFileSystemConfigurationTypeDef],  # (7)
    AdministrativeActions: NotRequired[list[AdministrativeActionPaginatorTypeDef]],  # (8)
    OntapConfiguration: NotRequired[OntapFileSystemConfigurationTypeDef],  # (9)
    FileSystemTypeVersion: NotRequired[str],
    OpenZFSConfiguration: NotRequired[OpenZFSFileSystemConfigurationTypeDef],  # (10)
```

1. See [:material-code-brackets: FileSystemTypeType](./literals.md#filesystemtypetype) 
2. See [:material-code-brackets: FileSystemLifecycleType](./literals.md#filesystemlifecycletype) 
3. See [:material-code-braces: FileSystemFailureDetailsTypeDef](./type_defs.md#filesystemfailuredetailstypedef) 
4. See [:material-code-brackets: StorageTypeType](./literals.md#storagetypetype) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: WindowsFileSystemConfigurationTypeDef](./type_defs.md#windowsfilesystemconfigurationtypedef) 
7. See [:material-code-braces: LustreFileSystemConfigurationTypeDef](./type_defs.md#lustrefilesystemconfigurationtypedef) 
8. See [:material-code-braces: AdministrativeActionPaginatorTypeDef](./type_defs.md#administrativeactionpaginatortypedef) 
9. See [:material-code-braces: OntapFileSystemConfigurationTypeDef](./type_defs.md#ontapfilesystemconfigurationtypedef) 
10. See [:material-code-braces: OpenZFSFileSystemConfigurationTypeDef](./type_defs.md#openzfsfilesystemconfigurationtypedef) 
## CopySnapshotAndUpdateVolumeResponseTypeDef

```python
# CopySnapshotAndUpdateVolumeResponseTypeDef definition

class CopySnapshotAndUpdateVolumeResponseTypeDef(TypedDict):
    VolumeId: str,
    Lifecycle: VolumeLifecycleType,  # (1)
    AdministrativeActions: list[AdministrativeActionTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: VolumeLifecycleType](./literals.md#volumelifecycletype) 
2. See [:material-code-braces: AdministrativeActionTypeDef](./type_defs.md#administrativeactiontypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FileSystemTypeDef

```python
# FileSystemTypeDef definition

class FileSystemTypeDef(TypedDict):
    OwnerId: NotRequired[str],
    CreationTime: NotRequired[datetime],
    FileSystemId: NotRequired[str],
    FileSystemType: NotRequired[FileSystemTypeType],  # (1)
    Lifecycle: NotRequired[FileSystemLifecycleType],  # (2)
    FailureDetails: NotRequired[FileSystemFailureDetailsTypeDef],  # (3)
    StorageCapacity: NotRequired[int],
    StorageType: NotRequired[StorageTypeType],  # (4)
    VpcId: NotRequired[str],
    SubnetIds: NotRequired[list[str]],
    NetworkInterfaceIds: NotRequired[list[str]],
    DNSName: NotRequired[str],
    KmsKeyId: NotRequired[str],
    ResourceARN: NotRequired[str],
    Tags: NotRequired[list[TagTypeDef]],  # (5)
    WindowsConfiguration: NotRequired[WindowsFileSystemConfigurationTypeDef],  # (6)
    LustreConfiguration: NotRequired[LustreFileSystemConfigurationTypeDef],  # (7)
    AdministrativeActions: NotRequired[list[AdministrativeActionTypeDef]],  # (8)
    OntapConfiguration: NotRequired[OntapFileSystemConfigurationTypeDef],  # (9)
    FileSystemTypeVersion: NotRequired[str],
    OpenZFSConfiguration: NotRequired[OpenZFSFileSystemConfigurationTypeDef],  # (10)
```

1. See [:material-code-brackets: FileSystemTypeType](./literals.md#filesystemtypetype) 
2. See [:material-code-brackets: FileSystemLifecycleType](./literals.md#filesystemlifecycletype) 
3. See [:material-code-braces: FileSystemFailureDetailsTypeDef](./type_defs.md#filesystemfailuredetailstypedef) 
4. See [:material-code-brackets: StorageTypeType](./literals.md#storagetypetype) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: WindowsFileSystemConfigurationTypeDef](./type_defs.md#windowsfilesystemconfigurationtypedef) 
7. See [:material-code-braces: LustreFileSystemConfigurationTypeDef](./type_defs.md#lustrefilesystemconfigurationtypedef) 
8. See [:material-code-braces: AdministrativeActionTypeDef](./type_defs.md#administrativeactiontypedef) 
9. See [:material-code-braces: OntapFileSystemConfigurationTypeDef](./type_defs.md#ontapfilesystemconfigurationtypedef) 
10. See [:material-code-braces: OpenZFSFileSystemConfigurationTypeDef](./type_defs.md#openzfsfilesystemconfigurationtypedef) 
## RestoreVolumeFromSnapshotResponseTypeDef

```python
# RestoreVolumeFromSnapshotResponseTypeDef definition

class RestoreVolumeFromSnapshotResponseTypeDef(TypedDict):
    VolumeId: str,
    Lifecycle: VolumeLifecycleType,  # (1)
    AdministrativeActions: list[AdministrativeActionTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: VolumeLifecycleType](./literals.md#volumelifecycletype) 
2. See [:material-code-braces: AdministrativeActionTypeDef](./type_defs.md#administrativeactiontypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BackupPaginatorTypeDef

```python
# BackupPaginatorTypeDef definition

class BackupPaginatorTypeDef(TypedDict):
    BackupId: str,
    Lifecycle: BackupLifecycleType,  # (1)
    Type: BackupTypeType,  # (3)
    CreationTime: datetime,
    FileSystem: FileSystemPaginatorTypeDef,  # (5)
    FailureDetails: NotRequired[BackupFailureDetailsTypeDef],  # (2)
    ProgressPercent: NotRequired[int],
    KmsKeyId: NotRequired[str],
    ResourceARN: NotRequired[str],
    Tags: NotRequired[list[TagTypeDef]],  # (4)
    DirectoryInformation: NotRequired[ActiveDirectoryBackupAttributesTypeDef],  # (6)
    OwnerId: NotRequired[str],
    SourceBackupId: NotRequired[str],
    SourceBackupRegion: NotRequired[str],
    ResourceType: NotRequired[ResourceTypeType],  # (7)
    Volume: NotRequired[VolumePaginatorTypeDef],  # (8)
    SizeInBytes: NotRequired[int],
```

1. See [:material-code-brackets: BackupLifecycleType](./literals.md#backuplifecycletype) 
2. See [:material-code-braces: BackupFailureDetailsTypeDef](./type_defs.md#backupfailuredetailstypedef) 
3. See [:material-code-brackets: BackupTypeType](./literals.md#backuptypetype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: FileSystemPaginatorTypeDef](./type_defs.md#filesystempaginatortypedef) 
6. See [:material-code-braces: ActiveDirectoryBackupAttributesTypeDef](./type_defs.md#activedirectorybackupattributestypedef) 
7. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
8. See [:material-code-braces: VolumePaginatorTypeDef](./type_defs.md#volumepaginatortypedef) 
## DescribeFileSystemsResponsePaginatorTypeDef

```python
# DescribeFileSystemsResponsePaginatorTypeDef definition

class DescribeFileSystemsResponsePaginatorTypeDef(TypedDict):
    FileSystems: list[FileSystemPaginatorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FileSystemPaginatorTypeDef](./type_defs.md#filesystempaginatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BackupTypeDef

```python
# BackupTypeDef definition

class BackupTypeDef(TypedDict):
    BackupId: str,
    Lifecycle: BackupLifecycleType,  # (1)
    Type: BackupTypeType,  # (3)
    CreationTime: datetime,
    FileSystem: FileSystemTypeDef,  # (5)
    FailureDetails: NotRequired[BackupFailureDetailsTypeDef],  # (2)
    ProgressPercent: NotRequired[int],
    KmsKeyId: NotRequired[str],
    ResourceARN: NotRequired[str],
    Tags: NotRequired[list[TagTypeDef]],  # (4)
    DirectoryInformation: NotRequired[ActiveDirectoryBackupAttributesTypeDef],  # (6)
    OwnerId: NotRequired[str],
    SourceBackupId: NotRequired[str],
    SourceBackupRegion: NotRequired[str],
    ResourceType: NotRequired[ResourceTypeType],  # (7)
    Volume: NotRequired[VolumeTypeDef],  # (8)
    SizeInBytes: NotRequired[int],
```

1. See [:material-code-brackets: BackupLifecycleType](./literals.md#backuplifecycletype) 
2. See [:material-code-braces: BackupFailureDetailsTypeDef](./type_defs.md#backupfailuredetailstypedef) 
3. See [:material-code-brackets: BackupTypeType](./literals.md#backuptypetype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: FileSystemTypeDef](./type_defs.md#filesystemtypedef) 
6. See [:material-code-braces: ActiveDirectoryBackupAttributesTypeDef](./type_defs.md#activedirectorybackupattributestypedef) 
7. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
8. See [:material-code-braces: VolumeTypeDef](./type_defs.md#volumetypedef) 
## CreateFileSystemFromBackupResponseTypeDef

```python
# CreateFileSystemFromBackupResponseTypeDef definition

class CreateFileSystemFromBackupResponseTypeDef(TypedDict):
    FileSystem: FileSystemTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FileSystemTypeDef](./type_defs.md#filesystemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFileSystemResponseTypeDef

```python
# CreateFileSystemResponseTypeDef definition

class CreateFileSystemResponseTypeDef(TypedDict):
    FileSystem: FileSystemTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FileSystemTypeDef](./type_defs.md#filesystemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFileSystemsResponseTypeDef

```python
# DescribeFileSystemsResponseTypeDef definition

class DescribeFileSystemsResponseTypeDef(TypedDict):
    FileSystems: list[FileSystemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FileSystemTypeDef](./type_defs.md#filesystemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReleaseFileSystemNfsV3LocksResponseTypeDef

```python
# ReleaseFileSystemNfsV3LocksResponseTypeDef definition

class ReleaseFileSystemNfsV3LocksResponseTypeDef(TypedDict):
    FileSystem: FileSystemTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FileSystemTypeDef](./type_defs.md#filesystemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMisconfiguredStateRecoveryResponseTypeDef

```python
# StartMisconfiguredStateRecoveryResponseTypeDef definition

class StartMisconfiguredStateRecoveryResponseTypeDef(TypedDict):
    FileSystem: FileSystemTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FileSystemTypeDef](./type_defs.md#filesystemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFileSystemResponseTypeDef

```python
# UpdateFileSystemResponseTypeDef definition

class UpdateFileSystemResponseTypeDef(TypedDict):
    FileSystem: FileSystemTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FileSystemTypeDef](./type_defs.md#filesystemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBackupsResponsePaginatorTypeDef

```python
# DescribeBackupsResponsePaginatorTypeDef definition

class DescribeBackupsResponsePaginatorTypeDef(TypedDict):
    Backups: list[BackupPaginatorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BackupPaginatorTypeDef](./type_defs.md#backuppaginatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CopyBackupResponseTypeDef

```python
# CopyBackupResponseTypeDef definition

class CopyBackupResponseTypeDef(TypedDict):
    Backup: BackupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupTypeDef](./type_defs.md#backuptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBackupResponseTypeDef

```python
# CreateBackupResponseTypeDef definition

class CreateBackupResponseTypeDef(TypedDict):
    Backup: BackupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupTypeDef](./type_defs.md#backuptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBackupsResponseTypeDef

```python
# DescribeBackupsResponseTypeDef definition

class DescribeBackupsResponseTypeDef(TypedDict):
    Backups: list[BackupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BackupTypeDef](./type_defs.md#backuptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 