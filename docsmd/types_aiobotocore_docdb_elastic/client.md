# DocDBElasticClient

> [Index](../README.md) > [DocDBElastic](./README.md) > DocDBElasticClient

!!! note ""

    Auto-generated documentation for [DocDBElastic](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#docdbelastic)
    type annotations stubs module [types-aiobotocore-docdb-elastic](https://pypi.org/project/types-aiobotocore-docdb-elastic/).

## DocDBElasticClient

Type annotations and code completion for `#!python session.client("docdb-elastic")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

```python
# DocDBElasticClient usage example

from aioboto3.session import Session
from types_aiobotocore_docdb_elastic.client import DocDBElasticClient

session = Session()
async with session.client("docdb-elastic") as client:
    client: DocDBElasticClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("docdb-elastic").exceptions` structure.

```python
# DocDBElasticClient.exceptions usage example

async with session.client("docdb-elastic") as client:
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
# DocDBElasticClient.exceptions type checking example

from types_aiobotocore_docdb_elastic.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("docdb-elastic").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("docdb-elastic").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

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


### apply\_pending\_maintenance\_action

The type of pending maintenance action to be applied to the resource.

Type annotations and code completion for `#!python session.client("docdb-elastic").apply_pending_maintenance_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

```python
# apply_pending_maintenance_action method definition

await def apply_pending_maintenance_action(
    self,
    *,
    applyAction: str,
    optInType: OptInTypeType,  # (1)
    resourceArn: str,
    applyOn: str = ...,
) -> ApplyPendingMaintenanceActionOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: OptInTypeType](./literals.md#optintypetype) 
2. See [:material-code-braces: ApplyPendingMaintenanceActionOutputTypeDef](./type_defs.md#applypendingmaintenanceactionoutputtypedef) 


```python
# apply_pending_maintenance_action method usage example with argument unpacking

kwargs: ApplyPendingMaintenanceActionInputRequestTypeDef = {  # (1)
    "applyAction": ...,
    "optInType": ...,
    "resourceArn": ...,
}

parent.apply_pending_maintenance_action(**kwargs)
```

1. See [:material-code-braces: ApplyPendingMaintenanceActionInputRequestTypeDef](./type_defs.md#applypendingmaintenanceactioninputrequesttypedef) 

### copy\_cluster\_snapshot

Copies a snapshot of an elastic cluster.

Type annotations and code completion for `#!python session.client("docdb-elastic").copy_cluster_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

```python
# copy_cluster_snapshot method definition

await def copy_cluster_snapshot(
    self,
    *,
    snapshotArn: str,
    targetSnapshotName: str,
    copyTags: bool = ...,
    kmsKeyId: str = ...,
    tags: Mapping[str, str] = ...,
) -> CopyClusterSnapshotOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CopyClusterSnapshotOutputTypeDef](./type_defs.md#copyclustersnapshotoutputtypedef) 


```python
# copy_cluster_snapshot method usage example with argument unpacking

kwargs: CopyClusterSnapshotInputRequestTypeDef = {  # (1)
    "snapshotArn": ...,
    "targetSnapshotName": ...,
}

parent.copy_cluster_snapshot(**kwargs)
```

1. See [:material-code-braces: CopyClusterSnapshotInputRequestTypeDef](./type_defs.md#copyclustersnapshotinputrequesttypedef) 

### create\_cluster

Creates a new Amazon DocumentDB elastic cluster and returns its cluster
structure.

Type annotations and code completion for `#!python session.client("docdb-elastic").create_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

```python
# create_cluster method definition

await def create_cluster(
    self,
    *,
    adminUserName: str,
    adminUserPassword: str,
    authType: AuthType,  # (1)
    clusterName: str,
    shardCapacity: int,
    shardCount: int,
    backupRetentionPeriod: int = ...,
    clientToken: str = ...,
    kmsKeyId: str = ...,
    preferredBackupWindow: str = ...,
    preferredMaintenanceWindow: str = ...,
    shardInstanceCount: int = ...,
    subnetIds: Sequence[str] = ...,
    tags: Mapping[str, str] = ...,
    vpcSecurityGroupIds: Sequence[str] = ...,
) -> CreateClusterOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AuthType](./literals.md#authtype) 
2. See [:material-code-braces: CreateClusterOutputTypeDef](./type_defs.md#createclusteroutputtypedef) 


```python
# create_cluster method usage example with argument unpacking

kwargs: CreateClusterInputRequestTypeDef = {  # (1)
    "adminUserName": ...,
    "adminUserPassword": ...,
    "authType": ...,
    "clusterName": ...,
    "shardCapacity": ...,
    "shardCount": ...,
}

parent.create_cluster(**kwargs)
```

1. See [:material-code-braces: CreateClusterInputRequestTypeDef](./type_defs.md#createclusterinputrequesttypedef) 

### create\_cluster\_snapshot

Creates a snapshot of an elastic cluster.

Type annotations and code completion for `#!python session.client("docdb-elastic").create_cluster_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

```python
# create_cluster_snapshot method definition

await def create_cluster_snapshot(
    self,
    *,
    clusterArn: str,
    snapshotName: str,
    tags: Mapping[str, str] = ...,
) -> CreateClusterSnapshotOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateClusterSnapshotOutputTypeDef](./type_defs.md#createclustersnapshotoutputtypedef) 


```python
# create_cluster_snapshot method usage example with argument unpacking

kwargs: CreateClusterSnapshotInputRequestTypeDef = {  # (1)
    "clusterArn": ...,
    "snapshotName": ...,
}

parent.create_cluster_snapshot(**kwargs)
```

1. See [:material-code-braces: CreateClusterSnapshotInputRequestTypeDef](./type_defs.md#createclustersnapshotinputrequesttypedef) 

### delete\_cluster

Delete an elastic cluster.

Type annotations and code completion for `#!python session.client("docdb-elastic").delete_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

```python
# delete_cluster method definition

await def delete_cluster(
    self,
    *,
    clusterArn: str,
) -> DeleteClusterOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteClusterOutputTypeDef](./type_defs.md#deleteclusteroutputtypedef) 


```python
# delete_cluster method usage example with argument unpacking

kwargs: DeleteClusterInputRequestTypeDef = {  # (1)
    "clusterArn": ...,
}

parent.delete_cluster(**kwargs)
```

1. See [:material-code-braces: DeleteClusterInputRequestTypeDef](./type_defs.md#deleteclusterinputrequesttypedef) 

### delete\_cluster\_snapshot

Delete an elastic cluster snapshot.

Type annotations and code completion for `#!python session.client("docdb-elastic").delete_cluster_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

```python
# delete_cluster_snapshot method definition

await def delete_cluster_snapshot(
    self,
    *,
    snapshotArn: str,
) -> DeleteClusterSnapshotOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteClusterSnapshotOutputTypeDef](./type_defs.md#deleteclustersnapshotoutputtypedef) 


```python
# delete_cluster_snapshot method usage example with argument unpacking

kwargs: DeleteClusterSnapshotInputRequestTypeDef = {  # (1)
    "snapshotArn": ...,
}

parent.delete_cluster_snapshot(**kwargs)
```

1. See [:material-code-braces: DeleteClusterSnapshotInputRequestTypeDef](./type_defs.md#deleteclustersnapshotinputrequesttypedef) 

### get\_cluster

Returns information about a specific elastic cluster.

Type annotations and code completion for `#!python session.client("docdb-elastic").get_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

```python
# get_cluster method definition

await def get_cluster(
    self,
    *,
    clusterArn: str,
) -> GetClusterOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetClusterOutputTypeDef](./type_defs.md#getclusteroutputtypedef) 


```python
# get_cluster method usage example with argument unpacking

kwargs: GetClusterInputRequestTypeDef = {  # (1)
    "clusterArn": ...,
}

parent.get_cluster(**kwargs)
```

1. See [:material-code-braces: GetClusterInputRequestTypeDef](./type_defs.md#getclusterinputrequesttypedef) 

### get\_cluster\_snapshot

Returns information about a specific elastic cluster snapshot.

Type annotations and code completion for `#!python session.client("docdb-elastic").get_cluster_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

```python
# get_cluster_snapshot method definition

await def get_cluster_snapshot(
    self,
    *,
    snapshotArn: str,
) -> GetClusterSnapshotOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetClusterSnapshotOutputTypeDef](./type_defs.md#getclustersnapshotoutputtypedef) 


```python
# get_cluster_snapshot method usage example with argument unpacking

kwargs: GetClusterSnapshotInputRequestTypeDef = {  # (1)
    "snapshotArn": ...,
}

parent.get_cluster_snapshot(**kwargs)
```

1. See [:material-code-braces: GetClusterSnapshotInputRequestTypeDef](./type_defs.md#getclustersnapshotinputrequesttypedef) 

### get\_pending\_maintenance\_action

Retrieves all maintenance actions that are pending.

Type annotations and code completion for `#!python session.client("docdb-elastic").get_pending_maintenance_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

```python
# get_pending_maintenance_action method definition

await def get_pending_maintenance_action(
    self,
    *,
    resourceArn: str,
) -> GetPendingMaintenanceActionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPendingMaintenanceActionOutputTypeDef](./type_defs.md#getpendingmaintenanceactionoutputtypedef) 


```python
# get_pending_maintenance_action method usage example with argument unpacking

kwargs: GetPendingMaintenanceActionInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.get_pending_maintenance_action(**kwargs)
```

1. See [:material-code-braces: GetPendingMaintenanceActionInputRequestTypeDef](./type_defs.md#getpendingmaintenanceactioninputrequesttypedef) 

### list\_cluster\_snapshots

Returns information about snapshots for a specified elastic cluster.

Type annotations and code completion for `#!python session.client("docdb-elastic").list_cluster_snapshots` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

```python
# list_cluster_snapshots method definition

await def list_cluster_snapshots(
    self,
    *,
    clusterArn: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    snapshotType: str = ...,
) -> ListClusterSnapshotsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListClusterSnapshotsOutputTypeDef](./type_defs.md#listclustersnapshotsoutputtypedef) 


```python
# list_cluster_snapshots method usage example with argument unpacking

kwargs: ListClusterSnapshotsInputRequestTypeDef = {  # (1)
    "clusterArn": ...,
}

parent.list_cluster_snapshots(**kwargs)
```

1. See [:material-code-braces: ListClusterSnapshotsInputRequestTypeDef](./type_defs.md#listclustersnapshotsinputrequesttypedef) 

### list\_clusters

Returns information about provisioned Amazon DocumentDB elastic clusters.

Type annotations and code completion for `#!python session.client("docdb-elastic").list_clusters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

```python
# list_clusters method definition

await def list_clusters(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListClustersOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListClustersOutputTypeDef](./type_defs.md#listclustersoutputtypedef) 


```python
# list_clusters method usage example with argument unpacking

kwargs: ListClustersInputRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_clusters(**kwargs)
```

1. See [:material-code-braces: ListClustersInputRequestTypeDef](./type_defs.md#listclustersinputrequesttypedef) 

### list\_pending\_maintenance\_actions

Retrieves a list of all maintenance actions that are pending.

Type annotations and code completion for `#!python session.client("docdb-elastic").list_pending_maintenance_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

```python
# list_pending_maintenance_actions method definition

await def list_pending_maintenance_actions(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListPendingMaintenanceActionsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPendingMaintenanceActionsOutputTypeDef](./type_defs.md#listpendingmaintenanceactionsoutputtypedef) 


```python
# list_pending_maintenance_actions method usage example with argument unpacking

kwargs: ListPendingMaintenanceActionsInputRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_pending_maintenance_actions(**kwargs)
```

1. See [:material-code-braces: ListPendingMaintenanceActionsInputRequestTypeDef](./type_defs.md#listpendingmaintenanceactionsinputrequesttypedef) 

### list\_tags\_for\_resource

Lists all tags on a elastic cluster resource.

Type annotations and code completion for `#!python session.client("docdb-elastic").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

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

### restore\_cluster\_from\_snapshot

Restores an elastic cluster from a snapshot.

Type annotations and code completion for `#!python session.client("docdb-elastic").restore_cluster_from_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

```python
# restore_cluster_from_snapshot method definition

await def restore_cluster_from_snapshot(
    self,
    *,
    clusterName: str,
    snapshotArn: str,
    kmsKeyId: str = ...,
    shardCapacity: int = ...,
    shardInstanceCount: int = ...,
    subnetIds: Sequence[str] = ...,
    tags: Mapping[str, str] = ...,
    vpcSecurityGroupIds: Sequence[str] = ...,
) -> RestoreClusterFromSnapshotOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RestoreClusterFromSnapshotOutputTypeDef](./type_defs.md#restoreclusterfromsnapshotoutputtypedef) 


```python
# restore_cluster_from_snapshot method usage example with argument unpacking

kwargs: RestoreClusterFromSnapshotInputRequestTypeDef = {  # (1)
    "clusterName": ...,
    "snapshotArn": ...,
}

parent.restore_cluster_from_snapshot(**kwargs)
```

1. See [:material-code-braces: RestoreClusterFromSnapshotInputRequestTypeDef](./type_defs.md#restoreclusterfromsnapshotinputrequesttypedef) 

### start\_cluster

Restarts the stopped elastic cluster that is specified by
<code>clusterARN</code>.

Type annotations and code completion for `#!python session.client("docdb-elastic").start_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

```python
# start_cluster method definition

await def start_cluster(
    self,
    *,
    clusterArn: str,
) -> StartClusterOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartClusterOutputTypeDef](./type_defs.md#startclusteroutputtypedef) 


```python
# start_cluster method usage example with argument unpacking

kwargs: StartClusterInputRequestTypeDef = {  # (1)
    "clusterArn": ...,
}

parent.start_cluster(**kwargs)
```

1. See [:material-code-braces: StartClusterInputRequestTypeDef](./type_defs.md#startclusterinputrequesttypedef) 

### stop\_cluster

Stops the running elastic cluster that is specified by <code>clusterArn</code>.

Type annotations and code completion for `#!python session.client("docdb-elastic").stop_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

```python
# stop_cluster method definition

await def stop_cluster(
    self,
    *,
    clusterArn: str,
) -> StopClusterOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopClusterOutputTypeDef](./type_defs.md#stopclusteroutputtypedef) 


```python
# stop_cluster method usage example with argument unpacking

kwargs: StopClusterInputRequestTypeDef = {  # (1)
    "clusterArn": ...,
}

parent.stop_cluster(**kwargs)
```

1. See [:material-code-braces: StopClusterInputRequestTypeDef](./type_defs.md#stopclusterinputrequesttypedef) 

### tag\_resource

Adds metadata tags to an elastic cluster resource.

Type annotations and code completion for `#!python session.client("docdb-elastic").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> dict[str, Any]:
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

Removes metadata tags from an elastic cluster resource.

Type annotations and code completion for `#!python session.client("docdb-elastic").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> dict[str, Any]:
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

### update\_cluster

Modifies an elastic cluster.

Type annotations and code completion for `#!python session.client("docdb-elastic").update_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

```python
# update_cluster method definition

await def update_cluster(
    self,
    *,
    clusterArn: str,
    adminUserPassword: str = ...,
    authType: AuthType = ...,  # (1)
    backupRetentionPeriod: int = ...,
    clientToken: str = ...,
    preferredBackupWindow: str = ...,
    preferredMaintenanceWindow: str = ...,
    shardCapacity: int = ...,
    shardCount: int = ...,
    shardInstanceCount: int = ...,
    subnetIds: Sequence[str] = ...,
    vpcSecurityGroupIds: Sequence[str] = ...,
) -> UpdateClusterOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AuthType](./literals.md#authtype) 
2. See [:material-code-braces: UpdateClusterOutputTypeDef](./type_defs.md#updateclusteroutputtypedef) 


```python
# update_cluster method usage example with argument unpacking

kwargs: UpdateClusterInputRequestTypeDef = {  # (1)
    "clusterArn": ...,
}

parent.update_cluster(**kwargs)
```

1. See [:material-code-braces: UpdateClusterInputRequestTypeDef](./type_defs.md#updateclusterinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("docdb-elastic").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("docdb-elastic").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.client("docdb-elastic").get_paginator` method with overloads.

- `client.get_paginator("list_cluster_snapshots")` -> [ListClusterSnapshotsPaginator](./paginators.md#listclustersnapshotspaginator)
- `client.get_paginator("list_clusters")` -> [ListClustersPaginator](./paginators.md#listclusterspaginator)
- `client.get_paginator("list_pending_maintenance_actions")` -> [ListPendingMaintenanceActionsPaginator](./paginators.md#listpendingmaintenanceactionspaginator)


