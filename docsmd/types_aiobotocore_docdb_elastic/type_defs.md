# Type definitions

> [Index](../README.md) > [DocDBElastic](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [DocDBElastic](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#docdbelastic)
    type annotations stubs module [types-aiobotocore-docdb-elastic](https://pypi.org/project/types-aiobotocore-docdb-elastic/).



## ApplyPendingMaintenanceActionInputRequestTypeDef

```python
# ApplyPendingMaintenanceActionInputRequestTypeDef definition

class ApplyPendingMaintenanceActionInputRequestTypeDef(TypedDict):
    applyAction: str,
    optInType: OptInTypeType,  # (1)
    resourceArn: str,
    applyOn: NotRequired[str],
```

1. See [:material-code-brackets: OptInTypeType](./literals.md#optintypetype) 
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

## ClusterInListTypeDef

```python
# ClusterInListTypeDef definition

class ClusterInListTypeDef(TypedDict):
    clusterArn: str,
    clusterName: str,
    status: StatusType,  # (1)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## ClusterSnapshotInListTypeDef

```python
# ClusterSnapshotInListTypeDef definition

class ClusterSnapshotInListTypeDef(TypedDict):
    clusterArn: str,
    snapshotArn: str,
    snapshotCreationTime: str,
    snapshotName: str,
    status: StatusType,  # (1)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## ClusterSnapshotTypeDef

```python
# ClusterSnapshotTypeDef definition

class ClusterSnapshotTypeDef(TypedDict):
    adminUserName: str,
    clusterArn: str,
    clusterCreationTime: str,
    kmsKeyId: str,
    snapshotArn: str,
    snapshotCreationTime: str,
    snapshotName: str,
    status: StatusType,  # (2)
    subnetIds: list[str],
    vpcSecurityGroupIds: list[str],
    snapshotType: NotRequired[SnapshotTypeType],  # (1)
```

1. See [:material-code-brackets: SnapshotTypeType](./literals.md#snapshottypetype) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## ShardTypeDef

```python
# ShardTypeDef definition

class ShardTypeDef(TypedDict):
    createTime: str,
    shardId: str,
    status: StatusType,  # (1)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## CopyClusterSnapshotInputRequestTypeDef

```python
# CopyClusterSnapshotInputRequestTypeDef definition

class CopyClusterSnapshotInputRequestTypeDef(TypedDict):
    snapshotArn: str,
    targetSnapshotName: str,
    copyTags: NotRequired[bool],
    kmsKeyId: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## CreateClusterInputRequestTypeDef

```python
# CreateClusterInputRequestTypeDef definition

class CreateClusterInputRequestTypeDef(TypedDict):
    adminUserName: str,
    adminUserPassword: str,
    authType: AuthType,  # (1)
    clusterName: str,
    shardCapacity: int,
    shardCount: int,
    backupRetentionPeriod: NotRequired[int],
    clientToken: NotRequired[str],
    kmsKeyId: NotRequired[str],
    preferredBackupWindow: NotRequired[str],
    preferredMaintenanceWindow: NotRequired[str],
    shardInstanceCount: NotRequired[int],
    subnetIds: NotRequired[Sequence[str]],
    tags: NotRequired[Mapping[str, str]],
    vpcSecurityGroupIds: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: AuthType](./literals.md#authtype) 
## CreateClusterSnapshotInputRequestTypeDef

```python
# CreateClusterSnapshotInputRequestTypeDef definition

class CreateClusterSnapshotInputRequestTypeDef(TypedDict):
    clusterArn: str,
    snapshotName: str,
    tags: NotRequired[Mapping[str, str]],
```

## DeleteClusterInputRequestTypeDef

```python
# DeleteClusterInputRequestTypeDef definition

class DeleteClusterInputRequestTypeDef(TypedDict):
    clusterArn: str,
```

## DeleteClusterSnapshotInputRequestTypeDef

```python
# DeleteClusterSnapshotInputRequestTypeDef definition

class DeleteClusterSnapshotInputRequestTypeDef(TypedDict):
    snapshotArn: str,
```

## GetClusterInputRequestTypeDef

```python
# GetClusterInputRequestTypeDef definition

class GetClusterInputRequestTypeDef(TypedDict):
    clusterArn: str,
```

## GetClusterSnapshotInputRequestTypeDef

```python
# GetClusterSnapshotInputRequestTypeDef definition

class GetClusterSnapshotInputRequestTypeDef(TypedDict):
    snapshotArn: str,
```

## GetPendingMaintenanceActionInputRequestTypeDef

```python
# GetPendingMaintenanceActionInputRequestTypeDef definition

class GetPendingMaintenanceActionInputRequestTypeDef(TypedDict):
    resourceArn: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListClusterSnapshotsInputRequestTypeDef

```python
# ListClusterSnapshotsInputRequestTypeDef definition

class ListClusterSnapshotsInputRequestTypeDef(TypedDict):
    clusterArn: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    snapshotType: NotRequired[str],
```

## ListClustersInputRequestTypeDef

```python
# ListClustersInputRequestTypeDef definition

class ListClustersInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListPendingMaintenanceActionsInputRequestTypeDef

```python
# ListPendingMaintenanceActionsInputRequestTypeDef definition

class ListPendingMaintenanceActionsInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## PendingMaintenanceActionDetailsTypeDef

```python
# PendingMaintenanceActionDetailsTypeDef definition

class PendingMaintenanceActionDetailsTypeDef(TypedDict):
    action: str,
    autoAppliedAfterDate: NotRequired[str],
    currentApplyDate: NotRequired[str],
    description: NotRequired[str],
    forcedApplyDate: NotRequired[str],
    optInStatus: NotRequired[str],
```

## RestoreClusterFromSnapshotInputRequestTypeDef

```python
# RestoreClusterFromSnapshotInputRequestTypeDef definition

class RestoreClusterFromSnapshotInputRequestTypeDef(TypedDict):
    clusterName: str,
    snapshotArn: str,
    kmsKeyId: NotRequired[str],
    shardCapacity: NotRequired[int],
    shardInstanceCount: NotRequired[int],
    subnetIds: NotRequired[Sequence[str]],
    tags: NotRequired[Mapping[str, str]],
    vpcSecurityGroupIds: NotRequired[Sequence[str]],
```

## StartClusterInputRequestTypeDef

```python
# StartClusterInputRequestTypeDef definition

class StartClusterInputRequestTypeDef(TypedDict):
    clusterArn: str,
```

## StopClusterInputRequestTypeDef

```python
# StopClusterInputRequestTypeDef definition

class StopClusterInputRequestTypeDef(TypedDict):
    clusterArn: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateClusterInputRequestTypeDef

```python
# UpdateClusterInputRequestTypeDef definition

class UpdateClusterInputRequestTypeDef(TypedDict):
    clusterArn: str,
    adminUserPassword: NotRequired[str],
    authType: NotRequired[AuthType],  # (1)
    backupRetentionPeriod: NotRequired[int],
    clientToken: NotRequired[str],
    preferredBackupWindow: NotRequired[str],
    preferredMaintenanceWindow: NotRequired[str],
    shardCapacity: NotRequired[int],
    shardCount: NotRequired[int],
    shardInstanceCount: NotRequired[int],
    subnetIds: NotRequired[Sequence[str]],
    vpcSecurityGroupIds: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: AuthType](./literals.md#authtype) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListClustersOutputTypeDef

```python
# ListClustersOutputTypeDef definition

class ListClustersOutputTypeDef(TypedDict):
    clusters: list[ClusterInListTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ClusterInListTypeDef](./type_defs.md#clusterinlisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListClusterSnapshotsOutputTypeDef

```python
# ListClusterSnapshotsOutputTypeDef definition

class ListClusterSnapshotsOutputTypeDef(TypedDict):
    snapshots: list[ClusterSnapshotInListTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ClusterSnapshotInListTypeDef](./type_defs.md#clustersnapshotinlisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CopyClusterSnapshotOutputTypeDef

```python
# CopyClusterSnapshotOutputTypeDef definition

class CopyClusterSnapshotOutputTypeDef(TypedDict):
    snapshot: ClusterSnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterSnapshotTypeDef](./type_defs.md#clustersnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateClusterSnapshotOutputTypeDef

```python
# CreateClusterSnapshotOutputTypeDef definition

class CreateClusterSnapshotOutputTypeDef(TypedDict):
    snapshot: ClusterSnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterSnapshotTypeDef](./type_defs.md#clustersnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteClusterSnapshotOutputTypeDef

```python
# DeleteClusterSnapshotOutputTypeDef definition

class DeleteClusterSnapshotOutputTypeDef(TypedDict):
    snapshot: ClusterSnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterSnapshotTypeDef](./type_defs.md#clustersnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetClusterSnapshotOutputTypeDef

```python
# GetClusterSnapshotOutputTypeDef definition

class GetClusterSnapshotOutputTypeDef(TypedDict):
    snapshot: ClusterSnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterSnapshotTypeDef](./type_defs.md#clustersnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClusterTypeDef

```python
# ClusterTypeDef definition

class ClusterTypeDef(TypedDict):
    adminUserName: str,
    authType: AuthType,  # (1)
    clusterArn: str,
    clusterEndpoint: str,
    clusterName: str,
    createTime: str,
    kmsKeyId: str,
    preferredMaintenanceWindow: str,
    shardCapacity: int,
    shardCount: int,
    status: StatusType,  # (3)
    subnetIds: list[str],
    vpcSecurityGroupIds: list[str],
    backupRetentionPeriod: NotRequired[int],
    preferredBackupWindow: NotRequired[str],
    shardInstanceCount: NotRequired[int],
    shards: NotRequired[list[ShardTypeDef]],  # (2)
```

1. See [:material-code-brackets: AuthType](./literals.md#authtype) 
2. See [:material-code-braces: ShardTypeDef](./type_defs.md#shardtypedef) 
3. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## ListClusterSnapshotsInputPaginateTypeDef

```python
# ListClusterSnapshotsInputPaginateTypeDef definition

class ListClusterSnapshotsInputPaginateTypeDef(TypedDict):
    clusterArn: NotRequired[str],
    snapshotType: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListClustersInputPaginateTypeDef

```python
# ListClustersInputPaginateTypeDef definition

class ListClustersInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPendingMaintenanceActionsInputPaginateTypeDef

```python
# ListPendingMaintenanceActionsInputPaginateTypeDef definition

class ListPendingMaintenanceActionsInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ResourcePendingMaintenanceActionTypeDef

```python
# ResourcePendingMaintenanceActionTypeDef definition

class ResourcePendingMaintenanceActionTypeDef(TypedDict):
    pendingMaintenanceActionDetails: NotRequired[list[PendingMaintenanceActionDetailsTypeDef]],  # (1)
    resourceArn: NotRequired[str],
```

1. See [:material-code-braces: PendingMaintenanceActionDetailsTypeDef](./type_defs.md#pendingmaintenanceactiondetailstypedef) 
## CreateClusterOutputTypeDef

```python
# CreateClusterOutputTypeDef definition

class CreateClusterOutputTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteClusterOutputTypeDef

```python
# DeleteClusterOutputTypeDef definition

class DeleteClusterOutputTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetClusterOutputTypeDef

```python
# GetClusterOutputTypeDef definition

class GetClusterOutputTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreClusterFromSnapshotOutputTypeDef

```python
# RestoreClusterFromSnapshotOutputTypeDef definition

class RestoreClusterFromSnapshotOutputTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartClusterOutputTypeDef

```python
# StartClusterOutputTypeDef definition

class StartClusterOutputTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopClusterOutputTypeDef

```python
# StopClusterOutputTypeDef definition

class StopClusterOutputTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateClusterOutputTypeDef

```python
# UpdateClusterOutputTypeDef definition

class UpdateClusterOutputTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ApplyPendingMaintenanceActionOutputTypeDef

```python
# ApplyPendingMaintenanceActionOutputTypeDef definition

class ApplyPendingMaintenanceActionOutputTypeDef(TypedDict):
    resourcePendingMaintenanceAction: ResourcePendingMaintenanceActionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePendingMaintenanceActionTypeDef](./type_defs.md#resourcependingmaintenanceactiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPendingMaintenanceActionOutputTypeDef

```python
# GetPendingMaintenanceActionOutputTypeDef definition

class GetPendingMaintenanceActionOutputTypeDef(TypedDict):
    resourcePendingMaintenanceAction: ResourcePendingMaintenanceActionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePendingMaintenanceActionTypeDef](./type_defs.md#resourcependingmaintenanceactiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPendingMaintenanceActionsOutputTypeDef

```python
# ListPendingMaintenanceActionsOutputTypeDef definition

class ListPendingMaintenanceActionsOutputTypeDef(TypedDict):
    resourcePendingMaintenanceActions: list[ResourcePendingMaintenanceActionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourcePendingMaintenanceActionTypeDef](./type_defs.md#resourcependingmaintenanceactiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 