# MemoryDBClient

> [Index](../README.md) > [MemoryDB](./README.md) > MemoryDBClient

!!! note ""

    Auto-generated documentation for [MemoryDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#memorydb)
    type annotations stubs module [types-aiobotocore-memorydb](https://pypi.org/project/types-aiobotocore-memorydb/).

## MemoryDBClient

Type annotations and code completion for `#!python session.client("memorydb")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# MemoryDBClient usage example

from aioboto3.session import Session
from types_aiobotocore_memorydb.client import MemoryDBClient

session = Session()
async with session.client("memorydb") as client:
    client: MemoryDBClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("memorydb").exceptions` structure.

```python
# MemoryDBClient.exceptions usage example

async with session.client("memorydb") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ACLAlreadyExistsFault,
        client.exceptions.ACLNotFoundFault,
        client.exceptions.ACLQuotaExceededFault,
        client.exceptions.APICallRateForCustomerExceededFault,
        client.exceptions.ClientError,
        client.exceptions.ClusterAlreadyExistsFault,
        client.exceptions.ClusterNotFoundFault,
        client.exceptions.ClusterQuotaForCustomerExceededFault,
        client.exceptions.DefaultUserRequired,
        client.exceptions.DuplicateUserNameFault,
        client.exceptions.InsufficientClusterCapacityFault,
        client.exceptions.InvalidACLStateFault,
        client.exceptions.InvalidARNFault,
        client.exceptions.InvalidClusterStateFault,
        client.exceptions.InvalidCredentialsException,
        client.exceptions.InvalidKMSKeyFault,
        client.exceptions.InvalidMultiRegionClusterStateFault,
        client.exceptions.InvalidNodeStateFault,
        client.exceptions.InvalidParameterCombinationException,
        client.exceptions.InvalidParameterGroupStateFault,
        client.exceptions.InvalidParameterValueException,
        client.exceptions.InvalidSnapshotStateFault,
        client.exceptions.InvalidSubnet,
        client.exceptions.InvalidUserStateFault,
        client.exceptions.InvalidVPCNetworkStateFault,
        client.exceptions.MultiRegionClusterAlreadyExistsFault,
        client.exceptions.MultiRegionClusterNotFoundFault,
        client.exceptions.MultiRegionParameterGroupNotFoundFault,
        client.exceptions.NoOperationFault,
        client.exceptions.NodeQuotaForClusterExceededFault,
        client.exceptions.NodeQuotaForCustomerExceededFault,
        client.exceptions.ParameterGroupAlreadyExistsFault,
        client.exceptions.ParameterGroupNotFoundFault,
        client.exceptions.ParameterGroupQuotaExceededFault,
        client.exceptions.ReservedNodeAlreadyExistsFault,
        client.exceptions.ReservedNodeNotFoundFault,
        client.exceptions.ReservedNodeQuotaExceededFault,
        client.exceptions.ReservedNodesOfferingNotFoundFault,
        client.exceptions.ServiceLinkedRoleNotFoundFault,
        client.exceptions.ServiceUpdateNotFoundFault,
        client.exceptions.ShardNotFoundFault,
        client.exceptions.ShardsPerClusterQuotaExceededFault,
        client.exceptions.SnapshotAlreadyExistsFault,
        client.exceptions.SnapshotNotFoundFault,
        client.exceptions.SnapshotQuotaExceededFault,
        client.exceptions.SubnetGroupAlreadyExistsFault,
        client.exceptions.SubnetGroupInUseFault,
        client.exceptions.SubnetGroupNotFoundFault,
        client.exceptions.SubnetGroupQuotaExceededFault,
        client.exceptions.SubnetInUse,
        client.exceptions.SubnetNotAllowedFault,
        client.exceptions.SubnetQuotaExceededFault,
        client.exceptions.TagNotFoundFault,
        client.exceptions.TagQuotaPerResourceExceeded,
        client.exceptions.TestFailoverNotAvailableFault,
        client.exceptions.UserAlreadyExistsFault,
        client.exceptions.UserNotFoundFault,
        client.exceptions.UserQuotaExceededFault,
    ) as e:
        print(e)
```

```python
# MemoryDBClient.exceptions type checking example

from types_aiobotocore_memorydb.client import Exceptions

def handle_error(exc: Exceptions.ACLAlreadyExistsFault) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("memorydb").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("memorydb").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

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


### batch\_update\_cluster

Apply the service update to a list of clusters supplied.

Type annotations and code completion for `#!python session.client("memorydb").batch_update_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# batch_update_cluster method definition

await def batch_update_cluster(
    self,
    *,
    ClusterNames: Sequence[str],
    ServiceUpdate: ServiceUpdateRequestTypeDef = ...,  # (1)
) -> BatchUpdateClusterResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ServiceUpdateRequestTypeDef](./type_defs.md#serviceupdaterequesttypedef) 
2. See [:material-code-braces: BatchUpdateClusterResponseTypeDef](./type_defs.md#batchupdateclusterresponsetypedef) 


```python
# batch_update_cluster method usage example with argument unpacking

kwargs: BatchUpdateClusterRequestRequestTypeDef = {  # (1)
    "ClusterNames": ...,
}

parent.batch_update_cluster(**kwargs)
```

1. See [:material-code-braces: BatchUpdateClusterRequestRequestTypeDef](./type_defs.md#batchupdateclusterrequestrequesttypedef) 

### copy\_snapshot

Makes a copy of an existing snapshot.

Type annotations and code completion for `#!python session.client("memorydb").copy_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# copy_snapshot method definition

await def copy_snapshot(
    self,
    *,
    SourceSnapshotName: str,
    TargetSnapshotName: str,
    TargetBucket: str = ...,
    KmsKeyId: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CopySnapshotResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CopySnapshotResponseTypeDef](./type_defs.md#copysnapshotresponsetypedef) 


```python
# copy_snapshot method usage example with argument unpacking

kwargs: CopySnapshotRequestRequestTypeDef = {  # (1)
    "SourceSnapshotName": ...,
    "TargetSnapshotName": ...,
}

parent.copy_snapshot(**kwargs)
```

1. See [:material-code-braces: CopySnapshotRequestRequestTypeDef](./type_defs.md#copysnapshotrequestrequesttypedef) 

### create\_acl

Creates an Access Control List.

Type annotations and code completion for `#!python session.client("memorydb").create_acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# create_acl method definition

await def create_acl(
    self,
    *,
    ACLName: str,
    UserNames: Sequence[str] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateACLResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateACLResponseTypeDef](./type_defs.md#createaclresponsetypedef) 


```python
# create_acl method usage example with argument unpacking

kwargs: CreateACLRequestRequestTypeDef = {  # (1)
    "ACLName": ...,
}

parent.create_acl(**kwargs)
```

1. See [:material-code-braces: CreateACLRequestRequestTypeDef](./type_defs.md#createaclrequestrequesttypedef) 

### create\_cluster

Creates a cluster.

Type annotations and code completion for `#!python session.client("memorydb").create_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# create_cluster method definition

await def create_cluster(
    self,
    *,
    ClusterName: str,
    NodeType: str,
    ACLName: str,
    MultiRegionClusterName: str = ...,
    ParameterGroupName: str = ...,
    Description: str = ...,
    NumShards: int = ...,
    NumReplicasPerShard: int = ...,
    SubnetGroupName: str = ...,
    SecurityGroupIds: Sequence[str] = ...,
    MaintenanceWindow: str = ...,
    Port: int = ...,
    SnsTopicArn: str = ...,
    TLSEnabled: bool = ...,
    KmsKeyId: str = ...,
    SnapshotArns: Sequence[str] = ...,
    SnapshotName: str = ...,
    SnapshotRetentionLimit: int = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
    SnapshotWindow: str = ...,
    Engine: str = ...,
    EngineVersion: str = ...,
    AutoMinorVersionUpgrade: bool = ...,
    DataTiering: bool = ...,
) -> CreateClusterResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateClusterResponseTypeDef](./type_defs.md#createclusterresponsetypedef) 


```python
# create_cluster method usage example with argument unpacking

kwargs: CreateClusterRequestRequestTypeDef = {  # (1)
    "ClusterName": ...,
    "NodeType": ...,
    "ACLName": ...,
}

parent.create_cluster(**kwargs)
```

1. See [:material-code-braces: CreateClusterRequestRequestTypeDef](./type_defs.md#createclusterrequestrequesttypedef) 

### create\_multi\_region\_cluster

Creates a new multi-Region cluster.

Type annotations and code completion for `#!python session.client("memorydb").create_multi_region_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# create_multi_region_cluster method definition

await def create_multi_region_cluster(
    self,
    *,
    MultiRegionClusterNameSuffix: str,
    NodeType: str,
    Description: str = ...,
    Engine: str = ...,
    EngineVersion: str = ...,
    MultiRegionParameterGroupName: str = ...,
    NumShards: int = ...,
    TLSEnabled: bool = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateMultiRegionClusterResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateMultiRegionClusterResponseTypeDef](./type_defs.md#createmultiregionclusterresponsetypedef) 


```python
# create_multi_region_cluster method usage example with argument unpacking

kwargs: CreateMultiRegionClusterRequestRequestTypeDef = {  # (1)
    "MultiRegionClusterNameSuffix": ...,
    "NodeType": ...,
}

parent.create_multi_region_cluster(**kwargs)
```

1. See [:material-code-braces: CreateMultiRegionClusterRequestRequestTypeDef](./type_defs.md#createmultiregionclusterrequestrequesttypedef) 

### create\_parameter\_group

Creates a new MemoryDB parameter group.

Type annotations and code completion for `#!python session.client("memorydb").create_parameter_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# create_parameter_group method definition

await def create_parameter_group(
    self,
    *,
    ParameterGroupName: str,
    Family: str,
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateParameterGroupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateParameterGroupResponseTypeDef](./type_defs.md#createparametergroupresponsetypedef) 


```python
# create_parameter_group method usage example with argument unpacking

kwargs: CreateParameterGroupRequestRequestTypeDef = {  # (1)
    "ParameterGroupName": ...,
    "Family": ...,
}

parent.create_parameter_group(**kwargs)
```

1. See [:material-code-braces: CreateParameterGroupRequestRequestTypeDef](./type_defs.md#createparametergrouprequestrequesttypedef) 

### create\_snapshot

Creates a copy of an entire cluster at a specific moment in time.

Type annotations and code completion for `#!python session.client("memorydb").create_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# create_snapshot method definition

await def create_snapshot(
    self,
    *,
    ClusterName: str,
    SnapshotName: str,
    KmsKeyId: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateSnapshotResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateSnapshotResponseTypeDef](./type_defs.md#createsnapshotresponsetypedef) 


```python
# create_snapshot method usage example with argument unpacking

kwargs: CreateSnapshotRequestRequestTypeDef = {  # (1)
    "ClusterName": ...,
    "SnapshotName": ...,
}

parent.create_snapshot(**kwargs)
```

1. See [:material-code-braces: CreateSnapshotRequestRequestTypeDef](./type_defs.md#createsnapshotrequestrequesttypedef) 

### create\_subnet\_group

Creates a subnet group.

Type annotations and code completion for `#!python session.client("memorydb").create_subnet_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# create_subnet_group method definition

await def create_subnet_group(
    self,
    *,
    SubnetGroupName: str,
    SubnetIds: Sequence[str],
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateSubnetGroupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateSubnetGroupResponseTypeDef](./type_defs.md#createsubnetgroupresponsetypedef) 


```python
# create_subnet_group method usage example with argument unpacking

kwargs: CreateSubnetGroupRequestRequestTypeDef = {  # (1)
    "SubnetGroupName": ...,
    "SubnetIds": ...,
}

parent.create_subnet_group(**kwargs)
```

1. See [:material-code-braces: CreateSubnetGroupRequestRequestTypeDef](./type_defs.md#createsubnetgrouprequestrequesttypedef) 

### create\_user

Creates a MemoryDB user.

Type annotations and code completion for `#!python session.client("memorydb").create_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# create_user method definition

await def create_user(
    self,
    *,
    UserName: str,
    AuthenticationMode: AuthenticationModeTypeDef,  # (1)
    AccessString: str,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateUserResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AuthenticationModeTypeDef](./type_defs.md#authenticationmodetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateUserResponseTypeDef](./type_defs.md#createuserresponsetypedef) 


```python
# create_user method usage example with argument unpacking

kwargs: CreateUserRequestRequestTypeDef = {  # (1)
    "UserName": ...,
    "AuthenticationMode": ...,
    "AccessString": ...,
}

parent.create_user(**kwargs)
```

1. See [:material-code-braces: CreateUserRequestRequestTypeDef](./type_defs.md#createuserrequestrequesttypedef) 

### delete\_acl

Deletes an Access Control List.

Type annotations and code completion for `#!python session.client("memorydb").delete_acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# delete_acl method definition

await def delete_acl(
    self,
    *,
    ACLName: str,
) -> DeleteACLResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteACLResponseTypeDef](./type_defs.md#deleteaclresponsetypedef) 


```python
# delete_acl method usage example with argument unpacking

kwargs: DeleteACLRequestRequestTypeDef = {  # (1)
    "ACLName": ...,
}

parent.delete_acl(**kwargs)
```

1. See [:material-code-braces: DeleteACLRequestRequestTypeDef](./type_defs.md#deleteaclrequestrequesttypedef) 

### delete\_cluster

Deletes a cluster.

Type annotations and code completion for `#!python session.client("memorydb").delete_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# delete_cluster method definition

await def delete_cluster(
    self,
    *,
    ClusterName: str,
    MultiRegionClusterName: str = ...,
    FinalSnapshotName: str = ...,
) -> DeleteClusterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteClusterResponseTypeDef](./type_defs.md#deleteclusterresponsetypedef) 


```python
# delete_cluster method usage example with argument unpacking

kwargs: DeleteClusterRequestRequestTypeDef = {  # (1)
    "ClusterName": ...,
}

parent.delete_cluster(**kwargs)
```

1. See [:material-code-braces: DeleteClusterRequestRequestTypeDef](./type_defs.md#deleteclusterrequestrequesttypedef) 

### delete\_multi\_region\_cluster

Deletes an existing multi-Region cluster.

Type annotations and code completion for `#!python session.client("memorydb").delete_multi_region_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# delete_multi_region_cluster method definition

await def delete_multi_region_cluster(
    self,
    *,
    MultiRegionClusterName: str,
) -> DeleteMultiRegionClusterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteMultiRegionClusterResponseTypeDef](./type_defs.md#deletemultiregionclusterresponsetypedef) 


```python
# delete_multi_region_cluster method usage example with argument unpacking

kwargs: DeleteMultiRegionClusterRequestRequestTypeDef = {  # (1)
    "MultiRegionClusterName": ...,
}

parent.delete_multi_region_cluster(**kwargs)
```

1. See [:material-code-braces: DeleteMultiRegionClusterRequestRequestTypeDef](./type_defs.md#deletemultiregionclusterrequestrequesttypedef) 

### delete\_parameter\_group

Deletes the specified parameter group.

Type annotations and code completion for `#!python session.client("memorydb").delete_parameter_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# delete_parameter_group method definition

await def delete_parameter_group(
    self,
    *,
    ParameterGroupName: str,
) -> DeleteParameterGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteParameterGroupResponseTypeDef](./type_defs.md#deleteparametergroupresponsetypedef) 


```python
# delete_parameter_group method usage example with argument unpacking

kwargs: DeleteParameterGroupRequestRequestTypeDef = {  # (1)
    "ParameterGroupName": ...,
}

parent.delete_parameter_group(**kwargs)
```

1. See [:material-code-braces: DeleteParameterGroupRequestRequestTypeDef](./type_defs.md#deleteparametergrouprequestrequesttypedef) 

### delete\_snapshot

Deletes an existing snapshot.

Type annotations and code completion for `#!python session.client("memorydb").delete_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# delete_snapshot method definition

await def delete_snapshot(
    self,
    *,
    SnapshotName: str,
) -> DeleteSnapshotResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteSnapshotResponseTypeDef](./type_defs.md#deletesnapshotresponsetypedef) 


```python
# delete_snapshot method usage example with argument unpacking

kwargs: DeleteSnapshotRequestRequestTypeDef = {  # (1)
    "SnapshotName": ...,
}

parent.delete_snapshot(**kwargs)
```

1. See [:material-code-braces: DeleteSnapshotRequestRequestTypeDef](./type_defs.md#deletesnapshotrequestrequesttypedef) 

### delete\_subnet\_group

Deletes a subnet group.

Type annotations and code completion for `#!python session.client("memorydb").delete_subnet_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# delete_subnet_group method definition

await def delete_subnet_group(
    self,
    *,
    SubnetGroupName: str,
) -> DeleteSubnetGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteSubnetGroupResponseTypeDef](./type_defs.md#deletesubnetgroupresponsetypedef) 


```python
# delete_subnet_group method usage example with argument unpacking

kwargs: DeleteSubnetGroupRequestRequestTypeDef = {  # (1)
    "SubnetGroupName": ...,
}

parent.delete_subnet_group(**kwargs)
```

1. See [:material-code-braces: DeleteSubnetGroupRequestRequestTypeDef](./type_defs.md#deletesubnetgrouprequestrequesttypedef) 

### delete\_user

Deletes a user.

Type annotations and code completion for `#!python session.client("memorydb").delete_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# delete_user method definition

await def delete_user(
    self,
    *,
    UserName: str,
) -> DeleteUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteUserResponseTypeDef](./type_defs.md#deleteuserresponsetypedef) 


```python
# delete_user method usage example with argument unpacking

kwargs: DeleteUserRequestRequestTypeDef = {  # (1)
    "UserName": ...,
}

parent.delete_user(**kwargs)
```

1. See [:material-code-braces: DeleteUserRequestRequestTypeDef](./type_defs.md#deleteuserrequestrequesttypedef) 

### describe\_acls

Returns a list of ACLs.

Type annotations and code completion for `#!python session.client("memorydb").describe_acls` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# describe_acls method definition

await def describe_acls(
    self,
    *,
    ACLName: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeACLsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeACLsResponseTypeDef](./type_defs.md#describeaclsresponsetypedef) 


```python
# describe_acls method usage example with argument unpacking

kwargs: DescribeACLsRequestRequestTypeDef = {  # (1)
    "ACLName": ...,
}

parent.describe_acls(**kwargs)
```

1. See [:material-code-braces: DescribeACLsRequestRequestTypeDef](./type_defs.md#describeaclsrequestrequesttypedef) 

### describe\_clusters

Returns information about all provisioned clusters if no cluster identifier is
specified, or about a specific cluster if a cluster name is supplied.

Type annotations and code completion for `#!python session.client("memorydb").describe_clusters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# describe_clusters method definition

await def describe_clusters(
    self,
    *,
    ClusterName: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    ShowShardDetails: bool = ...,
) -> DescribeClustersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeClustersResponseTypeDef](./type_defs.md#describeclustersresponsetypedef) 


```python
# describe_clusters method usage example with argument unpacking

kwargs: DescribeClustersRequestRequestTypeDef = {  # (1)
    "ClusterName": ...,
}

parent.describe_clusters(**kwargs)
```

1. See [:material-code-braces: DescribeClustersRequestRequestTypeDef](./type_defs.md#describeclustersrequestrequesttypedef) 

### describe\_engine\_versions

Returns a list of the available Redis OSS engine versions.

Type annotations and code completion for `#!python session.client("memorydb").describe_engine_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# describe_engine_versions method definition

await def describe_engine_versions(
    self,
    *,
    Engine: str = ...,
    EngineVersion: str = ...,
    ParameterGroupFamily: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    DefaultOnly: bool = ...,
) -> DescribeEngineVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEngineVersionsResponseTypeDef](./type_defs.md#describeengineversionsresponsetypedef) 


```python
# describe_engine_versions method usage example with argument unpacking

kwargs: DescribeEngineVersionsRequestRequestTypeDef = {  # (1)
    "Engine": ...,
}

parent.describe_engine_versions(**kwargs)
```

1. See [:material-code-braces: DescribeEngineVersionsRequestRequestTypeDef](./type_defs.md#describeengineversionsrequestrequesttypedef) 

### describe\_events

Returns events related to clusters, security groups, and parameter groups.

Type annotations and code completion for `#!python session.client("memorydb").describe_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# describe_events method definition

await def describe_events(
    self,
    *,
    SourceName: str = ...,
    SourceType: SourceTypeType = ...,  # (1)
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    Duration: int = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeEventsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-braces: DescribeEventsResponseTypeDef](./type_defs.md#describeeventsresponsetypedef) 


```python
# describe_events method usage example with argument unpacking

kwargs: DescribeEventsRequestRequestTypeDef = {  # (1)
    "SourceName": ...,
}

parent.describe_events(**kwargs)
```

1. See [:material-code-braces: DescribeEventsRequestRequestTypeDef](./type_defs.md#describeeventsrequestrequesttypedef) 

### describe\_multi\_region\_clusters

Returns details about one or more multi-Region clusters.

Type annotations and code completion for `#!python session.client("memorydb").describe_multi_region_clusters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# describe_multi_region_clusters method definition

await def describe_multi_region_clusters(
    self,
    *,
    MultiRegionClusterName: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    ShowClusterDetails: bool = ...,
) -> DescribeMultiRegionClustersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeMultiRegionClustersResponseTypeDef](./type_defs.md#describemultiregionclustersresponsetypedef) 


```python
# describe_multi_region_clusters method usage example with argument unpacking

kwargs: DescribeMultiRegionClustersRequestRequestTypeDef = {  # (1)
    "MultiRegionClusterName": ...,
}

parent.describe_multi_region_clusters(**kwargs)
```

1. See [:material-code-braces: DescribeMultiRegionClustersRequestRequestTypeDef](./type_defs.md#describemultiregionclustersrequestrequesttypedef) 

### describe\_parameter\_groups

Returns a list of parameter group descriptions.

Type annotations and code completion for `#!python session.client("memorydb").describe_parameter_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# describe_parameter_groups method definition

await def describe_parameter_groups(
    self,
    *,
    ParameterGroupName: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeParameterGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeParameterGroupsResponseTypeDef](./type_defs.md#describeparametergroupsresponsetypedef) 


```python
# describe_parameter_groups method usage example with argument unpacking

kwargs: DescribeParameterGroupsRequestRequestTypeDef = {  # (1)
    "ParameterGroupName": ...,
}

parent.describe_parameter_groups(**kwargs)
```

1. See [:material-code-braces: DescribeParameterGroupsRequestRequestTypeDef](./type_defs.md#describeparametergroupsrequestrequesttypedef) 

### describe\_parameters

Returns the detailed parameter list for a particular parameter group.

Type annotations and code completion for `#!python session.client("memorydb").describe_parameters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# describe_parameters method definition

await def describe_parameters(
    self,
    *,
    ParameterGroupName: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeParametersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeParametersResponseTypeDef](./type_defs.md#describeparametersresponsetypedef) 


```python
# describe_parameters method usage example with argument unpacking

kwargs: DescribeParametersRequestRequestTypeDef = {  # (1)
    "ParameterGroupName": ...,
}

parent.describe_parameters(**kwargs)
```

1. See [:material-code-braces: DescribeParametersRequestRequestTypeDef](./type_defs.md#describeparametersrequestrequesttypedef) 

### describe\_reserved\_nodes

Returns information about reserved nodes for this account, or about a specified
reserved node.

Type annotations and code completion for `#!python session.client("memorydb").describe_reserved_nodes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# describe_reserved_nodes method definition

await def describe_reserved_nodes(
    self,
    *,
    ReservationId: str = ...,
    ReservedNodesOfferingId: str = ...,
    NodeType: str = ...,
    Duration: str = ...,
    OfferingType: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeReservedNodesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeReservedNodesResponseTypeDef](./type_defs.md#describereservednodesresponsetypedef) 


```python
# describe_reserved_nodes method usage example with argument unpacking

kwargs: DescribeReservedNodesRequestRequestTypeDef = {  # (1)
    "ReservationId": ...,
}

parent.describe_reserved_nodes(**kwargs)
```

1. See [:material-code-braces: DescribeReservedNodesRequestRequestTypeDef](./type_defs.md#describereservednodesrequestrequesttypedef) 

### describe\_reserved\_nodes\_offerings

Lists available reserved node offerings.

Type annotations and code completion for `#!python session.client("memorydb").describe_reserved_nodes_offerings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# describe_reserved_nodes_offerings method definition

await def describe_reserved_nodes_offerings(
    self,
    *,
    ReservedNodesOfferingId: str = ...,
    NodeType: str = ...,
    Duration: str = ...,
    OfferingType: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeReservedNodesOfferingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeReservedNodesOfferingsResponseTypeDef](./type_defs.md#describereservednodesofferingsresponsetypedef) 


```python
# describe_reserved_nodes_offerings method usage example with argument unpacking

kwargs: DescribeReservedNodesOfferingsRequestRequestTypeDef = {  # (1)
    "ReservedNodesOfferingId": ...,
}

parent.describe_reserved_nodes_offerings(**kwargs)
```

1. See [:material-code-braces: DescribeReservedNodesOfferingsRequestRequestTypeDef](./type_defs.md#describereservednodesofferingsrequestrequesttypedef) 

### describe\_service\_updates

Returns details of the service updates.

Type annotations and code completion for `#!python session.client("memorydb").describe_service_updates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# describe_service_updates method definition

await def describe_service_updates(
    self,
    *,
    ServiceUpdateName: str = ...,
    ClusterNames: Sequence[str] = ...,
    Status: Sequence[ServiceUpdateStatusType] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeServiceUpdatesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ServiceUpdateStatusType](./literals.md#serviceupdatestatustype) 
2. See [:material-code-braces: DescribeServiceUpdatesResponseTypeDef](./type_defs.md#describeserviceupdatesresponsetypedef) 


```python
# describe_service_updates method usage example with argument unpacking

kwargs: DescribeServiceUpdatesRequestRequestTypeDef = {  # (1)
    "ServiceUpdateName": ...,
}

parent.describe_service_updates(**kwargs)
```

1. See [:material-code-braces: DescribeServiceUpdatesRequestRequestTypeDef](./type_defs.md#describeserviceupdatesrequestrequesttypedef) 

### describe\_snapshots

Returns information about cluster snapshots.

Type annotations and code completion for `#!python session.client("memorydb").describe_snapshots` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# describe_snapshots method definition

await def describe_snapshots(
    self,
    *,
    ClusterName: str = ...,
    SnapshotName: str = ...,
    Source: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    ShowDetail: bool = ...,
) -> DescribeSnapshotsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSnapshotsResponseTypeDef](./type_defs.md#describesnapshotsresponsetypedef) 


```python
# describe_snapshots method usage example with argument unpacking

kwargs: DescribeSnapshotsRequestRequestTypeDef = {  # (1)
    "ClusterName": ...,
}

parent.describe_snapshots(**kwargs)
```

1. See [:material-code-braces: DescribeSnapshotsRequestRequestTypeDef](./type_defs.md#describesnapshotsrequestrequesttypedef) 

### describe\_subnet\_groups

Returns a list of subnet group descriptions.

Type annotations and code completion for `#!python session.client("memorydb").describe_subnet_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# describe_subnet_groups method definition

await def describe_subnet_groups(
    self,
    *,
    SubnetGroupName: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeSubnetGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSubnetGroupsResponseTypeDef](./type_defs.md#describesubnetgroupsresponsetypedef) 


```python
# describe_subnet_groups method usage example with argument unpacking

kwargs: DescribeSubnetGroupsRequestRequestTypeDef = {  # (1)
    "SubnetGroupName": ...,
}

parent.describe_subnet_groups(**kwargs)
```

1. See [:material-code-braces: DescribeSubnetGroupsRequestRequestTypeDef](./type_defs.md#describesubnetgroupsrequestrequesttypedef) 

### describe\_users

Returns a list of users.

Type annotations and code completion for `#!python session.client("memorydb").describe_users` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# describe_users method definition

await def describe_users(
    self,
    *,
    UserName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeUsersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeUsersResponseTypeDef](./type_defs.md#describeusersresponsetypedef) 


```python
# describe_users method usage example with argument unpacking

kwargs: DescribeUsersRequestRequestTypeDef = {  # (1)
    "UserName": ...,
}

parent.describe_users(**kwargs)
```

1. See [:material-code-braces: DescribeUsersRequestRequestTypeDef](./type_defs.md#describeusersrequestrequesttypedef) 

### failover\_shard

Used to failover a shard.

Type annotations and code completion for `#!python session.client("memorydb").failover_shard` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# failover_shard method definition

await def failover_shard(
    self,
    *,
    ClusterName: str,
    ShardName: str,
) -> FailoverShardResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: FailoverShardResponseTypeDef](./type_defs.md#failovershardresponsetypedef) 


```python
# failover_shard method usage example with argument unpacking

kwargs: FailoverShardRequestRequestTypeDef = {  # (1)
    "ClusterName": ...,
    "ShardName": ...,
}

parent.failover_shard(**kwargs)
```

1. See [:material-code-braces: FailoverShardRequestRequestTypeDef](./type_defs.md#failovershardrequestrequesttypedef) 

### list\_allowed\_multi\_region\_cluster\_updates

Lists the allowed updates for a multi-Region cluster.

Type annotations and code completion for `#!python session.client("memorydb").list_allowed_multi_region_cluster_updates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# list_allowed_multi_region_cluster_updates method definition

await def list_allowed_multi_region_cluster_updates(
    self,
    *,
    MultiRegionClusterName: str,
) -> ListAllowedMultiRegionClusterUpdatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAllowedMultiRegionClusterUpdatesResponseTypeDef](./type_defs.md#listallowedmultiregionclusterupdatesresponsetypedef) 


```python
# list_allowed_multi_region_cluster_updates method usage example with argument unpacking

kwargs: ListAllowedMultiRegionClusterUpdatesRequestRequestTypeDef = {  # (1)
    "MultiRegionClusterName": ...,
}

parent.list_allowed_multi_region_cluster_updates(**kwargs)
```

1. See [:material-code-braces: ListAllowedMultiRegionClusterUpdatesRequestRequestTypeDef](./type_defs.md#listallowedmultiregionclusterupdatesrequestrequesttypedef) 

### list\_allowed\_node\_type\_updates

Lists all available node types that you can scale to from your cluster's
current node type.

Type annotations and code completion for `#!python session.client("memorydb").list_allowed_node_type_updates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# list_allowed_node_type_updates method definition

await def list_allowed_node_type_updates(
    self,
    *,
    ClusterName: str,
) -> ListAllowedNodeTypeUpdatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAllowedNodeTypeUpdatesResponseTypeDef](./type_defs.md#listallowednodetypeupdatesresponsetypedef) 


```python
# list_allowed_node_type_updates method usage example with argument unpacking

kwargs: ListAllowedNodeTypeUpdatesRequestRequestTypeDef = {  # (1)
    "ClusterName": ...,
}

parent.list_allowed_node_type_updates(**kwargs)
```

1. See [:material-code-braces: ListAllowedNodeTypeUpdatesRequestRequestTypeDef](./type_defs.md#listallowednodetypeupdatesrequestrequesttypedef) 

### list\_tags

Lists all tags currently on a named resource.

Type annotations and code completion for `#!python session.client("memorydb").list_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# list_tags method definition

await def list_tags(
    self,
    *,
    ResourceArn: str,
) -> ListTagsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef) 


```python
# list_tags method usage example with argument unpacking

kwargs: ListTagsRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags(**kwargs)
```

1. See [:material-code-braces: ListTagsRequestRequestTypeDef](./type_defs.md#listtagsrequestrequesttypedef) 

### purchase\_reserved\_nodes\_offering

Allows you to purchase a reserved node offering.

Type annotations and code completion for `#!python session.client("memorydb").purchase_reserved_nodes_offering` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# purchase_reserved_nodes_offering method definition

await def purchase_reserved_nodes_offering(
    self,
    *,
    ReservedNodesOfferingId: str,
    ReservationId: str = ...,
    NodeCount: int = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> PurchaseReservedNodesOfferingResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: PurchaseReservedNodesOfferingResponseTypeDef](./type_defs.md#purchasereservednodesofferingresponsetypedef) 


```python
# purchase_reserved_nodes_offering method usage example with argument unpacking

kwargs: PurchaseReservedNodesOfferingRequestRequestTypeDef = {  # (1)
    "ReservedNodesOfferingId": ...,
}

parent.purchase_reserved_nodes_offering(**kwargs)
```

1. See [:material-code-braces: PurchaseReservedNodesOfferingRequestRequestTypeDef](./type_defs.md#purchasereservednodesofferingrequestrequesttypedef) 

### reset\_parameter\_group

Modifies the parameters of a parameter group to the engine or system default
value.

Type annotations and code completion for `#!python session.client("memorydb").reset_parameter_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# reset_parameter_group method definition

await def reset_parameter_group(
    self,
    *,
    ParameterGroupName: str,
    AllParameters: bool = ...,
    ParameterNames: Sequence[str] = ...,
) -> ResetParameterGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ResetParameterGroupResponseTypeDef](./type_defs.md#resetparametergroupresponsetypedef) 


```python
# reset_parameter_group method usage example with argument unpacking

kwargs: ResetParameterGroupRequestRequestTypeDef = {  # (1)
    "ParameterGroupName": ...,
}

parent.reset_parameter_group(**kwargs)
```

1. See [:material-code-braces: ResetParameterGroupRequestRequestTypeDef](./type_defs.md#resetparametergrouprequestrequesttypedef) 

### tag\_resource

A tag is a key-value pair where the key and value are case-sensitive.

Type annotations and code completion for `#!python session.client("memorydb").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> TagResourceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: TagResourceResponseTypeDef](./type_defs.md#tagresourceresponsetypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Use this operation to remove tags on a resource.

Type annotations and code completion for `#!python session.client("memorydb").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> UntagResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UntagResourceResponseTypeDef](./type_defs.md#untagresourceresponsetypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_acl

Changes the list of users that belong to the Access Control List.

Type annotations and code completion for `#!python session.client("memorydb").update_acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# update_acl method definition

await def update_acl(
    self,
    *,
    ACLName: str,
    UserNamesToAdd: Sequence[str] = ...,
    UserNamesToRemove: Sequence[str] = ...,
) -> UpdateACLResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateACLResponseTypeDef](./type_defs.md#updateaclresponsetypedef) 


```python
# update_acl method usage example with argument unpacking

kwargs: UpdateACLRequestRequestTypeDef = {  # (1)
    "ACLName": ...,
}

parent.update_acl(**kwargs)
```

1. See [:material-code-braces: UpdateACLRequestRequestTypeDef](./type_defs.md#updateaclrequestrequesttypedef) 

### update\_cluster

Modifies the settings for a cluster.

Type annotations and code completion for `#!python session.client("memorydb").update_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# update_cluster method definition

await def update_cluster(
    self,
    *,
    ClusterName: str,
    Description: str = ...,
    SecurityGroupIds: Sequence[str] = ...,
    MaintenanceWindow: str = ...,
    SnsTopicArn: str = ...,
    SnsTopicStatus: str = ...,
    ParameterGroupName: str = ...,
    SnapshotWindow: str = ...,
    SnapshotRetentionLimit: int = ...,
    NodeType: str = ...,
    Engine: str = ...,
    EngineVersion: str = ...,
    ReplicaConfiguration: ReplicaConfigurationRequestTypeDef = ...,  # (1)
    ShardConfiguration: ShardConfigurationRequestTypeDef = ...,  # (2)
    ACLName: str = ...,
) -> UpdateClusterResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ReplicaConfigurationRequestTypeDef](./type_defs.md#replicaconfigurationrequesttypedef) 
2. See [:material-code-braces: ShardConfigurationRequestTypeDef](./type_defs.md#shardconfigurationrequesttypedef) 
3. See [:material-code-braces: UpdateClusterResponseTypeDef](./type_defs.md#updateclusterresponsetypedef) 


```python
# update_cluster method usage example with argument unpacking

kwargs: UpdateClusterRequestRequestTypeDef = {  # (1)
    "ClusterName": ...,
}

parent.update_cluster(**kwargs)
```

1. See [:material-code-braces: UpdateClusterRequestRequestTypeDef](./type_defs.md#updateclusterrequestrequesttypedef) 

### update\_multi\_region\_cluster

Updates the configuration of an existing multi-Region cluster.

Type annotations and code completion for `#!python session.client("memorydb").update_multi_region_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# update_multi_region_cluster method definition

await def update_multi_region_cluster(
    self,
    *,
    MultiRegionClusterName: str,
    NodeType: str = ...,
    Description: str = ...,
    EngineVersion: str = ...,
    ShardConfiguration: ShardConfigurationRequestTypeDef = ...,  # (1)
    MultiRegionParameterGroupName: str = ...,
    UpdateStrategy: UpdateStrategyType = ...,  # (2)
) -> UpdateMultiRegionClusterResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ShardConfigurationRequestTypeDef](./type_defs.md#shardconfigurationrequesttypedef) 
2. See [:material-code-brackets: UpdateStrategyType](./literals.md#updatestrategytype) 
3. See [:material-code-braces: UpdateMultiRegionClusterResponseTypeDef](./type_defs.md#updatemultiregionclusterresponsetypedef) 


```python
# update_multi_region_cluster method usage example with argument unpacking

kwargs: UpdateMultiRegionClusterRequestRequestTypeDef = {  # (1)
    "MultiRegionClusterName": ...,
}

parent.update_multi_region_cluster(**kwargs)
```

1. See [:material-code-braces: UpdateMultiRegionClusterRequestRequestTypeDef](./type_defs.md#updatemultiregionclusterrequestrequesttypedef) 

### update\_parameter\_group

Updates the parameters of a parameter group.

Type annotations and code completion for `#!python session.client("memorydb").update_parameter_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# update_parameter_group method definition

await def update_parameter_group(
    self,
    *,
    ParameterGroupName: str,
    ParameterNameValues: Sequence[ParameterNameValueTypeDef],  # (1)
) -> UpdateParameterGroupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ParameterNameValueTypeDef](./type_defs.md#parameternamevaluetypedef) 
2. See [:material-code-braces: UpdateParameterGroupResponseTypeDef](./type_defs.md#updateparametergroupresponsetypedef) 


```python
# update_parameter_group method usage example with argument unpacking

kwargs: UpdateParameterGroupRequestRequestTypeDef = {  # (1)
    "ParameterGroupName": ...,
    "ParameterNameValues": ...,
}

parent.update_parameter_group(**kwargs)
```

1. See [:material-code-braces: UpdateParameterGroupRequestRequestTypeDef](./type_defs.md#updateparametergrouprequestrequesttypedef) 

### update\_subnet\_group

Updates a subnet group.

Type annotations and code completion for `#!python session.client("memorydb").update_subnet_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# update_subnet_group method definition

await def update_subnet_group(
    self,
    *,
    SubnetGroupName: str,
    Description: str = ...,
    SubnetIds: Sequence[str] = ...,
) -> UpdateSubnetGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateSubnetGroupResponseTypeDef](./type_defs.md#updatesubnetgroupresponsetypedef) 


```python
# update_subnet_group method usage example with argument unpacking

kwargs: UpdateSubnetGroupRequestRequestTypeDef = {  # (1)
    "SubnetGroupName": ...,
}

parent.update_subnet_group(**kwargs)
```

1. See [:material-code-braces: UpdateSubnetGroupRequestRequestTypeDef](./type_defs.md#updatesubnetgrouprequestrequesttypedef) 

### update\_user

Changes user password(s) and/or access string.

Type annotations and code completion for `#!python session.client("memorydb").update_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# update_user method definition

await def update_user(
    self,
    *,
    UserName: str,
    AuthenticationMode: AuthenticationModeTypeDef = ...,  # (1)
    AccessString: str = ...,
) -> UpdateUserResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AuthenticationModeTypeDef](./type_defs.md#authenticationmodetypedef) 
2. See [:material-code-braces: UpdateUserResponseTypeDef](./type_defs.md#updateuserresponsetypedef) 


```python
# update_user method usage example with argument unpacking

kwargs: UpdateUserRequestRequestTypeDef = {  # (1)
    "UserName": ...,
}

parent.update_user(**kwargs)
```

1. See [:material-code-braces: UpdateUserRequestRequestTypeDef](./type_defs.md#updateuserrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("memorydb").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("memorydb").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client)

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

Type annotations and code completion for `#!python session.client("memorydb").get_paginator` method with overloads.

- `client.get_paginator("describe_acls")` -> [DescribeACLsPaginator](./paginators.md#describeaclspaginator)
- `client.get_paginator("describe_clusters")` -> [DescribeClustersPaginator](./paginators.md#describeclusterspaginator)
- `client.get_paginator("describe_engine_versions")` -> [DescribeEngineVersionsPaginator](./paginators.md#describeengineversionspaginator)
- `client.get_paginator("describe_events")` -> [DescribeEventsPaginator](./paginators.md#describeeventspaginator)
- `client.get_paginator("describe_multi_region_clusters")` -> [DescribeMultiRegionClustersPaginator](./paginators.md#describemultiregionclusterspaginator)
- `client.get_paginator("describe_parameter_groups")` -> [DescribeParameterGroupsPaginator](./paginators.md#describeparametergroupspaginator)
- `client.get_paginator("describe_parameters")` -> [DescribeParametersPaginator](./paginators.md#describeparameterspaginator)
- `client.get_paginator("describe_reserved_nodes_offerings")` -> [DescribeReservedNodesOfferingsPaginator](./paginators.md#describereservednodesofferingspaginator)
- `client.get_paginator("describe_reserved_nodes")` -> [DescribeReservedNodesPaginator](./paginators.md#describereservednodespaginator)
- `client.get_paginator("describe_service_updates")` -> [DescribeServiceUpdatesPaginator](./paginators.md#describeserviceupdatespaginator)
- `client.get_paginator("describe_snapshots")` -> [DescribeSnapshotsPaginator](./paginators.md#describesnapshotspaginator)
- `client.get_paginator("describe_subnet_groups")` -> [DescribeSubnetGroupsPaginator](./paginators.md#describesubnetgroupspaginator)
- `client.get_paginator("describe_users")` -> [DescribeUsersPaginator](./paginators.md#describeuserspaginator)


