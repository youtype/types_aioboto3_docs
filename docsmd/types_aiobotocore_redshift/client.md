# RedshiftClient

> [Index](../README.md) > [Redshift](./README.md) > RedshiftClient

!!! note ""

    Auto-generated documentation for [Redshift](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#redshift)
    type annotations stubs module [types-aiobotocore-redshift](https://pypi.org/project/types-aiobotocore-redshift/).

## RedshiftClient

Type annotations and code completion for `#!python session.client("redshift")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# RedshiftClient usage example

from aioboto3.session import Session
from types_aiobotocore_redshift.client import RedshiftClient

session = Session()
async with session.client("redshift") as client:
    client: RedshiftClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("redshift").exceptions` structure.

```python
# RedshiftClient.exceptions usage example

async with session.client("redshift") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessToClusterDeniedFault,
        client.exceptions.AccessToSnapshotDeniedFault,
        client.exceptions.AuthenticationProfileAlreadyExistsFault,
        client.exceptions.AuthenticationProfileNotFoundFault,
        client.exceptions.AuthenticationProfileQuotaExceededFault,
        client.exceptions.AuthorizationAlreadyExistsFault,
        client.exceptions.AuthorizationNotFoundFault,
        client.exceptions.AuthorizationQuotaExceededFault,
        client.exceptions.BatchDeleteRequestSizeExceededFault,
        client.exceptions.BatchModifyClusterSnapshotsLimitExceededFault,
        client.exceptions.BucketNotFoundFault,
        client.exceptions.ClientError,
        client.exceptions.ClusterAlreadyExistsFault,
        client.exceptions.ClusterNotFoundFault,
        client.exceptions.ClusterOnLatestRevisionFault,
        client.exceptions.ClusterParameterGroupAlreadyExistsFault,
        client.exceptions.ClusterParameterGroupNotFoundFault,
        client.exceptions.ClusterParameterGroupQuotaExceededFault,
        client.exceptions.ClusterQuotaExceededFault,
        client.exceptions.ClusterSecurityGroupAlreadyExistsFault,
        client.exceptions.ClusterSecurityGroupNotFoundFault,
        client.exceptions.ClusterSecurityGroupQuotaExceededFault,
        client.exceptions.ClusterSnapshotAlreadyExistsFault,
        client.exceptions.ClusterSnapshotNotFoundFault,
        client.exceptions.ClusterSnapshotQuotaExceededFault,
        client.exceptions.ClusterSubnetGroupAlreadyExistsFault,
        client.exceptions.ClusterSubnetGroupNotFoundFault,
        client.exceptions.ClusterSubnetGroupQuotaExceededFault,
        client.exceptions.ClusterSubnetQuotaExceededFault,
        client.exceptions.ConflictPolicyUpdateFault,
        client.exceptions.CopyToRegionDisabledFault,
        client.exceptions.CustomCnameAssociationFault,
        client.exceptions.CustomDomainAssociationNotFoundFault,
        client.exceptions.DependentServiceAccessDeniedFault,
        client.exceptions.DependentServiceRequestThrottlingFault,
        client.exceptions.DependentServiceUnavailableFault,
        client.exceptions.EndpointAlreadyExistsFault,
        client.exceptions.EndpointAuthorizationAlreadyExistsFault,
        client.exceptions.EndpointAuthorizationNotFoundFault,
        client.exceptions.EndpointAuthorizationsPerClusterLimitExceededFault,
        client.exceptions.EndpointNotFoundFault,
        client.exceptions.EndpointsPerAuthorizationLimitExceededFault,
        client.exceptions.EndpointsPerClusterLimitExceededFault,
        client.exceptions.EventSubscriptionQuotaExceededFault,
        client.exceptions.HsmClientCertificateAlreadyExistsFault,
        client.exceptions.HsmClientCertificateNotFoundFault,
        client.exceptions.HsmClientCertificateQuotaExceededFault,
        client.exceptions.HsmConfigurationAlreadyExistsFault,
        client.exceptions.HsmConfigurationNotFoundFault,
        client.exceptions.HsmConfigurationQuotaExceededFault,
        client.exceptions.InProgressTableRestoreQuotaExceededFault,
        client.exceptions.IncompatibleOrderableOptions,
        client.exceptions.InsufficientClusterCapacityFault,
        client.exceptions.InsufficientS3BucketPolicyFault,
        client.exceptions.IntegrationAlreadyExistsFault,
        client.exceptions.IntegrationConflictOperationFault,
        client.exceptions.IntegrationConflictStateFault,
        client.exceptions.IntegrationNotFoundFault,
        client.exceptions.IntegrationQuotaExceededFault,
        client.exceptions.IntegrationSourceNotFoundFault,
        client.exceptions.IntegrationTargetNotFoundFault,
        client.exceptions.InvalidAuthenticationProfileRequestFault,
        client.exceptions.InvalidAuthorizationStateFault,
        client.exceptions.InvalidClusterParameterGroupStateFault,
        client.exceptions.InvalidClusterSecurityGroupStateFault,
        client.exceptions.InvalidClusterSnapshotScheduleStateFault,
        client.exceptions.InvalidClusterSnapshotStateFault,
        client.exceptions.InvalidClusterStateFault,
        client.exceptions.InvalidClusterSubnetGroupStateFault,
        client.exceptions.InvalidClusterSubnetStateFault,
        client.exceptions.InvalidClusterTrackFault,
        client.exceptions.InvalidDataShareFault,
        client.exceptions.InvalidElasticIpFault,
        client.exceptions.InvalidEndpointStateFault,
        client.exceptions.InvalidHsmClientCertificateStateFault,
        client.exceptions.InvalidHsmConfigurationStateFault,
        client.exceptions.InvalidNamespaceFault,
        client.exceptions.InvalidPolicyFault,
        client.exceptions.InvalidReservedNodeStateFault,
        client.exceptions.InvalidRestoreFault,
        client.exceptions.InvalidRetentionPeriodFault,
        client.exceptions.InvalidS3BucketNameFault,
        client.exceptions.InvalidS3KeyPrefixFault,
        client.exceptions.InvalidScheduleFault,
        client.exceptions.InvalidScheduledActionFault,
        client.exceptions.InvalidSnapshotCopyGrantStateFault,
        client.exceptions.InvalidSubnet,
        client.exceptions.InvalidSubscriptionStateFault,
        client.exceptions.InvalidTableRestoreArgumentFault,
        client.exceptions.InvalidTagFault,
        client.exceptions.InvalidUsageLimitFault,
        client.exceptions.InvalidVPCNetworkStateFault,
        client.exceptions.Ipv6CidrBlockNotFoundFault,
        client.exceptions.LimitExceededFault,
        client.exceptions.NumberOfNodesPerClusterLimitExceededFault,
        client.exceptions.NumberOfNodesQuotaExceededFault,
        client.exceptions.PartnerNotFoundFault,
        client.exceptions.RedshiftIdcApplicationAlreadyExistsFault,
        client.exceptions.RedshiftIdcApplicationNotExistsFault,
        client.exceptions.RedshiftIdcApplicationQuotaExceededFault,
        client.exceptions.ReservedNodeAlreadyExistsFault,
        client.exceptions.ReservedNodeAlreadyMigratedFault,
        client.exceptions.ReservedNodeExchangeNotFoundFault,
        client.exceptions.ReservedNodeNotFoundFault,
        client.exceptions.ReservedNodeOfferingNotFoundFault,
        client.exceptions.ReservedNodeQuotaExceededFault,
        client.exceptions.ResizeNotFoundFault,
        client.exceptions.ResourceNotFoundFault,
        client.exceptions.SNSInvalidTopicFault,
        client.exceptions.SNSNoAuthorizationFault,
        client.exceptions.SNSTopicArnNotFoundFault,
        client.exceptions.ScheduleDefinitionTypeUnsupportedFault,
        client.exceptions.ScheduledActionAlreadyExistsFault,
        client.exceptions.ScheduledActionNotFoundFault,
        client.exceptions.ScheduledActionQuotaExceededFault,
        client.exceptions.ScheduledActionTypeUnsupportedFault,
        client.exceptions.SnapshotCopyAlreadyDisabledFault,
        client.exceptions.SnapshotCopyAlreadyEnabledFault,
        client.exceptions.SnapshotCopyDisabledFault,
        client.exceptions.SnapshotCopyGrantAlreadyExistsFault,
        client.exceptions.SnapshotCopyGrantNotFoundFault,
        client.exceptions.SnapshotCopyGrantQuotaExceededFault,
        client.exceptions.SnapshotScheduleAlreadyExistsFault,
        client.exceptions.SnapshotScheduleNotFoundFault,
        client.exceptions.SnapshotScheduleQuotaExceededFault,
        client.exceptions.SnapshotScheduleUpdateInProgressFault,
        client.exceptions.SourceNotFoundFault,
        client.exceptions.SubnetAlreadyInUse,
        client.exceptions.SubscriptionAlreadyExistFault,
        client.exceptions.SubscriptionCategoryNotFoundFault,
        client.exceptions.SubscriptionEventIdNotFoundFault,
        client.exceptions.SubscriptionNotFoundFault,
        client.exceptions.SubscriptionSeverityNotFoundFault,
        client.exceptions.TableLimitExceededFault,
        client.exceptions.TableRestoreNotFoundFault,
        client.exceptions.TagLimitExceededFault,
        client.exceptions.UnauthorizedOperation,
        client.exceptions.UnauthorizedPartnerIntegrationFault,
        client.exceptions.UnknownSnapshotCopyRegionFault,
        client.exceptions.UnsupportedOperationFault,
        client.exceptions.UnsupportedOptionFault,
        client.exceptions.UsageLimitAlreadyExistsFault,
        client.exceptions.UsageLimitNotFoundFault,
    ) as e:
        print(e)
```

```python
# RedshiftClient.exceptions type checking example

from types_aiobotocore_redshift.client import Exceptions

def handle_error(exc: Exceptions.AccessToClusterDeniedFault) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("redshift").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("redshift").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

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


### accept\_reserved\_node\_exchange

Exchanges a DC1 Reserved Node for a DC2 Reserved Node with no changes to the
configuration (term, payment type, or number of nodes) and no additional costs.

Type annotations and code completion for `#!python session.client("redshift").accept_reserved_node_exchange` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# accept_reserved_node_exchange method definition

await def accept_reserved_node_exchange(
    self,
    *,
    ReservedNodeId: str,
    TargetReservedNodeOfferingId: str,
) -> AcceptReservedNodeExchangeOutputMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AcceptReservedNodeExchangeOutputMessageTypeDef](./type_defs.md#acceptreservednodeexchangeoutputmessagetypedef) 


```python
# accept_reserved_node_exchange method usage example with argument unpacking

kwargs: AcceptReservedNodeExchangeInputMessageRequestTypeDef = {  # (1)
    "ReservedNodeId": ...,
    "TargetReservedNodeOfferingId": ...,
}

parent.accept_reserved_node_exchange(**kwargs)
```

1. See [:material-code-braces: AcceptReservedNodeExchangeInputMessageRequestTypeDef](./type_defs.md#acceptreservednodeexchangeinputmessagerequesttypedef) 

### add\_partner

Adds a partner integration to a cluster.

Type annotations and code completion for `#!python session.client("redshift").add_partner` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# add_partner method definition

await def add_partner(
    self,
    *,
    AccountId: str,
    ClusterIdentifier: str,
    DatabaseName: str,
    PartnerName: str,
) -> PartnerIntegrationOutputMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PartnerIntegrationOutputMessageTypeDef](./type_defs.md#partnerintegrationoutputmessagetypedef) 


```python
# add_partner method usage example with argument unpacking

kwargs: PartnerIntegrationInputMessageRequestTypeDef = {  # (1)
    "AccountId": ...,
    "ClusterIdentifier": ...,
    "DatabaseName": ...,
    "PartnerName": ...,
}

parent.add_partner(**kwargs)
```

1. See [:material-code-braces: PartnerIntegrationInputMessageRequestTypeDef](./type_defs.md#partnerintegrationinputmessagerequesttypedef) 

### associate\_data\_share\_consumer

From a datashare consumer account, associates a datashare with the account
(AssociateEntireAccount) or the specified namespace (ConsumerArn).

Type annotations and code completion for `#!python session.client("redshift").associate_data_share_consumer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# associate_data_share_consumer method definition

await def associate_data_share_consumer(
    self,
    *,
    DataShareArn: str,
    AssociateEntireAccount: bool = ...,
    ConsumerArn: str = ...,
    ConsumerRegion: str = ...,
    AllowWrites: bool = ...,
) -> DataShareResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DataShareResponseTypeDef](./type_defs.md#datashareresponsetypedef) 


```python
# associate_data_share_consumer method usage example with argument unpacking

kwargs: AssociateDataShareConsumerMessageRequestTypeDef = {  # (1)
    "DataShareArn": ...,
}

parent.associate_data_share_consumer(**kwargs)
```

1. See [:material-code-braces: AssociateDataShareConsumerMessageRequestTypeDef](./type_defs.md#associatedatashareconsumermessagerequesttypedef) 

### authorize\_cluster\_security\_group\_ingress

Adds an inbound (ingress) rule to an Amazon Redshift security group.

Type annotations and code completion for `#!python session.client("redshift").authorize_cluster_security_group_ingress` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# authorize_cluster_security_group_ingress method definition

await def authorize_cluster_security_group_ingress(
    self,
    *,
    ClusterSecurityGroupName: str,
    CIDRIP: str = ...,
    EC2SecurityGroupName: str = ...,
    EC2SecurityGroupOwnerId: str = ...,
) -> AuthorizeClusterSecurityGroupIngressResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AuthorizeClusterSecurityGroupIngressResultTypeDef](./type_defs.md#authorizeclustersecuritygroupingressresulttypedef) 


```python
# authorize_cluster_security_group_ingress method usage example with argument unpacking

kwargs: AuthorizeClusterSecurityGroupIngressMessageRequestTypeDef = {  # (1)
    "ClusterSecurityGroupName": ...,
}

parent.authorize_cluster_security_group_ingress(**kwargs)
```

1. See [:material-code-braces: AuthorizeClusterSecurityGroupIngressMessageRequestTypeDef](./type_defs.md#authorizeclustersecuritygroupingressmessagerequesttypedef) 

### authorize\_data\_share

From a data producer account, authorizes the sharing of a datashare with one or
more consumer accounts or managing entities.

Type annotations and code completion for `#!python session.client("redshift").authorize_data_share` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# authorize_data_share method definition

await def authorize_data_share(
    self,
    *,
    DataShareArn: str,
    ConsumerIdentifier: str,
    AllowWrites: bool = ...,
) -> DataShareResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DataShareResponseTypeDef](./type_defs.md#datashareresponsetypedef) 


```python
# authorize_data_share method usage example with argument unpacking

kwargs: AuthorizeDataShareMessageRequestTypeDef = {  # (1)
    "DataShareArn": ...,
    "ConsumerIdentifier": ...,
}

parent.authorize_data_share(**kwargs)
```

1. See [:material-code-braces: AuthorizeDataShareMessageRequestTypeDef](./type_defs.md#authorizedatasharemessagerequesttypedef) 

### authorize\_endpoint\_access

Grants access to a cluster.

Type annotations and code completion for `#!python session.client("redshift").authorize_endpoint_access` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# authorize_endpoint_access method definition

await def authorize_endpoint_access(
    self,
    *,
    Account: str,
    ClusterIdentifier: str = ...,
    VpcIds: Sequence[str] = ...,
) -> EndpointAuthorizationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EndpointAuthorizationResponseTypeDef](./type_defs.md#endpointauthorizationresponsetypedef) 


```python
# authorize_endpoint_access method usage example with argument unpacking

kwargs: AuthorizeEndpointAccessMessageRequestTypeDef = {  # (1)
    "Account": ...,
}

parent.authorize_endpoint_access(**kwargs)
```

1. See [:material-code-braces: AuthorizeEndpointAccessMessageRequestTypeDef](./type_defs.md#authorizeendpointaccessmessagerequesttypedef) 

### authorize\_snapshot\_access

Authorizes the specified Amazon Web Services account to restore the specified
snapshot.

Type annotations and code completion for `#!python session.client("redshift").authorize_snapshot_access` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# authorize_snapshot_access method definition

await def authorize_snapshot_access(
    self,
    *,
    AccountWithRestoreAccess: str,
    SnapshotIdentifier: str = ...,
    SnapshotArn: str = ...,
    SnapshotClusterIdentifier: str = ...,
) -> AuthorizeSnapshotAccessResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AuthorizeSnapshotAccessResultTypeDef](./type_defs.md#authorizesnapshotaccessresulttypedef) 


```python
# authorize_snapshot_access method usage example with argument unpacking

kwargs: AuthorizeSnapshotAccessMessageRequestTypeDef = {  # (1)
    "AccountWithRestoreAccess": ...,
}

parent.authorize_snapshot_access(**kwargs)
```

1. See [:material-code-braces: AuthorizeSnapshotAccessMessageRequestTypeDef](./type_defs.md#authorizesnapshotaccessmessagerequesttypedef) 

### batch\_delete\_cluster\_snapshots

Deletes a set of cluster snapshots.

Type annotations and code completion for `#!python session.client("redshift").batch_delete_cluster_snapshots` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# batch_delete_cluster_snapshots method definition

await def batch_delete_cluster_snapshots(
    self,
    *,
    Identifiers: Sequence[DeleteClusterSnapshotMessageTypeDef],  # (1)
) -> BatchDeleteClusterSnapshotsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DeleteClusterSnapshotMessageTypeDef](./type_defs.md#deleteclustersnapshotmessagetypedef) 
2. See [:material-code-braces: BatchDeleteClusterSnapshotsResultTypeDef](./type_defs.md#batchdeleteclustersnapshotsresulttypedef) 


```python
# batch_delete_cluster_snapshots method usage example with argument unpacking

kwargs: BatchDeleteClusterSnapshotsRequestRequestTypeDef = {  # (1)
    "Identifiers": ...,
}

parent.batch_delete_cluster_snapshots(**kwargs)
```

1. See [:material-code-braces: BatchDeleteClusterSnapshotsRequestRequestTypeDef](./type_defs.md#batchdeleteclustersnapshotsrequestrequesttypedef) 

### batch\_modify\_cluster\_snapshots

Modifies the settings for a set of cluster snapshots.

Type annotations and code completion for `#!python session.client("redshift").batch_modify_cluster_snapshots` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# batch_modify_cluster_snapshots method definition

await def batch_modify_cluster_snapshots(
    self,
    *,
    SnapshotIdentifierList: Sequence[str],
    ManualSnapshotRetentionPeriod: int = ...,
    Force: bool = ...,
) -> BatchModifyClusterSnapshotsOutputMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchModifyClusterSnapshotsOutputMessageTypeDef](./type_defs.md#batchmodifyclustersnapshotsoutputmessagetypedef) 


```python
# batch_modify_cluster_snapshots method usage example with argument unpacking

kwargs: BatchModifyClusterSnapshotsMessageRequestTypeDef = {  # (1)
    "SnapshotIdentifierList": ...,
}

parent.batch_modify_cluster_snapshots(**kwargs)
```

1. See [:material-code-braces: BatchModifyClusterSnapshotsMessageRequestTypeDef](./type_defs.md#batchmodifyclustersnapshotsmessagerequesttypedef) 

### cancel\_resize

Cancels a resize operation for a cluster.

Type annotations and code completion for `#!python session.client("redshift").cancel_resize` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# cancel_resize method definition

await def cancel_resize(
    self,
    *,
    ClusterIdentifier: str,
) -> ResizeProgressMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ResizeProgressMessageTypeDef](./type_defs.md#resizeprogressmessagetypedef) 


```python
# cancel_resize method usage example with argument unpacking

kwargs: CancelResizeMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.cancel_resize(**kwargs)
```

1. See [:material-code-braces: CancelResizeMessageRequestTypeDef](./type_defs.md#cancelresizemessagerequesttypedef) 

### copy\_cluster\_snapshot

Copies the specified automated cluster snapshot to a new manual cluster
snapshot.

Type annotations and code completion for `#!python session.client("redshift").copy_cluster_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# copy_cluster_snapshot method definition

await def copy_cluster_snapshot(
    self,
    *,
    SourceSnapshotIdentifier: str,
    TargetSnapshotIdentifier: str,
    SourceSnapshotClusterIdentifier: str = ...,
    ManualSnapshotRetentionPeriod: int = ...,
) -> CopyClusterSnapshotResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CopyClusterSnapshotResultTypeDef](./type_defs.md#copyclustersnapshotresulttypedef) 


```python
# copy_cluster_snapshot method usage example with argument unpacking

kwargs: CopyClusterSnapshotMessageRequestTypeDef = {  # (1)
    "SourceSnapshotIdentifier": ...,
    "TargetSnapshotIdentifier": ...,
}

parent.copy_cluster_snapshot(**kwargs)
```

1. See [:material-code-braces: CopyClusterSnapshotMessageRequestTypeDef](./type_defs.md#copyclustersnapshotmessagerequesttypedef) 

### create\_authentication\_profile

Creates an authentication profile with the specified parameters.

Type annotations and code completion for `#!python session.client("redshift").create_authentication_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# create_authentication_profile method definition

await def create_authentication_profile(
    self,
    *,
    AuthenticationProfileName: str,
    AuthenticationProfileContent: str,
) -> CreateAuthenticationProfileResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateAuthenticationProfileResultTypeDef](./type_defs.md#createauthenticationprofileresulttypedef) 


```python
# create_authentication_profile method usage example with argument unpacking

kwargs: CreateAuthenticationProfileMessageRequestTypeDef = {  # (1)
    "AuthenticationProfileName": ...,
    "AuthenticationProfileContent": ...,
}

parent.create_authentication_profile(**kwargs)
```

1. See [:material-code-braces: CreateAuthenticationProfileMessageRequestTypeDef](./type_defs.md#createauthenticationprofilemessagerequesttypedef) 

### create\_cluster

Creates a new cluster with the specified parameters.

Type annotations and code completion for `#!python session.client("redshift").create_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# create_cluster method definition

await def create_cluster(
    self,
    *,
    ClusterIdentifier: str,
    NodeType: str,
    MasterUsername: str,
    DBName: str = ...,
    ClusterType: str = ...,
    MasterUserPassword: str = ...,
    ClusterSecurityGroups: Sequence[str] = ...,
    VpcSecurityGroupIds: Sequence[str] = ...,
    ClusterSubnetGroupName: str = ...,
    AvailabilityZone: str = ...,
    PreferredMaintenanceWindow: str = ...,
    ClusterParameterGroupName: str = ...,
    AutomatedSnapshotRetentionPeriod: int = ...,
    ManualSnapshotRetentionPeriod: int = ...,
    Port: int = ...,
    ClusterVersion: str = ...,
    AllowVersionUpgrade: bool = ...,
    NumberOfNodes: int = ...,
    PubliclyAccessible: bool = ...,
    Encrypted: bool = ...,
    HsmClientCertificateIdentifier: str = ...,
    HsmConfigurationIdentifier: str = ...,
    ElasticIp: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
    KmsKeyId: str = ...,
    EnhancedVpcRouting: bool = ...,
    AdditionalInfo: str = ...,
    IamRoles: Sequence[str] = ...,
    MaintenanceTrackName: str = ...,
    SnapshotScheduleIdentifier: str = ...,
    AvailabilityZoneRelocation: bool = ...,
    AquaConfigurationStatus: AquaConfigurationStatusType = ...,  # (2)
    DefaultIamRoleArn: str = ...,
    LoadSampleData: str = ...,
    ManageMasterPassword: bool = ...,
    MasterPasswordSecretKmsKeyId: str = ...,
    IpAddressType: str = ...,
    MultiAZ: bool = ...,
    RedshiftIdcApplicationArn: str = ...,
) -> CreateClusterResultTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-brackets: AquaConfigurationStatusType](./literals.md#aquaconfigurationstatustype) 
3. See [:material-code-braces: CreateClusterResultTypeDef](./type_defs.md#createclusterresulttypedef) 


```python
# create_cluster method usage example with argument unpacking

kwargs: CreateClusterMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
    "NodeType": ...,
    "MasterUsername": ...,
}

parent.create_cluster(**kwargs)
```

1. See [:material-code-braces: CreateClusterMessageRequestTypeDef](./type_defs.md#createclustermessagerequesttypedef) 

### create\_cluster\_parameter\_group

Creates an Amazon Redshift parameter group.

Type annotations and code completion for `#!python session.client("redshift").create_cluster_parameter_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# create_cluster_parameter_group method definition

await def create_cluster_parameter_group(
    self,
    *,
    ParameterGroupName: str,
    ParameterGroupFamily: str,
    Description: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateClusterParameterGroupResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateClusterParameterGroupResultTypeDef](./type_defs.md#createclusterparametergroupresulttypedef) 


```python
# create_cluster_parameter_group method usage example with argument unpacking

kwargs: CreateClusterParameterGroupMessageRequestTypeDef = {  # (1)
    "ParameterGroupName": ...,
    "ParameterGroupFamily": ...,
    "Description": ...,
}

parent.create_cluster_parameter_group(**kwargs)
```

1. See [:material-code-braces: CreateClusterParameterGroupMessageRequestTypeDef](./type_defs.md#createclusterparametergroupmessagerequesttypedef) 

### create\_cluster\_security\_group

Creates a new Amazon Redshift security group.

Type annotations and code completion for `#!python session.client("redshift").create_cluster_security_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# create_cluster_security_group method definition

await def create_cluster_security_group(
    self,
    *,
    ClusterSecurityGroupName: str,
    Description: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateClusterSecurityGroupResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateClusterSecurityGroupResultTypeDef](./type_defs.md#createclustersecuritygroupresulttypedef) 


```python
# create_cluster_security_group method usage example with argument unpacking

kwargs: CreateClusterSecurityGroupMessageRequestTypeDef = {  # (1)
    "ClusterSecurityGroupName": ...,
    "Description": ...,
}

parent.create_cluster_security_group(**kwargs)
```

1. See [:material-code-braces: CreateClusterSecurityGroupMessageRequestTypeDef](./type_defs.md#createclustersecuritygroupmessagerequesttypedef) 

### create\_cluster\_snapshot

Creates a manual snapshot of the specified cluster.

Type annotations and code completion for `#!python session.client("redshift").create_cluster_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# create_cluster_snapshot method definition

await def create_cluster_snapshot(
    self,
    *,
    SnapshotIdentifier: str,
    ClusterIdentifier: str,
    ManualSnapshotRetentionPeriod: int = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateClusterSnapshotResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateClusterSnapshotResultTypeDef](./type_defs.md#createclustersnapshotresulttypedef) 


```python
# create_cluster_snapshot method usage example with argument unpacking

kwargs: CreateClusterSnapshotMessageRequestTypeDef = {  # (1)
    "SnapshotIdentifier": ...,
    "ClusterIdentifier": ...,
}

parent.create_cluster_snapshot(**kwargs)
```

1. See [:material-code-braces: CreateClusterSnapshotMessageRequestTypeDef](./type_defs.md#createclustersnapshotmessagerequesttypedef) 

### create\_cluster\_subnet\_group

Creates a new Amazon Redshift subnet group.

Type annotations and code completion for `#!python session.client("redshift").create_cluster_subnet_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# create_cluster_subnet_group method definition

await def create_cluster_subnet_group(
    self,
    *,
    ClusterSubnetGroupName: str,
    Description: str,
    SubnetIds: Sequence[str],
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateClusterSubnetGroupResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateClusterSubnetGroupResultTypeDef](./type_defs.md#createclustersubnetgroupresulttypedef) 


```python
# create_cluster_subnet_group method usage example with argument unpacking

kwargs: CreateClusterSubnetGroupMessageRequestTypeDef = {  # (1)
    "ClusterSubnetGroupName": ...,
    "Description": ...,
    "SubnetIds": ...,
}

parent.create_cluster_subnet_group(**kwargs)
```

1. See [:material-code-braces: CreateClusterSubnetGroupMessageRequestTypeDef](./type_defs.md#createclustersubnetgroupmessagerequesttypedef) 

### create\_custom\_domain\_association

Used to create a custom domain name for a cluster.

Type annotations and code completion for `#!python session.client("redshift").create_custom_domain_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# create_custom_domain_association method definition

await def create_custom_domain_association(
    self,
    *,
    CustomDomainName: str,
    CustomDomainCertificateArn: str,
    ClusterIdentifier: str,
) -> CreateCustomDomainAssociationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateCustomDomainAssociationResultTypeDef](./type_defs.md#createcustomdomainassociationresulttypedef) 


```python
# create_custom_domain_association method usage example with argument unpacking

kwargs: CreateCustomDomainAssociationMessageRequestTypeDef = {  # (1)
    "CustomDomainName": ...,
    "CustomDomainCertificateArn": ...,
    "ClusterIdentifier": ...,
}

parent.create_custom_domain_association(**kwargs)
```

1. See [:material-code-braces: CreateCustomDomainAssociationMessageRequestTypeDef](./type_defs.md#createcustomdomainassociationmessagerequesttypedef) 

### create\_endpoint\_access

Creates a Redshift-managed VPC endpoint.

Type annotations and code completion for `#!python session.client("redshift").create_endpoint_access` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# create_endpoint_access method definition

await def create_endpoint_access(
    self,
    *,
    EndpointName: str,
    SubnetGroupName: str,
    ClusterIdentifier: str = ...,
    ResourceOwner: str = ...,
    VpcSecurityGroupIds: Sequence[str] = ...,
) -> EndpointAccessResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EndpointAccessResponseTypeDef](./type_defs.md#endpointaccessresponsetypedef) 


```python
# create_endpoint_access method usage example with argument unpacking

kwargs: CreateEndpointAccessMessageRequestTypeDef = {  # (1)
    "EndpointName": ...,
    "SubnetGroupName": ...,
}

parent.create_endpoint_access(**kwargs)
```

1. See [:material-code-braces: CreateEndpointAccessMessageRequestTypeDef](./type_defs.md#createendpointaccessmessagerequesttypedef) 

### create\_event\_subscription

Creates an Amazon Redshift event notification subscription.

Type annotations and code completion for `#!python session.client("redshift").create_event_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# create_event_subscription method definition

await def create_event_subscription(
    self,
    *,
    SubscriptionName: str,
    SnsTopicArn: str,
    SourceType: str = ...,
    SourceIds: Sequence[str] = ...,
    EventCategories: Sequence[str] = ...,
    Severity: str = ...,
    Enabled: bool = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateEventSubscriptionResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateEventSubscriptionResultTypeDef](./type_defs.md#createeventsubscriptionresulttypedef) 


```python
# create_event_subscription method usage example with argument unpacking

kwargs: CreateEventSubscriptionMessageRequestTypeDef = {  # (1)
    "SubscriptionName": ...,
    "SnsTopicArn": ...,
}

parent.create_event_subscription(**kwargs)
```

1. See [:material-code-braces: CreateEventSubscriptionMessageRequestTypeDef](./type_defs.md#createeventsubscriptionmessagerequesttypedef) 

### create\_hsm\_client\_certificate

Creates an HSM client certificate that an Amazon Redshift cluster will use to
connect to the client's HSM in order to store and retrieve the keys used to
encrypt the cluster databases.

Type annotations and code completion for `#!python session.client("redshift").create_hsm_client_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# create_hsm_client_certificate method definition

await def create_hsm_client_certificate(
    self,
    *,
    HsmClientCertificateIdentifier: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateHsmClientCertificateResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateHsmClientCertificateResultTypeDef](./type_defs.md#createhsmclientcertificateresulttypedef) 


```python
# create_hsm_client_certificate method usage example with argument unpacking

kwargs: CreateHsmClientCertificateMessageRequestTypeDef = {  # (1)
    "HsmClientCertificateIdentifier": ...,
}

parent.create_hsm_client_certificate(**kwargs)
```

1. See [:material-code-braces: CreateHsmClientCertificateMessageRequestTypeDef](./type_defs.md#createhsmclientcertificatemessagerequesttypedef) 

### create\_hsm\_configuration

Creates an HSM configuration that contains the information required by an
Amazon Redshift cluster to store and use database encryption keys in a Hardware
Security Module (HSM).

Type annotations and code completion for `#!python session.client("redshift").create_hsm_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# create_hsm_configuration method definition

await def create_hsm_configuration(
    self,
    *,
    HsmConfigurationIdentifier: str,
    Description: str,
    HsmIpAddress: str,
    HsmPartitionName: str,
    HsmPartitionPassword: str,
    HsmServerPublicCertificate: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateHsmConfigurationResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateHsmConfigurationResultTypeDef](./type_defs.md#createhsmconfigurationresulttypedef) 


```python
# create_hsm_configuration method usage example with argument unpacking

kwargs: CreateHsmConfigurationMessageRequestTypeDef = {  # (1)
    "HsmConfigurationIdentifier": ...,
    "Description": ...,
    "HsmIpAddress": ...,
    "HsmPartitionName": ...,
    "HsmPartitionPassword": ...,
    "HsmServerPublicCertificate": ...,
}

parent.create_hsm_configuration(**kwargs)
```

1. See [:material-code-braces: CreateHsmConfigurationMessageRequestTypeDef](./type_defs.md#createhsmconfigurationmessagerequesttypedef) 

### create\_integration

Creates a zero-ETL integration or S3 event integration with Amazon Redshift.

Type annotations and code completion for `#!python session.client("redshift").create_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# create_integration method definition

await def create_integration(
    self,
    *,
    SourceArn: str,
    TargetArn: str,
    IntegrationName: str,
    KMSKeyId: str = ...,
    TagList: Sequence[TagTypeDef] = ...,  # (1)
    AdditionalEncryptionContext: Mapping[str, str] = ...,
    Description: str = ...,
) -> IntegrationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: IntegrationResponseTypeDef](./type_defs.md#integrationresponsetypedef) 


```python
# create_integration method usage example with argument unpacking

kwargs: CreateIntegrationMessageRequestTypeDef = {  # (1)
    "SourceArn": ...,
    "TargetArn": ...,
    "IntegrationName": ...,
}

parent.create_integration(**kwargs)
```

1. See [:material-code-braces: CreateIntegrationMessageRequestTypeDef](./type_defs.md#createintegrationmessagerequesttypedef) 

### create\_redshift\_idc\_application

Creates an Amazon Redshift application for use with IAM Identity Center.

Type annotations and code completion for `#!python session.client("redshift").create_redshift_idc_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# create_redshift_idc_application method definition

await def create_redshift_idc_application(
    self,
    *,
    IdcInstanceArn: str,
    RedshiftIdcApplicationName: str,
    IdcDisplayName: str,
    IamRoleArn: str,
    IdentityNamespace: str = ...,
    AuthorizedTokenIssuerList: Sequence[AuthorizedTokenIssuerUnionTypeDef] = ...,  # (1)
    ServiceIntegrations: Sequence[ServiceIntegrationsUnionUnionTypeDef] = ...,  # (2)
) -> CreateRedshiftIdcApplicationResultTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AuthorizedTokenIssuerTypeDef](./type_defs.md#authorizedtokenissuertypedef) [:material-code-braces: AuthorizedTokenIssuerOutputTypeDef](./type_defs.md#authorizedtokenissueroutputtypedef) 
2. See [:material-code-braces: ServiceIntegrationsUnionTypeDef](./type_defs.md#serviceintegrationsuniontypedef) [:material-code-braces: ServiceIntegrationsUnionOutputTypeDef](./type_defs.md#serviceintegrationsunionoutputtypedef) 
3. See [:material-code-braces: CreateRedshiftIdcApplicationResultTypeDef](./type_defs.md#createredshiftidcapplicationresulttypedef) 


```python
# create_redshift_idc_application method usage example with argument unpacking

kwargs: CreateRedshiftIdcApplicationMessageRequestTypeDef = {  # (1)
    "IdcInstanceArn": ...,
    "RedshiftIdcApplicationName": ...,
    "IdcDisplayName": ...,
    "IamRoleArn": ...,
}

parent.create_redshift_idc_application(**kwargs)
```

1. See [:material-code-braces: CreateRedshiftIdcApplicationMessageRequestTypeDef](./type_defs.md#createredshiftidcapplicationmessagerequesttypedef) 

### create\_scheduled\_action

Creates a scheduled action.

Type annotations and code completion for `#!python session.client("redshift").create_scheduled_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# create_scheduled_action method definition

await def create_scheduled_action(
    self,
    *,
    ScheduledActionName: str,
    TargetAction: ScheduledActionTypeTypeDef,  # (1)
    Schedule: str,
    IamRole: str,
    ScheduledActionDescription: str = ...,
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    Enable: bool = ...,
) -> ScheduledActionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ScheduledActionTypeTypeDef](./type_defs.md#scheduledactiontypetypedef) 
2. See [:material-code-braces: ScheduledActionResponseTypeDef](./type_defs.md#scheduledactionresponsetypedef) 


```python
# create_scheduled_action method usage example with argument unpacking

kwargs: CreateScheduledActionMessageRequestTypeDef = {  # (1)
    "ScheduledActionName": ...,
    "TargetAction": ...,
    "Schedule": ...,
    "IamRole": ...,
}

parent.create_scheduled_action(**kwargs)
```

1. See [:material-code-braces: CreateScheduledActionMessageRequestTypeDef](./type_defs.md#createscheduledactionmessagerequesttypedef) 

### create\_snapshot\_copy\_grant

Creates a snapshot copy grant that permits Amazon Redshift to use an encrypted
symmetric key from Key Management Service (KMS) to encrypt copied snapshots in
a destination region.

Type annotations and code completion for `#!python session.client("redshift").create_snapshot_copy_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# create_snapshot_copy_grant method definition

await def create_snapshot_copy_grant(
    self,
    *,
    SnapshotCopyGrantName: str,
    KmsKeyId: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateSnapshotCopyGrantResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateSnapshotCopyGrantResultTypeDef](./type_defs.md#createsnapshotcopygrantresulttypedef) 


```python
# create_snapshot_copy_grant method usage example with argument unpacking

kwargs: CreateSnapshotCopyGrantMessageRequestTypeDef = {  # (1)
    "SnapshotCopyGrantName": ...,
}

parent.create_snapshot_copy_grant(**kwargs)
```

1. See [:material-code-braces: CreateSnapshotCopyGrantMessageRequestTypeDef](./type_defs.md#createsnapshotcopygrantmessagerequesttypedef) 

### create\_snapshot\_schedule

Create a snapshot schedule that can be associated to a cluster and which
overrides the default system backup schedule.

Type annotations and code completion for `#!python session.client("redshift").create_snapshot_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# create_snapshot_schedule method definition

await def create_snapshot_schedule(
    self,
    *,
    ScheduleDefinitions: Sequence[str] = ...,
    ScheduleIdentifier: str = ...,
    ScheduleDescription: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    NextInvocations: int = ...,
) -> SnapshotScheduleResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: SnapshotScheduleResponseTypeDef](./type_defs.md#snapshotscheduleresponsetypedef) 


```python
# create_snapshot_schedule method usage example with argument unpacking

kwargs: CreateSnapshotScheduleMessageRequestTypeDef = {  # (1)
    "ScheduleDefinitions": ...,
}

parent.create_snapshot_schedule(**kwargs)
```

1. See [:material-code-braces: CreateSnapshotScheduleMessageRequestTypeDef](./type_defs.md#createsnapshotschedulemessagerequesttypedef) 

### create\_tags

Adds tags to a cluster.

Type annotations and code completion for `#!python session.client("redshift").create_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# create_tags method definition

await def create_tags(
    self,
    *,
    ResourceName: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# create_tags method usage example with argument unpacking

kwargs: CreateTagsMessageRequestTypeDef = {  # (1)
    "ResourceName": ...,
    "Tags": ...,
}

parent.create_tags(**kwargs)
```

1. See [:material-code-braces: CreateTagsMessageRequestTypeDef](./type_defs.md#createtagsmessagerequesttypedef) 

### create\_usage\_limit

Creates a usage limit for a specified Amazon Redshift feature on a cluster.

Type annotations and code completion for `#!python session.client("redshift").create_usage_limit` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# create_usage_limit method definition

await def create_usage_limit(
    self,
    *,
    ClusterIdentifier: str,
    FeatureType: UsageLimitFeatureTypeType,  # (1)
    LimitType: UsageLimitLimitTypeType,  # (2)
    Amount: int,
    Period: UsageLimitPeriodType = ...,  # (3)
    BreachAction: UsageLimitBreachActionType = ...,  # (4)
    Tags: Sequence[TagTypeDef] = ...,  # (5)
) -> UsageLimitResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: UsageLimitFeatureTypeType](./literals.md#usagelimitfeaturetypetype) 
2. See [:material-code-brackets: UsageLimitLimitTypeType](./literals.md#usagelimitlimittypetype) 
3. See [:material-code-brackets: UsageLimitPeriodType](./literals.md#usagelimitperiodtype) 
4. See [:material-code-brackets: UsageLimitBreachActionType](./literals.md#usagelimitbreachactiontype) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: UsageLimitResponseTypeDef](./type_defs.md#usagelimitresponsetypedef) 


```python
# create_usage_limit method usage example with argument unpacking

kwargs: CreateUsageLimitMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
    "FeatureType": ...,
    "LimitType": ...,
    "Amount": ...,
}

parent.create_usage_limit(**kwargs)
```

1. See [:material-code-braces: CreateUsageLimitMessageRequestTypeDef](./type_defs.md#createusagelimitmessagerequesttypedef) 

### deauthorize\_data\_share

From a datashare producer account, removes authorization from the specified
datashare.

Type annotations and code completion for `#!python session.client("redshift").deauthorize_data_share` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# deauthorize_data_share method definition

await def deauthorize_data_share(
    self,
    *,
    DataShareArn: str,
    ConsumerIdentifier: str,
) -> DataShareResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DataShareResponseTypeDef](./type_defs.md#datashareresponsetypedef) 


```python
# deauthorize_data_share method usage example with argument unpacking

kwargs: DeauthorizeDataShareMessageRequestTypeDef = {  # (1)
    "DataShareArn": ...,
    "ConsumerIdentifier": ...,
}

parent.deauthorize_data_share(**kwargs)
```

1. See [:material-code-braces: DeauthorizeDataShareMessageRequestTypeDef](./type_defs.md#deauthorizedatasharemessagerequesttypedef) 

### delete\_authentication\_profile

Deletes an authentication profile.

Type annotations and code completion for `#!python session.client("redshift").delete_authentication_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# delete_authentication_profile method definition

await def delete_authentication_profile(
    self,
    *,
    AuthenticationProfileName: str,
) -> DeleteAuthenticationProfileResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteAuthenticationProfileResultTypeDef](./type_defs.md#deleteauthenticationprofileresulttypedef) 


```python
# delete_authentication_profile method usage example with argument unpacking

kwargs: DeleteAuthenticationProfileMessageRequestTypeDef = {  # (1)
    "AuthenticationProfileName": ...,
}

parent.delete_authentication_profile(**kwargs)
```

1. See [:material-code-braces: DeleteAuthenticationProfileMessageRequestTypeDef](./type_defs.md#deleteauthenticationprofilemessagerequesttypedef) 

### delete\_cluster

Deletes a previously provisioned cluster without its final snapshot being
created.

Type annotations and code completion for `#!python session.client("redshift").delete_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# delete_cluster method definition

await def delete_cluster(
    self,
    *,
    ClusterIdentifier: str,
    SkipFinalClusterSnapshot: bool = ...,
    FinalClusterSnapshotIdentifier: str = ...,
    FinalClusterSnapshotRetentionPeriod: int = ...,
) -> DeleteClusterResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteClusterResultTypeDef](./type_defs.md#deleteclusterresulttypedef) 


```python
# delete_cluster method usage example with argument unpacking

kwargs: DeleteClusterMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.delete_cluster(**kwargs)
```

1. See [:material-code-braces: DeleteClusterMessageRequestTypeDef](./type_defs.md#deleteclustermessagerequesttypedef) 

### delete\_cluster\_parameter\_group

Deletes a specified Amazon Redshift parameter group.

Type annotations and code completion for `#!python session.client("redshift").delete_cluster_parameter_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# delete_cluster_parameter_group method definition

await def delete_cluster_parameter_group(
    self,
    *,
    ParameterGroupName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_cluster_parameter_group method usage example with argument unpacking

kwargs: DeleteClusterParameterGroupMessageRequestTypeDef = {  # (1)
    "ParameterGroupName": ...,
}

parent.delete_cluster_parameter_group(**kwargs)
```

1. See [:material-code-braces: DeleteClusterParameterGroupMessageRequestTypeDef](./type_defs.md#deleteclusterparametergroupmessagerequesttypedef) 

### delete\_cluster\_security\_group

Deletes an Amazon Redshift security group.

Type annotations and code completion for `#!python session.client("redshift").delete_cluster_security_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# delete_cluster_security_group method definition

await def delete_cluster_security_group(
    self,
    *,
    ClusterSecurityGroupName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_cluster_security_group method usage example with argument unpacking

kwargs: DeleteClusterSecurityGroupMessageRequestTypeDef = {  # (1)
    "ClusterSecurityGroupName": ...,
}

parent.delete_cluster_security_group(**kwargs)
```

1. See [:material-code-braces: DeleteClusterSecurityGroupMessageRequestTypeDef](./type_defs.md#deleteclustersecuritygroupmessagerequesttypedef) 

### delete\_cluster\_snapshot

Deletes the specified manual snapshot.

Type annotations and code completion for `#!python session.client("redshift").delete_cluster_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# delete_cluster_snapshot method definition

await def delete_cluster_snapshot(
    self,
    *,
    SnapshotIdentifier: str,
    SnapshotClusterIdentifier: str = ...,
) -> DeleteClusterSnapshotResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteClusterSnapshotResultTypeDef](./type_defs.md#deleteclustersnapshotresulttypedef) 


```python
# delete_cluster_snapshot method usage example with argument unpacking

kwargs: DeleteClusterSnapshotMessageRequestTypeDef = {  # (1)
    "SnapshotIdentifier": ...,
}

parent.delete_cluster_snapshot(**kwargs)
```

1. See [:material-code-braces: DeleteClusterSnapshotMessageRequestTypeDef](./type_defs.md#deleteclustersnapshotmessagerequesttypedef) 

### delete\_cluster\_subnet\_group

Deletes the specified cluster subnet group.

Type annotations and code completion for `#!python session.client("redshift").delete_cluster_subnet_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# delete_cluster_subnet_group method definition

await def delete_cluster_subnet_group(
    self,
    *,
    ClusterSubnetGroupName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_cluster_subnet_group method usage example with argument unpacking

kwargs: DeleteClusterSubnetGroupMessageRequestTypeDef = {  # (1)
    "ClusterSubnetGroupName": ...,
}

parent.delete_cluster_subnet_group(**kwargs)
```

1. See [:material-code-braces: DeleteClusterSubnetGroupMessageRequestTypeDef](./type_defs.md#deleteclustersubnetgroupmessagerequesttypedef) 

### delete\_custom\_domain\_association

Contains information about deleting a custom domain association for a cluster.

Type annotations and code completion for `#!python session.client("redshift").delete_custom_domain_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# delete_custom_domain_association method definition

await def delete_custom_domain_association(
    self,
    *,
    ClusterIdentifier: str,
    CustomDomainName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_custom_domain_association method usage example with argument unpacking

kwargs: DeleteCustomDomainAssociationMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
    "CustomDomainName": ...,
}

parent.delete_custom_domain_association(**kwargs)
```

1. See [:material-code-braces: DeleteCustomDomainAssociationMessageRequestTypeDef](./type_defs.md#deletecustomdomainassociationmessagerequesttypedef) 

### delete\_endpoint\_access

Deletes a Redshift-managed VPC endpoint.

Type annotations and code completion for `#!python session.client("redshift").delete_endpoint_access` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# delete_endpoint_access method definition

await def delete_endpoint_access(
    self,
    *,
    EndpointName: str,
) -> EndpointAccessResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EndpointAccessResponseTypeDef](./type_defs.md#endpointaccessresponsetypedef) 


```python
# delete_endpoint_access method usage example with argument unpacking

kwargs: DeleteEndpointAccessMessageRequestTypeDef = {  # (1)
    "EndpointName": ...,
}

parent.delete_endpoint_access(**kwargs)
```

1. See [:material-code-braces: DeleteEndpointAccessMessageRequestTypeDef](./type_defs.md#deleteendpointaccessmessagerequesttypedef) 

### delete\_event\_subscription

Deletes an Amazon Redshift event notification subscription.

Type annotations and code completion for `#!python session.client("redshift").delete_event_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# delete_event_subscription method definition

await def delete_event_subscription(
    self,
    *,
    SubscriptionName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_event_subscription method usage example with argument unpacking

kwargs: DeleteEventSubscriptionMessageRequestTypeDef = {  # (1)
    "SubscriptionName": ...,
}

parent.delete_event_subscription(**kwargs)
```

1. See [:material-code-braces: DeleteEventSubscriptionMessageRequestTypeDef](./type_defs.md#deleteeventsubscriptionmessagerequesttypedef) 

### delete\_hsm\_client\_certificate

Deletes the specified HSM client certificate.

Type annotations and code completion for `#!python session.client("redshift").delete_hsm_client_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# delete_hsm_client_certificate method definition

await def delete_hsm_client_certificate(
    self,
    *,
    HsmClientCertificateIdentifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_hsm_client_certificate method usage example with argument unpacking

kwargs: DeleteHsmClientCertificateMessageRequestTypeDef = {  # (1)
    "HsmClientCertificateIdentifier": ...,
}

parent.delete_hsm_client_certificate(**kwargs)
```

1. See [:material-code-braces: DeleteHsmClientCertificateMessageRequestTypeDef](./type_defs.md#deletehsmclientcertificatemessagerequesttypedef) 

### delete\_hsm\_configuration

Deletes the specified Amazon Redshift HSM configuration.

Type annotations and code completion for `#!python session.client("redshift").delete_hsm_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# delete_hsm_configuration method definition

await def delete_hsm_configuration(
    self,
    *,
    HsmConfigurationIdentifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_hsm_configuration method usage example with argument unpacking

kwargs: DeleteHsmConfigurationMessageRequestTypeDef = {  # (1)
    "HsmConfigurationIdentifier": ...,
}

parent.delete_hsm_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteHsmConfigurationMessageRequestTypeDef](./type_defs.md#deletehsmconfigurationmessagerequesttypedef) 

### delete\_integration

Deletes a zero-ETL integration or S3 event integration with Amazon Redshift.

Type annotations and code completion for `#!python session.client("redshift").delete_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# delete_integration method definition

await def delete_integration(
    self,
    *,
    IntegrationArn: str,
) -> IntegrationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: IntegrationResponseTypeDef](./type_defs.md#integrationresponsetypedef) 


```python
# delete_integration method usage example with argument unpacking

kwargs: DeleteIntegrationMessageRequestTypeDef = {  # (1)
    "IntegrationArn": ...,
}

parent.delete_integration(**kwargs)
```

1. See [:material-code-braces: DeleteIntegrationMessageRequestTypeDef](./type_defs.md#deleteintegrationmessagerequesttypedef) 

### delete\_partner

Deletes a partner integration from a cluster.

Type annotations and code completion for `#!python session.client("redshift").delete_partner` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# delete_partner method definition

await def delete_partner(
    self,
    *,
    AccountId: str,
    ClusterIdentifier: str,
    DatabaseName: str,
    PartnerName: str,
) -> PartnerIntegrationOutputMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PartnerIntegrationOutputMessageTypeDef](./type_defs.md#partnerintegrationoutputmessagetypedef) 


```python
# delete_partner method usage example with argument unpacking

kwargs: PartnerIntegrationInputMessageRequestTypeDef = {  # (1)
    "AccountId": ...,
    "ClusterIdentifier": ...,
    "DatabaseName": ...,
    "PartnerName": ...,
}

parent.delete_partner(**kwargs)
```

1. See [:material-code-braces: PartnerIntegrationInputMessageRequestTypeDef](./type_defs.md#partnerintegrationinputmessagerequesttypedef) 

### delete\_redshift\_idc\_application

Deletes an Amazon Redshift IAM Identity Center application.

Type annotations and code completion for `#!python session.client("redshift").delete_redshift_idc_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# delete_redshift_idc_application method definition

await def delete_redshift_idc_application(
    self,
    *,
    RedshiftIdcApplicationArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_redshift_idc_application method usage example with argument unpacking

kwargs: DeleteRedshiftIdcApplicationMessageRequestTypeDef = {  # (1)
    "RedshiftIdcApplicationArn": ...,
}

parent.delete_redshift_idc_application(**kwargs)
```

1. See [:material-code-braces: DeleteRedshiftIdcApplicationMessageRequestTypeDef](./type_defs.md#deleteredshiftidcapplicationmessagerequesttypedef) 

### delete\_resource\_policy

Deletes the resource policy for a specified resource.

Type annotations and code completion for `#!python session.client("redshift").delete_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# delete_resource_policy method definition

await def delete_resource_policy(
    self,
    *,
    ResourceArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_resource_policy method usage example with argument unpacking

kwargs: DeleteResourcePolicyMessageRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.delete_resource_policy(**kwargs)
```

1. See [:material-code-braces: DeleteResourcePolicyMessageRequestTypeDef](./type_defs.md#deleteresourcepolicymessagerequesttypedef) 

### delete\_scheduled\_action

Deletes a scheduled action.

Type annotations and code completion for `#!python session.client("redshift").delete_scheduled_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# delete_scheduled_action method definition

await def delete_scheduled_action(
    self,
    *,
    ScheduledActionName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_scheduled_action method usage example with argument unpacking

kwargs: DeleteScheduledActionMessageRequestTypeDef = {  # (1)
    "ScheduledActionName": ...,
}

parent.delete_scheduled_action(**kwargs)
```

1. See [:material-code-braces: DeleteScheduledActionMessageRequestTypeDef](./type_defs.md#deletescheduledactionmessagerequesttypedef) 

### delete\_snapshot\_copy\_grant

Deletes the specified snapshot copy grant.

Type annotations and code completion for `#!python session.client("redshift").delete_snapshot_copy_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# delete_snapshot_copy_grant method definition

await def delete_snapshot_copy_grant(
    self,
    *,
    SnapshotCopyGrantName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_snapshot_copy_grant method usage example with argument unpacking

kwargs: DeleteSnapshotCopyGrantMessageRequestTypeDef = {  # (1)
    "SnapshotCopyGrantName": ...,
}

parent.delete_snapshot_copy_grant(**kwargs)
```

1. See [:material-code-braces: DeleteSnapshotCopyGrantMessageRequestTypeDef](./type_defs.md#deletesnapshotcopygrantmessagerequesttypedef) 

### delete\_snapshot\_schedule

Deletes a snapshot schedule.

Type annotations and code completion for `#!python session.client("redshift").delete_snapshot_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# delete_snapshot_schedule method definition

await def delete_snapshot_schedule(
    self,
    *,
    ScheduleIdentifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_snapshot_schedule method usage example with argument unpacking

kwargs: DeleteSnapshotScheduleMessageRequestTypeDef = {  # (1)
    "ScheduleIdentifier": ...,
}

parent.delete_snapshot_schedule(**kwargs)
```

1. See [:material-code-braces: DeleteSnapshotScheduleMessageRequestTypeDef](./type_defs.md#deletesnapshotschedulemessagerequesttypedef) 

### delete\_tags

Deletes tags from a resource.

Type annotations and code completion for `#!python session.client("redshift").delete_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# delete_tags method definition

await def delete_tags(
    self,
    *,
    ResourceName: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_tags method usage example with argument unpacking

kwargs: DeleteTagsMessageRequestTypeDef = {  # (1)
    "ResourceName": ...,
    "TagKeys": ...,
}

parent.delete_tags(**kwargs)
```

1. See [:material-code-braces: DeleteTagsMessageRequestTypeDef](./type_defs.md#deletetagsmessagerequesttypedef) 

### delete\_usage\_limit

Deletes a usage limit from a cluster.

Type annotations and code completion for `#!python session.client("redshift").delete_usage_limit` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# delete_usage_limit method definition

await def delete_usage_limit(
    self,
    *,
    UsageLimitId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_usage_limit method usage example with argument unpacking

kwargs: DeleteUsageLimitMessageRequestTypeDef = {  # (1)
    "UsageLimitId": ...,
}

parent.delete_usage_limit(**kwargs)
```

1. See [:material-code-braces: DeleteUsageLimitMessageRequestTypeDef](./type_defs.md#deleteusagelimitmessagerequesttypedef) 

### deregister\_namespace

Deregisters a cluster or serverless namespace from the Amazon Web Services Glue
Data Catalog.

Type annotations and code completion for `#!python session.client("redshift").deregister_namespace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# deregister_namespace method definition

await def deregister_namespace(
    self,
    *,
    NamespaceIdentifier: NamespaceIdentifierUnionTypeDef,  # (1)
    ConsumerIdentifiers: Sequence[str],
) -> DeregisterNamespaceOutputMessageTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: NamespaceIdentifierUnionTypeDef](./type_defs.md#namespaceidentifieruniontypedef) 
2. See [:material-code-braces: DeregisterNamespaceOutputMessageTypeDef](./type_defs.md#deregisternamespaceoutputmessagetypedef) 


```python
# deregister_namespace method usage example with argument unpacking

kwargs: DeregisterNamespaceInputMessageRequestTypeDef = {  # (1)
    "NamespaceIdentifier": ...,
    "ConsumerIdentifiers": ...,
}

parent.deregister_namespace(**kwargs)
```

1. See [:material-code-braces: DeregisterNamespaceInputMessageRequestTypeDef](./type_defs.md#deregisternamespaceinputmessagerequesttypedef) 

### describe\_account\_attributes

Returns a list of attributes attached to an account.

Type annotations and code completion for `#!python session.client("redshift").describe_account_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_account_attributes method definition

await def describe_account_attributes(
    self,
    *,
    AttributeNames: Sequence[str] = ...,
) -> AccountAttributeListTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AccountAttributeListTypeDef](./type_defs.md#accountattributelisttypedef) 


```python
# describe_account_attributes method usage example with argument unpacking

kwargs: DescribeAccountAttributesMessageRequestTypeDef = {  # (1)
    "AttributeNames": ...,
}

parent.describe_account_attributes(**kwargs)
```

1. See [:material-code-braces: DescribeAccountAttributesMessageRequestTypeDef](./type_defs.md#describeaccountattributesmessagerequesttypedef) 

### describe\_authentication\_profiles

Describes an authentication profile.

Type annotations and code completion for `#!python session.client("redshift").describe_authentication_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_authentication_profiles method definition

await def describe_authentication_profiles(
    self,
    *,
    AuthenticationProfileName: str = ...,
) -> DescribeAuthenticationProfilesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAuthenticationProfilesResultTypeDef](./type_defs.md#describeauthenticationprofilesresulttypedef) 


```python
# describe_authentication_profiles method usage example with argument unpacking

kwargs: DescribeAuthenticationProfilesMessageRequestTypeDef = {  # (1)
    "AuthenticationProfileName": ...,
}

parent.describe_authentication_profiles(**kwargs)
```

1. See [:material-code-braces: DescribeAuthenticationProfilesMessageRequestTypeDef](./type_defs.md#describeauthenticationprofilesmessagerequesttypedef) 

### describe\_cluster\_db\_revisions

Returns an array of <code>ClusterDbRevision</code> objects.

Type annotations and code completion for `#!python session.client("redshift").describe_cluster_db_revisions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_cluster_db_revisions method definition

await def describe_cluster_db_revisions(
    self,
    *,
    ClusterIdentifier: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> ClusterDbRevisionsMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ClusterDbRevisionsMessageTypeDef](./type_defs.md#clusterdbrevisionsmessagetypedef) 


```python
# describe_cluster_db_revisions method usage example with argument unpacking

kwargs: DescribeClusterDbRevisionsMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.describe_cluster_db_revisions(**kwargs)
```

1. See [:material-code-braces: DescribeClusterDbRevisionsMessageRequestTypeDef](./type_defs.md#describeclusterdbrevisionsmessagerequesttypedef) 

### describe\_cluster\_parameter\_groups

Returns a list of Amazon Redshift parameter groups, including parameter groups
you created and the default parameter group.

Type annotations and code completion for `#!python session.client("redshift").describe_cluster_parameter_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_cluster_parameter_groups method definition

await def describe_cluster_parameter_groups(
    self,
    *,
    ParameterGroupName: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
) -> ClusterParameterGroupsMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ClusterParameterGroupsMessageTypeDef](./type_defs.md#clusterparametergroupsmessagetypedef) 


```python
# describe_cluster_parameter_groups method usage example with argument unpacking

kwargs: DescribeClusterParameterGroupsMessageRequestTypeDef = {  # (1)
    "ParameterGroupName": ...,
}

parent.describe_cluster_parameter_groups(**kwargs)
```

1. See [:material-code-braces: DescribeClusterParameterGroupsMessageRequestTypeDef](./type_defs.md#describeclusterparametergroupsmessagerequesttypedef) 

### describe\_cluster\_parameters

Returns a detailed list of parameters contained within the specified Amazon
Redshift parameter group.

Type annotations and code completion for `#!python session.client("redshift").describe_cluster_parameters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_cluster_parameters method definition

await def describe_cluster_parameters(
    self,
    *,
    ParameterGroupName: str,
    Source: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> ClusterParameterGroupDetailsTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ClusterParameterGroupDetailsTypeDef](./type_defs.md#clusterparametergroupdetailstypedef) 


```python
# describe_cluster_parameters method usage example with argument unpacking

kwargs: DescribeClusterParametersMessageRequestTypeDef = {  # (1)
    "ParameterGroupName": ...,
}

parent.describe_cluster_parameters(**kwargs)
```

1. See [:material-code-braces: DescribeClusterParametersMessageRequestTypeDef](./type_defs.md#describeclusterparametersmessagerequesttypedef) 

### describe\_cluster\_security\_groups

Returns information about Amazon Redshift security groups.

Type annotations and code completion for `#!python session.client("redshift").describe_cluster_security_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_cluster_security_groups method definition

await def describe_cluster_security_groups(
    self,
    *,
    ClusterSecurityGroupName: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
) -> ClusterSecurityGroupMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ClusterSecurityGroupMessageTypeDef](./type_defs.md#clustersecuritygroupmessagetypedef) 


```python
# describe_cluster_security_groups method usage example with argument unpacking

kwargs: DescribeClusterSecurityGroupsMessageRequestTypeDef = {  # (1)
    "ClusterSecurityGroupName": ...,
}

parent.describe_cluster_security_groups(**kwargs)
```

1. See [:material-code-braces: DescribeClusterSecurityGroupsMessageRequestTypeDef](./type_defs.md#describeclustersecuritygroupsmessagerequesttypedef) 

### describe\_cluster\_snapshots

Returns one or more snapshot objects, which contain metadata about your cluster
snapshots.

Type annotations and code completion for `#!python session.client("redshift").describe_cluster_snapshots` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_cluster_snapshots method definition

await def describe_cluster_snapshots(
    self,
    *,
    ClusterIdentifier: str = ...,
    SnapshotIdentifier: str = ...,
    SnapshotArn: str = ...,
    SnapshotType: str = ...,
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
    OwnerAccount: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    ClusterExists: bool = ...,
    SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...,  # (1)
) -> SnapshotMessageTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SnapshotSortingEntityTypeDef](./type_defs.md#snapshotsortingentitytypedef) 
2. See [:material-code-braces: SnapshotMessageTypeDef](./type_defs.md#snapshotmessagetypedef) 


```python
# describe_cluster_snapshots method usage example with argument unpacking

kwargs: DescribeClusterSnapshotsMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.describe_cluster_snapshots(**kwargs)
```

1. See [:material-code-braces: DescribeClusterSnapshotsMessageRequestTypeDef](./type_defs.md#describeclustersnapshotsmessagerequesttypedef) 

### describe\_cluster\_subnet\_groups

Returns one or more cluster subnet group objects, which contain metadata about
your cluster subnet groups.

Type annotations and code completion for `#!python session.client("redshift").describe_cluster_subnet_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_cluster_subnet_groups method definition

await def describe_cluster_subnet_groups(
    self,
    *,
    ClusterSubnetGroupName: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
) -> ClusterSubnetGroupMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ClusterSubnetGroupMessageTypeDef](./type_defs.md#clustersubnetgroupmessagetypedef) 


```python
# describe_cluster_subnet_groups method usage example with argument unpacking

kwargs: DescribeClusterSubnetGroupsMessageRequestTypeDef = {  # (1)
    "ClusterSubnetGroupName": ...,
}

parent.describe_cluster_subnet_groups(**kwargs)
```

1. See [:material-code-braces: DescribeClusterSubnetGroupsMessageRequestTypeDef](./type_defs.md#describeclustersubnetgroupsmessagerequesttypedef) 

### describe\_cluster\_tracks

Returns a list of all the available maintenance tracks.

Type annotations and code completion for `#!python session.client("redshift").describe_cluster_tracks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_cluster_tracks method definition

await def describe_cluster_tracks(
    self,
    *,
    MaintenanceTrackName: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> TrackListMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TrackListMessageTypeDef](./type_defs.md#tracklistmessagetypedef) 


```python
# describe_cluster_tracks method usage example with argument unpacking

kwargs: DescribeClusterTracksMessageRequestTypeDef = {  # (1)
    "MaintenanceTrackName": ...,
}

parent.describe_cluster_tracks(**kwargs)
```

1. See [:material-code-braces: DescribeClusterTracksMessageRequestTypeDef](./type_defs.md#describeclustertracksmessagerequesttypedef) 

### describe\_cluster\_versions

Returns descriptions of the available Amazon Redshift cluster versions.

Type annotations and code completion for `#!python session.client("redshift").describe_cluster_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_cluster_versions method definition

await def describe_cluster_versions(
    self,
    *,
    ClusterVersion: str = ...,
    ClusterParameterGroupFamily: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> ClusterVersionsMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ClusterVersionsMessageTypeDef](./type_defs.md#clusterversionsmessagetypedef) 


```python
# describe_cluster_versions method usage example with argument unpacking

kwargs: DescribeClusterVersionsMessageRequestTypeDef = {  # (1)
    "ClusterVersion": ...,
}

parent.describe_cluster_versions(**kwargs)
```

1. See [:material-code-braces: DescribeClusterVersionsMessageRequestTypeDef](./type_defs.md#describeclusterversionsmessagerequesttypedef) 

### describe\_clusters

Returns properties of provisioned clusters including general cluster
properties, cluster database properties, maintenance and backup properties, and
security and access properties.

Type annotations and code completion for `#!python session.client("redshift").describe_clusters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_clusters method definition

await def describe_clusters(
    self,
    *,
    ClusterIdentifier: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
) -> ClustersMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ClustersMessageTypeDef](./type_defs.md#clustersmessagetypedef) 


```python
# describe_clusters method usage example with argument unpacking

kwargs: DescribeClustersMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.describe_clusters(**kwargs)
```

1. See [:material-code-braces: DescribeClustersMessageRequestTypeDef](./type_defs.md#describeclustersmessagerequesttypedef) 

### describe\_custom\_domain\_associations

Contains information about custom domain associations for a cluster.

Type annotations and code completion for `#!python session.client("redshift").describe_custom_domain_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_custom_domain_associations method definition

await def describe_custom_domain_associations(
    self,
    *,
    CustomDomainName: str = ...,
    CustomDomainCertificateArn: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> CustomDomainAssociationsMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CustomDomainAssociationsMessageTypeDef](./type_defs.md#customdomainassociationsmessagetypedef) 


```python
# describe_custom_domain_associations method usage example with argument unpacking

kwargs: DescribeCustomDomainAssociationsMessageRequestTypeDef = {  # (1)
    "CustomDomainName": ...,
}

parent.describe_custom_domain_associations(**kwargs)
```

1. See [:material-code-braces: DescribeCustomDomainAssociationsMessageRequestTypeDef](./type_defs.md#describecustomdomainassociationsmessagerequesttypedef) 

### describe\_data\_shares

Shows the status of any inbound or outbound datashares available in the
specified account.

Type annotations and code completion for `#!python session.client("redshift").describe_data_shares` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_data_shares method definition

await def describe_data_shares(
    self,
    *,
    DataShareArn: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeDataSharesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDataSharesResultTypeDef](./type_defs.md#describedatasharesresulttypedef) 


```python
# describe_data_shares method usage example with argument unpacking

kwargs: DescribeDataSharesMessageRequestTypeDef = {  # (1)
    "DataShareArn": ...,
}

parent.describe_data_shares(**kwargs)
```

1. See [:material-code-braces: DescribeDataSharesMessageRequestTypeDef](./type_defs.md#describedatasharesmessagerequesttypedef) 

### describe\_data\_shares\_for\_consumer

Returns a list of datashares where the account identifier being called is a
consumer account identifier.

Type annotations and code completion for `#!python session.client("redshift").describe_data_shares_for_consumer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_data_shares_for_consumer method definition

await def describe_data_shares_for_consumer(
    self,
    *,
    ConsumerArn: str = ...,
    Status: DataShareStatusForConsumerType = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeDataSharesForConsumerResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DataShareStatusForConsumerType](./literals.md#datasharestatusforconsumertype) 
2. See [:material-code-braces: DescribeDataSharesForConsumerResultTypeDef](./type_defs.md#describedatasharesforconsumerresulttypedef) 


```python
# describe_data_shares_for_consumer method usage example with argument unpacking

kwargs: DescribeDataSharesForConsumerMessageRequestTypeDef = {  # (1)
    "ConsumerArn": ...,
}

parent.describe_data_shares_for_consumer(**kwargs)
```

1. See [:material-code-braces: DescribeDataSharesForConsumerMessageRequestTypeDef](./type_defs.md#describedatasharesforconsumermessagerequesttypedef) 

### describe\_data\_shares\_for\_producer

Returns a list of datashares when the account identifier being called is a
producer account identifier.

Type annotations and code completion for `#!python session.client("redshift").describe_data_shares_for_producer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_data_shares_for_producer method definition

await def describe_data_shares_for_producer(
    self,
    *,
    ProducerArn: str = ...,
    Status: DataShareStatusForProducerType = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeDataSharesForProducerResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DataShareStatusForProducerType](./literals.md#datasharestatusforproducertype) 
2. See [:material-code-braces: DescribeDataSharesForProducerResultTypeDef](./type_defs.md#describedatasharesforproducerresulttypedef) 


```python
# describe_data_shares_for_producer method usage example with argument unpacking

kwargs: DescribeDataSharesForProducerMessageRequestTypeDef = {  # (1)
    "ProducerArn": ...,
}

parent.describe_data_shares_for_producer(**kwargs)
```

1. See [:material-code-braces: DescribeDataSharesForProducerMessageRequestTypeDef](./type_defs.md#describedatasharesforproducermessagerequesttypedef) 

### describe\_default\_cluster\_parameters

Returns a list of parameter settings for the specified parameter group family.

Type annotations and code completion for `#!python session.client("redshift").describe_default_cluster_parameters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_default_cluster_parameters method definition

await def describe_default_cluster_parameters(
    self,
    *,
    ParameterGroupFamily: str,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeDefaultClusterParametersResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDefaultClusterParametersResultTypeDef](./type_defs.md#describedefaultclusterparametersresulttypedef) 


```python
# describe_default_cluster_parameters method usage example with argument unpacking

kwargs: DescribeDefaultClusterParametersMessageRequestTypeDef = {  # (1)
    "ParameterGroupFamily": ...,
}

parent.describe_default_cluster_parameters(**kwargs)
```

1. See [:material-code-braces: DescribeDefaultClusterParametersMessageRequestTypeDef](./type_defs.md#describedefaultclusterparametersmessagerequesttypedef) 

### describe\_endpoint\_access

Describes a Redshift-managed VPC endpoint.

Type annotations and code completion for `#!python session.client("redshift").describe_endpoint_access` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_endpoint_access method definition

await def describe_endpoint_access(
    self,
    *,
    ClusterIdentifier: str = ...,
    ResourceOwner: str = ...,
    EndpointName: str = ...,
    VpcId: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> EndpointAccessListTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EndpointAccessListTypeDef](./type_defs.md#endpointaccesslisttypedef) 


```python
# describe_endpoint_access method usage example with argument unpacking

kwargs: DescribeEndpointAccessMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.describe_endpoint_access(**kwargs)
```

1. See [:material-code-braces: DescribeEndpointAccessMessageRequestTypeDef](./type_defs.md#describeendpointaccessmessagerequesttypedef) 

### describe\_endpoint\_authorization

Describes an endpoint authorization.

Type annotations and code completion for `#!python session.client("redshift").describe_endpoint_authorization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_endpoint_authorization method definition

await def describe_endpoint_authorization(
    self,
    *,
    ClusterIdentifier: str = ...,
    Account: str = ...,
    Grantee: bool = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> EndpointAuthorizationListTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EndpointAuthorizationListTypeDef](./type_defs.md#endpointauthorizationlisttypedef) 


```python
# describe_endpoint_authorization method usage example with argument unpacking

kwargs: DescribeEndpointAuthorizationMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.describe_endpoint_authorization(**kwargs)
```

1. See [:material-code-braces: DescribeEndpointAuthorizationMessageRequestTypeDef](./type_defs.md#describeendpointauthorizationmessagerequesttypedef) 

### describe\_event\_categories

Displays a list of event categories for all event source types, or for a
specified source type.

Type annotations and code completion for `#!python session.client("redshift").describe_event_categories` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_event_categories method definition

await def describe_event_categories(
    self,
    *,
    SourceType: str = ...,
) -> EventCategoriesMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EventCategoriesMessageTypeDef](./type_defs.md#eventcategoriesmessagetypedef) 


```python
# describe_event_categories method usage example with argument unpacking

kwargs: DescribeEventCategoriesMessageRequestTypeDef = {  # (1)
    "SourceType": ...,
}

parent.describe_event_categories(**kwargs)
```

1. See [:material-code-braces: DescribeEventCategoriesMessageRequestTypeDef](./type_defs.md#describeeventcategoriesmessagerequesttypedef) 

### describe\_event\_subscriptions

Lists descriptions of all the Amazon Redshift event notification subscriptions
for a customer account.

Type annotations and code completion for `#!python session.client("redshift").describe_event_subscriptions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_event_subscriptions method definition

await def describe_event_subscriptions(
    self,
    *,
    SubscriptionName: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
) -> EventSubscriptionsMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EventSubscriptionsMessageTypeDef](./type_defs.md#eventsubscriptionsmessagetypedef) 


```python
# describe_event_subscriptions method usage example with argument unpacking

kwargs: DescribeEventSubscriptionsMessageRequestTypeDef = {  # (1)
    "SubscriptionName": ...,
}

parent.describe_event_subscriptions(**kwargs)
```

1. See [:material-code-braces: DescribeEventSubscriptionsMessageRequestTypeDef](./type_defs.md#describeeventsubscriptionsmessagerequesttypedef) 

### describe\_events

Returns events related to clusters, security groups, snapshots, and parameter
groups for the past 14 days.

Type annotations and code completion for `#!python session.client("redshift").describe_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_events method definition

await def describe_events(
    self,
    *,
    SourceIdentifier: str = ...,
    SourceType: SourceTypeType = ...,  # (1)
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    Duration: int = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> EventsMessageTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-braces: EventsMessageTypeDef](./type_defs.md#eventsmessagetypedef) 


```python
# describe_events method usage example with argument unpacking

kwargs: DescribeEventsMessageRequestTypeDef = {  # (1)
    "SourceIdentifier": ...,
}

parent.describe_events(**kwargs)
```

1. See [:material-code-braces: DescribeEventsMessageRequestTypeDef](./type_defs.md#describeeventsmessagerequesttypedef) 

### describe\_hsm\_client\_certificates

Returns information about the specified HSM client certificate.

Type annotations and code completion for `#!python session.client("redshift").describe_hsm_client_certificates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_hsm_client_certificates method definition

await def describe_hsm_client_certificates(
    self,
    *,
    HsmClientCertificateIdentifier: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
) -> HsmClientCertificateMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: HsmClientCertificateMessageTypeDef](./type_defs.md#hsmclientcertificatemessagetypedef) 


```python
# describe_hsm_client_certificates method usage example with argument unpacking

kwargs: DescribeHsmClientCertificatesMessageRequestTypeDef = {  # (1)
    "HsmClientCertificateIdentifier": ...,
}

parent.describe_hsm_client_certificates(**kwargs)
```

1. See [:material-code-braces: DescribeHsmClientCertificatesMessageRequestTypeDef](./type_defs.md#describehsmclientcertificatesmessagerequesttypedef) 

### describe\_hsm\_configurations

Returns information about the specified Amazon Redshift HSM configuration.

Type annotations and code completion for `#!python session.client("redshift").describe_hsm_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_hsm_configurations method definition

await def describe_hsm_configurations(
    self,
    *,
    HsmConfigurationIdentifier: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
) -> HsmConfigurationMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: HsmConfigurationMessageTypeDef](./type_defs.md#hsmconfigurationmessagetypedef) 


```python
# describe_hsm_configurations method usage example with argument unpacking

kwargs: DescribeHsmConfigurationsMessageRequestTypeDef = {  # (1)
    "HsmConfigurationIdentifier": ...,
}

parent.describe_hsm_configurations(**kwargs)
```

1. See [:material-code-braces: DescribeHsmConfigurationsMessageRequestTypeDef](./type_defs.md#describehsmconfigurationsmessagerequesttypedef) 

### describe\_inbound\_integrations

Returns a list of inbound integrations.

Type annotations and code completion for `#!python session.client("redshift").describe_inbound_integrations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_inbound_integrations method definition

await def describe_inbound_integrations(
    self,
    *,
    IntegrationArn: str = ...,
    TargetArn: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> InboundIntegrationsMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: InboundIntegrationsMessageTypeDef](./type_defs.md#inboundintegrationsmessagetypedef) 


```python
# describe_inbound_integrations method usage example with argument unpacking

kwargs: DescribeInboundIntegrationsMessageRequestTypeDef = {  # (1)
    "IntegrationArn": ...,
}

parent.describe_inbound_integrations(**kwargs)
```

1. See [:material-code-braces: DescribeInboundIntegrationsMessageRequestTypeDef](./type_defs.md#describeinboundintegrationsmessagerequesttypedef) 

### describe\_integrations

Describes one or more zero-ETL or S3 event integrations with Amazon Redshift.

Type annotations and code completion for `#!python session.client("redshift").describe_integrations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_integrations method definition

await def describe_integrations(
    self,
    *,
    IntegrationArn: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
    Filters: Sequence[DescribeIntegrationsFilterTypeDef] = ...,  # (1)
) -> IntegrationsMessageTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DescribeIntegrationsFilterTypeDef](./type_defs.md#describeintegrationsfiltertypedef) 
2. See [:material-code-braces: IntegrationsMessageTypeDef](./type_defs.md#integrationsmessagetypedef) 


```python
# describe_integrations method usage example with argument unpacking

kwargs: DescribeIntegrationsMessageRequestTypeDef = {  # (1)
    "IntegrationArn": ...,
}

parent.describe_integrations(**kwargs)
```

1. See [:material-code-braces: DescribeIntegrationsMessageRequestTypeDef](./type_defs.md#describeintegrationsmessagerequesttypedef) 

### describe\_logging\_status

Describes whether information, such as queries and connection attempts, is
being logged for the specified Amazon Redshift cluster.

Type annotations and code completion for `#!python session.client("redshift").describe_logging_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_logging_status method definition

await def describe_logging_status(
    self,
    *,
    ClusterIdentifier: str,
) -> LoggingStatusTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: LoggingStatusTypeDef](./type_defs.md#loggingstatustypedef) 


```python
# describe_logging_status method usage example with argument unpacking

kwargs: DescribeLoggingStatusMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.describe_logging_status(**kwargs)
```

1. See [:material-code-braces: DescribeLoggingStatusMessageRequestTypeDef](./type_defs.md#describeloggingstatusmessagerequesttypedef) 

### describe\_node\_configuration\_options

Returns properties of possible node configurations such as node type, number of
nodes, and disk usage for the specified action type.

Type annotations and code completion for `#!python session.client("redshift").describe_node_configuration_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_node_configuration_options method definition

await def describe_node_configuration_options(
    self,
    *,
    ActionType: ActionTypeType,  # (1)
    ClusterIdentifier: str = ...,
    SnapshotIdentifier: str = ...,
    SnapshotArn: str = ...,
    OwnerAccount: str = ...,
    Filters: Sequence[NodeConfigurationOptionsFilterTypeDef] = ...,  # (2)
    Marker: str = ...,
    MaxRecords: int = ...,
) -> NodeConfigurationOptionsMessageTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
2. See [:material-code-braces: NodeConfigurationOptionsFilterTypeDef](./type_defs.md#nodeconfigurationoptionsfiltertypedef) 
3. See [:material-code-braces: NodeConfigurationOptionsMessageTypeDef](./type_defs.md#nodeconfigurationoptionsmessagetypedef) 


```python
# describe_node_configuration_options method usage example with argument unpacking

kwargs: DescribeNodeConfigurationOptionsMessageRequestTypeDef = {  # (1)
    "ActionType": ...,
}

parent.describe_node_configuration_options(**kwargs)
```

1. See [:material-code-braces: DescribeNodeConfigurationOptionsMessageRequestTypeDef](./type_defs.md#describenodeconfigurationoptionsmessagerequesttypedef) 

### describe\_orderable\_cluster\_options

Returns a list of orderable cluster options.

Type annotations and code completion for `#!python session.client("redshift").describe_orderable_cluster_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_orderable_cluster_options method definition

await def describe_orderable_cluster_options(
    self,
    *,
    ClusterVersion: str = ...,
    NodeType: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> OrderableClusterOptionsMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: OrderableClusterOptionsMessageTypeDef](./type_defs.md#orderableclusteroptionsmessagetypedef) 


```python
# describe_orderable_cluster_options method usage example with argument unpacking

kwargs: DescribeOrderableClusterOptionsMessageRequestTypeDef = {  # (1)
    "ClusterVersion": ...,
}

parent.describe_orderable_cluster_options(**kwargs)
```

1. See [:material-code-braces: DescribeOrderableClusterOptionsMessageRequestTypeDef](./type_defs.md#describeorderableclusteroptionsmessagerequesttypedef) 

### describe\_partners

Returns information about the partner integrations defined for a cluster.

Type annotations and code completion for `#!python session.client("redshift").describe_partners` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_partners method definition

await def describe_partners(
    self,
    *,
    AccountId: str,
    ClusterIdentifier: str,
    DatabaseName: str = ...,
    PartnerName: str = ...,
) -> DescribePartnersOutputMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePartnersOutputMessageTypeDef](./type_defs.md#describepartnersoutputmessagetypedef) 


```python
# describe_partners method usage example with argument unpacking

kwargs: DescribePartnersInputMessageRequestTypeDef = {  # (1)
    "AccountId": ...,
    "ClusterIdentifier": ...,
}

parent.describe_partners(**kwargs)
```

1. See [:material-code-braces: DescribePartnersInputMessageRequestTypeDef](./type_defs.md#describepartnersinputmessagerequesttypedef) 

### describe\_redshift\_idc\_applications

Lists the Amazon Redshift IAM Identity Center applications.

Type annotations and code completion for `#!python session.client("redshift").describe_redshift_idc_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_redshift_idc_applications method definition

await def describe_redshift_idc_applications(
    self,
    *,
    RedshiftIdcApplicationArn: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeRedshiftIdcApplicationsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRedshiftIdcApplicationsResultTypeDef](./type_defs.md#describeredshiftidcapplicationsresulttypedef) 


```python
# describe_redshift_idc_applications method usage example with argument unpacking

kwargs: DescribeRedshiftIdcApplicationsMessageRequestTypeDef = {  # (1)
    "RedshiftIdcApplicationArn": ...,
}

parent.describe_redshift_idc_applications(**kwargs)
```

1. See [:material-code-braces: DescribeRedshiftIdcApplicationsMessageRequestTypeDef](./type_defs.md#describeredshiftidcapplicationsmessagerequesttypedef) 

### describe\_reserved\_node\_exchange\_status

Returns exchange status details and associated metadata for a reserved-node
exchange.

Type annotations and code completion for `#!python session.client("redshift").describe_reserved_node_exchange_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_reserved_node_exchange_status method definition

await def describe_reserved_node_exchange_status(
    self,
    *,
    ReservedNodeId: str = ...,
    ReservedNodeExchangeRequestId: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> DescribeReservedNodeExchangeStatusOutputMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeReservedNodeExchangeStatusOutputMessageTypeDef](./type_defs.md#describereservednodeexchangestatusoutputmessagetypedef) 


```python
# describe_reserved_node_exchange_status method usage example with argument unpacking

kwargs: DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef = {  # (1)
    "ReservedNodeId": ...,
}

parent.describe_reserved_node_exchange_status(**kwargs)
```

1. See [:material-code-braces: DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef](./type_defs.md#describereservednodeexchangestatusinputmessagerequesttypedef) 

### describe\_reserved\_node\_offerings

Returns a list of the available reserved node offerings by Amazon Redshift with
their descriptions including the node type, the fixed and recurring costs of
reserving the node and duration the node will be reserved for you.

Type annotations and code completion for `#!python session.client("redshift").describe_reserved_node_offerings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_reserved_node_offerings method definition

await def describe_reserved_node_offerings(
    self,
    *,
    ReservedNodeOfferingId: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> ReservedNodeOfferingsMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ReservedNodeOfferingsMessageTypeDef](./type_defs.md#reservednodeofferingsmessagetypedef) 


```python
# describe_reserved_node_offerings method usage example with argument unpacking

kwargs: DescribeReservedNodeOfferingsMessageRequestTypeDef = {  # (1)
    "ReservedNodeOfferingId": ...,
}

parent.describe_reserved_node_offerings(**kwargs)
```

1. See [:material-code-braces: DescribeReservedNodeOfferingsMessageRequestTypeDef](./type_defs.md#describereservednodeofferingsmessagerequesttypedef) 

### describe\_reserved\_nodes

Returns the descriptions of the reserved nodes.

Type annotations and code completion for `#!python session.client("redshift").describe_reserved_nodes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_reserved_nodes method definition

await def describe_reserved_nodes(
    self,
    *,
    ReservedNodeId: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> ReservedNodesMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ReservedNodesMessageTypeDef](./type_defs.md#reservednodesmessagetypedef) 


```python
# describe_reserved_nodes method usage example with argument unpacking

kwargs: DescribeReservedNodesMessageRequestTypeDef = {  # (1)
    "ReservedNodeId": ...,
}

parent.describe_reserved_nodes(**kwargs)
```

1. See [:material-code-braces: DescribeReservedNodesMessageRequestTypeDef](./type_defs.md#describereservednodesmessagerequesttypedef) 

### describe\_resize

Returns information about the last resize operation for the specified cluster.

Type annotations and code completion for `#!python session.client("redshift").describe_resize` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_resize method definition

await def describe_resize(
    self,
    *,
    ClusterIdentifier: str,
) -> ResizeProgressMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ResizeProgressMessageTypeDef](./type_defs.md#resizeprogressmessagetypedef) 


```python
# describe_resize method usage example with argument unpacking

kwargs: DescribeResizeMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.describe_resize(**kwargs)
```

1. See [:material-code-braces: DescribeResizeMessageRequestTypeDef](./type_defs.md#describeresizemessagerequesttypedef) 

### describe\_scheduled\_actions

Describes properties of scheduled actions.

Type annotations and code completion for `#!python session.client("redshift").describe_scheduled_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_scheduled_actions method definition

await def describe_scheduled_actions(
    self,
    *,
    ScheduledActionName: str = ...,
    TargetActionType: ScheduledActionTypeValuesType = ...,  # (1)
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    Active: bool = ...,
    Filters: Sequence[ScheduledActionFilterTypeDef] = ...,  # (2)
    Marker: str = ...,
    MaxRecords: int = ...,
) -> ScheduledActionsMessageTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ScheduledActionTypeValuesType](./literals.md#scheduledactiontypevaluestype) 
2. See [:material-code-braces: ScheduledActionFilterTypeDef](./type_defs.md#scheduledactionfiltertypedef) 
3. See [:material-code-braces: ScheduledActionsMessageTypeDef](./type_defs.md#scheduledactionsmessagetypedef) 


```python
# describe_scheduled_actions method usage example with argument unpacking

kwargs: DescribeScheduledActionsMessageRequestTypeDef = {  # (1)
    "ScheduledActionName": ...,
}

parent.describe_scheduled_actions(**kwargs)
```

1. See [:material-code-braces: DescribeScheduledActionsMessageRequestTypeDef](./type_defs.md#describescheduledactionsmessagerequesttypedef) 

### describe\_snapshot\_copy\_grants

Returns a list of snapshot copy grants owned by the Amazon Web Services account
in the destination region.

Type annotations and code completion for `#!python session.client("redshift").describe_snapshot_copy_grants` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_snapshot_copy_grants method definition

await def describe_snapshot_copy_grants(
    self,
    *,
    SnapshotCopyGrantName: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
) -> SnapshotCopyGrantMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SnapshotCopyGrantMessageTypeDef](./type_defs.md#snapshotcopygrantmessagetypedef) 


```python
# describe_snapshot_copy_grants method usage example with argument unpacking

kwargs: DescribeSnapshotCopyGrantsMessageRequestTypeDef = {  # (1)
    "SnapshotCopyGrantName": ...,
}

parent.describe_snapshot_copy_grants(**kwargs)
```

1. See [:material-code-braces: DescribeSnapshotCopyGrantsMessageRequestTypeDef](./type_defs.md#describesnapshotcopygrantsmessagerequesttypedef) 

### describe\_snapshot\_schedules

Returns a list of snapshot schedules.

Type annotations and code completion for `#!python session.client("redshift").describe_snapshot_schedules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_snapshot_schedules method definition

await def describe_snapshot_schedules(
    self,
    *,
    ClusterIdentifier: str = ...,
    ScheduleIdentifier: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    Marker: str = ...,
    MaxRecords: int = ...,
) -> DescribeSnapshotSchedulesOutputMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSnapshotSchedulesOutputMessageTypeDef](./type_defs.md#describesnapshotschedulesoutputmessagetypedef) 


```python
# describe_snapshot_schedules method usage example with argument unpacking

kwargs: DescribeSnapshotSchedulesMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.describe_snapshot_schedules(**kwargs)
```

1. See [:material-code-braces: DescribeSnapshotSchedulesMessageRequestTypeDef](./type_defs.md#describesnapshotschedulesmessagerequesttypedef) 

### describe\_storage

Returns account level backups storage size and provisional storage.

Type annotations and code completion for `#!python session.client("redshift").describe_storage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_storage method definition

await def describe_storage(
    self,
) -> CustomerStorageMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CustomerStorageMessageTypeDef](./type_defs.md#customerstoragemessagetypedef) 

### describe\_table\_restore\_status

Lists the status of one or more table restore requests made using the
<a>RestoreTableFromClusterSnapshot</a> API action.

Type annotations and code completion for `#!python session.client("redshift").describe_table_restore_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_table_restore_status method definition

await def describe_table_restore_status(
    self,
    *,
    ClusterIdentifier: str = ...,
    TableRestoreRequestId: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> TableRestoreStatusMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TableRestoreStatusMessageTypeDef](./type_defs.md#tablerestorestatusmessagetypedef) 


```python
# describe_table_restore_status method usage example with argument unpacking

kwargs: DescribeTableRestoreStatusMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.describe_table_restore_status(**kwargs)
```

1. See [:material-code-braces: DescribeTableRestoreStatusMessageRequestTypeDef](./type_defs.md#describetablerestorestatusmessagerequesttypedef) 

### describe\_tags

Returns a list of tags.

Type annotations and code completion for `#!python session.client("redshift").describe_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_tags method definition

await def describe_tags(
    self,
    *,
    ResourceName: str = ...,
    ResourceType: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
) -> TaggedResourceListMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TaggedResourceListMessageTypeDef](./type_defs.md#taggedresourcelistmessagetypedef) 


```python
# describe_tags method usage example with argument unpacking

kwargs: DescribeTagsMessageRequestTypeDef = {  # (1)
    "ResourceName": ...,
}

parent.describe_tags(**kwargs)
```

1. See [:material-code-braces: DescribeTagsMessageRequestTypeDef](./type_defs.md#describetagsmessagerequesttypedef) 

### describe\_usage\_limits

Shows usage limits on a cluster.

Type annotations and code completion for `#!python session.client("redshift").describe_usage_limits` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# describe_usage_limits method definition

await def describe_usage_limits(
    self,
    *,
    UsageLimitId: str = ...,
    ClusterIdentifier: str = ...,
    FeatureType: UsageLimitFeatureTypeType = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
) -> UsageLimitListTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: UsageLimitFeatureTypeType](./literals.md#usagelimitfeaturetypetype) 
2. See [:material-code-braces: UsageLimitListTypeDef](./type_defs.md#usagelimitlisttypedef) 


```python
# describe_usage_limits method usage example with argument unpacking

kwargs: DescribeUsageLimitsMessageRequestTypeDef = {  # (1)
    "UsageLimitId": ...,
}

parent.describe_usage_limits(**kwargs)
```

1. See [:material-code-braces: DescribeUsageLimitsMessageRequestTypeDef](./type_defs.md#describeusagelimitsmessagerequesttypedef) 

### disable\_logging

Stops logging information, such as queries and connection attempts, for the
specified Amazon Redshift cluster.

Type annotations and code completion for `#!python session.client("redshift").disable_logging` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# disable_logging method definition

await def disable_logging(
    self,
    *,
    ClusterIdentifier: str,
) -> LoggingStatusTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: LoggingStatusTypeDef](./type_defs.md#loggingstatustypedef) 


```python
# disable_logging method usage example with argument unpacking

kwargs: DisableLoggingMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.disable_logging(**kwargs)
```

1. See [:material-code-braces: DisableLoggingMessageRequestTypeDef](./type_defs.md#disableloggingmessagerequesttypedef) 

### disable\_snapshot\_copy

Disables the automatic copying of snapshots from one region to another region
for a specified cluster.

Type annotations and code completion for `#!python session.client("redshift").disable_snapshot_copy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# disable_snapshot_copy method definition

await def disable_snapshot_copy(
    self,
    *,
    ClusterIdentifier: str,
) -> DisableSnapshotCopyResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisableSnapshotCopyResultTypeDef](./type_defs.md#disablesnapshotcopyresulttypedef) 


```python
# disable_snapshot_copy method usage example with argument unpacking

kwargs: DisableSnapshotCopyMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.disable_snapshot_copy(**kwargs)
```

1. See [:material-code-braces: DisableSnapshotCopyMessageRequestTypeDef](./type_defs.md#disablesnapshotcopymessagerequesttypedef) 

### disassociate\_data\_share\_consumer

From a datashare consumer account, remove association for the specified
datashare.

Type annotations and code completion for `#!python session.client("redshift").disassociate_data_share_consumer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# disassociate_data_share_consumer method definition

await def disassociate_data_share_consumer(
    self,
    *,
    DataShareArn: str,
    DisassociateEntireAccount: bool = ...,
    ConsumerArn: str = ...,
    ConsumerRegion: str = ...,
) -> DataShareResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DataShareResponseTypeDef](./type_defs.md#datashareresponsetypedef) 


```python
# disassociate_data_share_consumer method usage example with argument unpacking

kwargs: DisassociateDataShareConsumerMessageRequestTypeDef = {  # (1)
    "DataShareArn": ...,
}

parent.disassociate_data_share_consumer(**kwargs)
```

1. See [:material-code-braces: DisassociateDataShareConsumerMessageRequestTypeDef](./type_defs.md#disassociatedatashareconsumermessagerequesttypedef) 

### enable\_logging

Starts logging information, such as queries and connection attempts, for the
specified Amazon Redshift cluster.

Type annotations and code completion for `#!python session.client("redshift").enable_logging` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# enable_logging method definition

await def enable_logging(
    self,
    *,
    ClusterIdentifier: str,
    BucketName: str = ...,
    S3KeyPrefix: str = ...,
    LogDestinationType: LogDestinationTypeType = ...,  # (1)
    LogExports: Sequence[str] = ...,
) -> LoggingStatusTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LogDestinationTypeType](./literals.md#logdestinationtypetype) 
2. See [:material-code-braces: LoggingStatusTypeDef](./type_defs.md#loggingstatustypedef) 


```python
# enable_logging method usage example with argument unpacking

kwargs: EnableLoggingMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.enable_logging(**kwargs)
```

1. See [:material-code-braces: EnableLoggingMessageRequestTypeDef](./type_defs.md#enableloggingmessagerequesttypedef) 

### enable\_snapshot\_copy

Enables the automatic copy of snapshots from one region to another region for a
specified cluster.

Type annotations and code completion for `#!python session.client("redshift").enable_snapshot_copy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# enable_snapshot_copy method definition

await def enable_snapshot_copy(
    self,
    *,
    ClusterIdentifier: str,
    DestinationRegion: str,
    RetentionPeriod: int = ...,
    SnapshotCopyGrantName: str = ...,
    ManualSnapshotRetentionPeriod: int = ...,
) -> EnableSnapshotCopyResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EnableSnapshotCopyResultTypeDef](./type_defs.md#enablesnapshotcopyresulttypedef) 


```python
# enable_snapshot_copy method usage example with argument unpacking

kwargs: EnableSnapshotCopyMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
    "DestinationRegion": ...,
}

parent.enable_snapshot_copy(**kwargs)
```

1. See [:material-code-braces: EnableSnapshotCopyMessageRequestTypeDef](./type_defs.md#enablesnapshotcopymessagerequesttypedef) 

### failover\_primary\_compute

Fails over the primary compute unit of the specified Multi-AZ cluster to
another Availability Zone.

Type annotations and code completion for `#!python session.client("redshift").failover_primary_compute` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# failover_primary_compute method definition

await def failover_primary_compute(
    self,
    *,
    ClusterIdentifier: str,
) -> FailoverPrimaryComputeResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: FailoverPrimaryComputeResultTypeDef](./type_defs.md#failoverprimarycomputeresulttypedef) 


```python
# failover_primary_compute method usage example with argument unpacking

kwargs: FailoverPrimaryComputeInputMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.failover_primary_compute(**kwargs)
```

1. See [:material-code-braces: FailoverPrimaryComputeInputMessageRequestTypeDef](./type_defs.md#failoverprimarycomputeinputmessagerequesttypedef) 

### get\_cluster\_credentials

Returns a database user name and temporary password with temporary
authorization to log on to an Amazon Redshift database.

Type annotations and code completion for `#!python session.client("redshift").get_cluster_credentials` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# get_cluster_credentials method definition

await def get_cluster_credentials(
    self,
    *,
    DbUser: str,
    DbName: str = ...,
    ClusterIdentifier: str = ...,
    DurationSeconds: int = ...,
    AutoCreate: bool = ...,
    DbGroups: Sequence[str] = ...,
    CustomDomainName: str = ...,
) -> ClusterCredentialsTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ClusterCredentialsTypeDef](./type_defs.md#clustercredentialstypedef) 


```python
# get_cluster_credentials method usage example with argument unpacking

kwargs: GetClusterCredentialsMessageRequestTypeDef = {  # (1)
    "DbUser": ...,
}

parent.get_cluster_credentials(**kwargs)
```

1. See [:material-code-braces: GetClusterCredentialsMessageRequestTypeDef](./type_defs.md#getclustercredentialsmessagerequesttypedef) 

### get\_cluster\_credentials\_with\_iam

Returns a database user name and temporary password with temporary
authorization to log in to an Amazon Redshift database.

Type annotations and code completion for `#!python session.client("redshift").get_cluster_credentials_with_iam` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# get_cluster_credentials_with_iam method definition

await def get_cluster_credentials_with_iam(
    self,
    *,
    DbName: str = ...,
    ClusterIdentifier: str = ...,
    DurationSeconds: int = ...,
    CustomDomainName: str = ...,
) -> ClusterExtendedCredentialsTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ClusterExtendedCredentialsTypeDef](./type_defs.md#clusterextendedcredentialstypedef) 


```python
# get_cluster_credentials_with_iam method usage example with argument unpacking

kwargs: GetClusterCredentialsWithIAMMessageRequestTypeDef = {  # (1)
    "DbName": ...,
}

parent.get_cluster_credentials_with_iam(**kwargs)
```

1. See [:material-code-braces: GetClusterCredentialsWithIAMMessageRequestTypeDef](./type_defs.md#getclustercredentialswithiammessagerequesttypedef) 

### get\_reserved\_node\_exchange\_configuration\_options

Gets the configuration options for the reserved-node exchange.

Type annotations and code completion for `#!python session.client("redshift").get_reserved_node_exchange_configuration_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# get_reserved_node_exchange_configuration_options method definition

await def get_reserved_node_exchange_configuration_options(
    self,
    *,
    ActionType: ReservedNodeExchangeActionTypeType,  # (1)
    ClusterIdentifier: str = ...,
    SnapshotIdentifier: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ReservedNodeExchangeActionTypeType](./literals.md#reservednodeexchangeactiontypetype) 
2. See [:material-code-braces: GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef](./type_defs.md#getreservednodeexchangeconfigurationoptionsoutputmessagetypedef) 


```python
# get_reserved_node_exchange_configuration_options method usage example with argument unpacking

kwargs: GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef = {  # (1)
    "ActionType": ...,
}

parent.get_reserved_node_exchange_configuration_options(**kwargs)
```

1. See [:material-code-braces: GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef](./type_defs.md#getreservednodeexchangeconfigurationoptionsinputmessagerequesttypedef) 

### get\_reserved\_node\_exchange\_offerings

Returns an array of DC2 ReservedNodeOfferings that matches the payment type,
term, and usage price of the given DC1 reserved node.

Type annotations and code completion for `#!python session.client("redshift").get_reserved_node_exchange_offerings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# get_reserved_node_exchange_offerings method definition

await def get_reserved_node_exchange_offerings(
    self,
    *,
    ReservedNodeId: str,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> GetReservedNodeExchangeOfferingsOutputMessageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetReservedNodeExchangeOfferingsOutputMessageTypeDef](./type_defs.md#getreservednodeexchangeofferingsoutputmessagetypedef) 


```python
# get_reserved_node_exchange_offerings method usage example with argument unpacking

kwargs: GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef = {  # (1)
    "ReservedNodeId": ...,
}

parent.get_reserved_node_exchange_offerings(**kwargs)
```

1. See [:material-code-braces: GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef](./type_defs.md#getreservednodeexchangeofferingsinputmessagerequesttypedef) 

### get\_resource\_policy

Get the resource policy for a specified resource.

Type annotations and code completion for `#!python session.client("redshift").get_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# get_resource_policy method definition

await def get_resource_policy(
    self,
    *,
    ResourceArn: str,
) -> GetResourcePolicyResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResourcePolicyResultTypeDef](./type_defs.md#getresourcepolicyresulttypedef) 


```python
# get_resource_policy method usage example with argument unpacking

kwargs: GetResourcePolicyMessageRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.get_resource_policy(**kwargs)
```

1. See [:material-code-braces: GetResourcePolicyMessageRequestTypeDef](./type_defs.md#getresourcepolicymessagerequesttypedef) 

### list\_recommendations

List the Amazon Redshift Advisor recommendations for one or multiple Amazon
Redshift clusters in an Amazon Web Services account.

Type annotations and code completion for `#!python session.client("redshift").list_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# list_recommendations method definition

await def list_recommendations(
    self,
    *,
    ClusterIdentifier: str = ...,
    NamespaceArn: str = ...,
    MaxRecords: int = ...,
    Marker: str = ...,
) -> ListRecommendationsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRecommendationsResultTypeDef](./type_defs.md#listrecommendationsresulttypedef) 


```python
# list_recommendations method usage example with argument unpacking

kwargs: ListRecommendationsMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.list_recommendations(**kwargs)
```

1. See [:material-code-braces: ListRecommendationsMessageRequestTypeDef](./type_defs.md#listrecommendationsmessagerequesttypedef) 

### modify\_aqua\_configuration

This operation is retired.

Type annotations and code completion for `#!python session.client("redshift").modify_aqua_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# modify_aqua_configuration method definition

await def modify_aqua_configuration(
    self,
    *,
    ClusterIdentifier: str,
    AquaConfigurationStatus: AquaConfigurationStatusType = ...,  # (1)
) -> ModifyAquaOutputMessageTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AquaConfigurationStatusType](./literals.md#aquaconfigurationstatustype) 
2. See [:material-code-braces: ModifyAquaOutputMessageTypeDef](./type_defs.md#modifyaquaoutputmessagetypedef) 


```python
# modify_aqua_configuration method usage example with argument unpacking

kwargs: ModifyAquaInputMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.modify_aqua_configuration(**kwargs)
```

1. See [:material-code-braces: ModifyAquaInputMessageRequestTypeDef](./type_defs.md#modifyaquainputmessagerequesttypedef) 

### modify\_authentication\_profile

Modifies an authentication profile.

Type annotations and code completion for `#!python session.client("redshift").modify_authentication_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# modify_authentication_profile method definition

await def modify_authentication_profile(
    self,
    *,
    AuthenticationProfileName: str,
    AuthenticationProfileContent: str,
) -> ModifyAuthenticationProfileResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ModifyAuthenticationProfileResultTypeDef](./type_defs.md#modifyauthenticationprofileresulttypedef) 


```python
# modify_authentication_profile method usage example with argument unpacking

kwargs: ModifyAuthenticationProfileMessageRequestTypeDef = {  # (1)
    "AuthenticationProfileName": ...,
    "AuthenticationProfileContent": ...,
}

parent.modify_authentication_profile(**kwargs)
```

1. See [:material-code-braces: ModifyAuthenticationProfileMessageRequestTypeDef](./type_defs.md#modifyauthenticationprofilemessagerequesttypedef) 

### modify\_cluster

Modifies the settings for a cluster.

Type annotations and code completion for `#!python session.client("redshift").modify_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# modify_cluster method definition

await def modify_cluster(
    self,
    *,
    ClusterIdentifier: str,
    ClusterType: str = ...,
    NodeType: str = ...,
    NumberOfNodes: int = ...,
    ClusterSecurityGroups: Sequence[str] = ...,
    VpcSecurityGroupIds: Sequence[str] = ...,
    MasterUserPassword: str = ...,
    ClusterParameterGroupName: str = ...,
    AutomatedSnapshotRetentionPeriod: int = ...,
    ManualSnapshotRetentionPeriod: int = ...,
    PreferredMaintenanceWindow: str = ...,
    ClusterVersion: str = ...,
    AllowVersionUpgrade: bool = ...,
    HsmClientCertificateIdentifier: str = ...,
    HsmConfigurationIdentifier: str = ...,
    NewClusterIdentifier: str = ...,
    PubliclyAccessible: bool = ...,
    ElasticIp: str = ...,
    EnhancedVpcRouting: bool = ...,
    MaintenanceTrackName: str = ...,
    Encrypted: bool = ...,
    KmsKeyId: str = ...,
    AvailabilityZoneRelocation: bool = ...,
    AvailabilityZone: str = ...,
    Port: int = ...,
    ManageMasterPassword: bool = ...,
    MasterPasswordSecretKmsKeyId: str = ...,
    IpAddressType: str = ...,
    MultiAZ: bool = ...,
) -> ModifyClusterResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ModifyClusterResultTypeDef](./type_defs.md#modifyclusterresulttypedef) 


```python
# modify_cluster method usage example with argument unpacking

kwargs: ModifyClusterMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.modify_cluster(**kwargs)
```

1. See [:material-code-braces: ModifyClusterMessageRequestTypeDef](./type_defs.md#modifyclustermessagerequesttypedef) 

### modify\_cluster\_db\_revision

Modifies the database revision of a cluster.

Type annotations and code completion for `#!python session.client("redshift").modify_cluster_db_revision` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# modify_cluster_db_revision method definition

await def modify_cluster_db_revision(
    self,
    *,
    ClusterIdentifier: str,
    RevisionTarget: str,
) -> ModifyClusterDbRevisionResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ModifyClusterDbRevisionResultTypeDef](./type_defs.md#modifyclusterdbrevisionresulttypedef) 


```python
# modify_cluster_db_revision method usage example with argument unpacking

kwargs: ModifyClusterDbRevisionMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
    "RevisionTarget": ...,
}

parent.modify_cluster_db_revision(**kwargs)
```

1. See [:material-code-braces: ModifyClusterDbRevisionMessageRequestTypeDef](./type_defs.md#modifyclusterdbrevisionmessagerequesttypedef) 

### modify\_cluster\_iam\_roles

Modifies the list of Identity and Access Management (IAM) roles that can be
used by the cluster to access other Amazon Web Services services.

Type annotations and code completion for `#!python session.client("redshift").modify_cluster_iam_roles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# modify_cluster_iam_roles method definition

await def modify_cluster_iam_roles(
    self,
    *,
    ClusterIdentifier: str,
    AddIamRoles: Sequence[str] = ...,
    RemoveIamRoles: Sequence[str] = ...,
    DefaultIamRoleArn: str = ...,
) -> ModifyClusterIamRolesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ModifyClusterIamRolesResultTypeDef](./type_defs.md#modifyclusteriamrolesresulttypedef) 


```python
# modify_cluster_iam_roles method usage example with argument unpacking

kwargs: ModifyClusterIamRolesMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.modify_cluster_iam_roles(**kwargs)
```

1. See [:material-code-braces: ModifyClusterIamRolesMessageRequestTypeDef](./type_defs.md#modifyclusteriamrolesmessagerequesttypedef) 

### modify\_cluster\_maintenance

Modifies the maintenance settings of a cluster.

Type annotations and code completion for `#!python session.client("redshift").modify_cluster_maintenance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# modify_cluster_maintenance method definition

await def modify_cluster_maintenance(
    self,
    *,
    ClusterIdentifier: str,
    DeferMaintenance: bool = ...,
    DeferMaintenanceIdentifier: str = ...,
    DeferMaintenanceStartTime: TimestampTypeDef = ...,
    DeferMaintenanceEndTime: TimestampTypeDef = ...,
    DeferMaintenanceDuration: int = ...,
) -> ModifyClusterMaintenanceResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ModifyClusterMaintenanceResultTypeDef](./type_defs.md#modifyclustermaintenanceresulttypedef) 


```python
# modify_cluster_maintenance method usage example with argument unpacking

kwargs: ModifyClusterMaintenanceMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.modify_cluster_maintenance(**kwargs)
```

1. See [:material-code-braces: ModifyClusterMaintenanceMessageRequestTypeDef](./type_defs.md#modifyclustermaintenancemessagerequesttypedef) 

### modify\_cluster\_parameter\_group

Modifies the parameters of a parameter group.

Type annotations and code completion for `#!python session.client("redshift").modify_cluster_parameter_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# modify_cluster_parameter_group method definition

await def modify_cluster_parameter_group(
    self,
    *,
    ParameterGroupName: str,
    Parameters: Sequence[ParameterTypeDef],  # (1)
) -> ClusterParameterGroupNameMessageTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
2. See [:material-code-braces: ClusterParameterGroupNameMessageTypeDef](./type_defs.md#clusterparametergroupnamemessagetypedef) 


```python
# modify_cluster_parameter_group method usage example with argument unpacking

kwargs: ModifyClusterParameterGroupMessageRequestTypeDef = {  # (1)
    "ParameterGroupName": ...,
    "Parameters": ...,
}

parent.modify_cluster_parameter_group(**kwargs)
```

1. See [:material-code-braces: ModifyClusterParameterGroupMessageRequestTypeDef](./type_defs.md#modifyclusterparametergroupmessagerequesttypedef) 

### modify\_cluster\_snapshot

Modifies the settings for a snapshot.

Type annotations and code completion for `#!python session.client("redshift").modify_cluster_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# modify_cluster_snapshot method definition

await def modify_cluster_snapshot(
    self,
    *,
    SnapshotIdentifier: str,
    ManualSnapshotRetentionPeriod: int = ...,
    Force: bool = ...,
) -> ModifyClusterSnapshotResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ModifyClusterSnapshotResultTypeDef](./type_defs.md#modifyclustersnapshotresulttypedef) 


```python
# modify_cluster_snapshot method usage example with argument unpacking

kwargs: ModifyClusterSnapshotMessageRequestTypeDef = {  # (1)
    "SnapshotIdentifier": ...,
}

parent.modify_cluster_snapshot(**kwargs)
```

1. See [:material-code-braces: ModifyClusterSnapshotMessageRequestTypeDef](./type_defs.md#modifyclustersnapshotmessagerequesttypedef) 

### modify\_cluster\_snapshot\_schedule

Modifies a snapshot schedule for a cluster.

Type annotations and code completion for `#!python session.client("redshift").modify_cluster_snapshot_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# modify_cluster_snapshot_schedule method definition

await def modify_cluster_snapshot_schedule(
    self,
    *,
    ClusterIdentifier: str,
    ScheduleIdentifier: str = ...,
    DisassociateSchedule: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# modify_cluster_snapshot_schedule method usage example with argument unpacking

kwargs: ModifyClusterSnapshotScheduleMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.modify_cluster_snapshot_schedule(**kwargs)
```

1. See [:material-code-braces: ModifyClusterSnapshotScheduleMessageRequestTypeDef](./type_defs.md#modifyclustersnapshotschedulemessagerequesttypedef) 

### modify\_cluster\_subnet\_group

Modifies a cluster subnet group to include the specified list of VPC subnets.

Type annotations and code completion for `#!python session.client("redshift").modify_cluster_subnet_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# modify_cluster_subnet_group method definition

await def modify_cluster_subnet_group(
    self,
    *,
    ClusterSubnetGroupName: str,
    SubnetIds: Sequence[str],
    Description: str = ...,
) -> ModifyClusterSubnetGroupResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ModifyClusterSubnetGroupResultTypeDef](./type_defs.md#modifyclustersubnetgroupresulttypedef) 


```python
# modify_cluster_subnet_group method usage example with argument unpacking

kwargs: ModifyClusterSubnetGroupMessageRequestTypeDef = {  # (1)
    "ClusterSubnetGroupName": ...,
    "SubnetIds": ...,
}

parent.modify_cluster_subnet_group(**kwargs)
```

1. See [:material-code-braces: ModifyClusterSubnetGroupMessageRequestTypeDef](./type_defs.md#modifyclustersubnetgroupmessagerequesttypedef) 

### modify\_custom\_domain\_association

Contains information for changing a custom domain association.

Type annotations and code completion for `#!python session.client("redshift").modify_custom_domain_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# modify_custom_domain_association method definition

await def modify_custom_domain_association(
    self,
    *,
    CustomDomainName: str,
    CustomDomainCertificateArn: str,
    ClusterIdentifier: str,
) -> ModifyCustomDomainAssociationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ModifyCustomDomainAssociationResultTypeDef](./type_defs.md#modifycustomdomainassociationresulttypedef) 


```python
# modify_custom_domain_association method usage example with argument unpacking

kwargs: ModifyCustomDomainAssociationMessageRequestTypeDef = {  # (1)
    "CustomDomainName": ...,
    "CustomDomainCertificateArn": ...,
    "ClusterIdentifier": ...,
}

parent.modify_custom_domain_association(**kwargs)
```

1. See [:material-code-braces: ModifyCustomDomainAssociationMessageRequestTypeDef](./type_defs.md#modifycustomdomainassociationmessagerequesttypedef) 

### modify\_endpoint\_access

Modifies a Redshift-managed VPC endpoint.

Type annotations and code completion for `#!python session.client("redshift").modify_endpoint_access` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# modify_endpoint_access method definition

await def modify_endpoint_access(
    self,
    *,
    EndpointName: str,
    VpcSecurityGroupIds: Sequence[str] = ...,
) -> EndpointAccessResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EndpointAccessResponseTypeDef](./type_defs.md#endpointaccessresponsetypedef) 


```python
# modify_endpoint_access method usage example with argument unpacking

kwargs: ModifyEndpointAccessMessageRequestTypeDef = {  # (1)
    "EndpointName": ...,
}

parent.modify_endpoint_access(**kwargs)
```

1. See [:material-code-braces: ModifyEndpointAccessMessageRequestTypeDef](./type_defs.md#modifyendpointaccessmessagerequesttypedef) 

### modify\_event\_subscription

Modifies an existing Amazon Redshift event notification subscription.

Type annotations and code completion for `#!python session.client("redshift").modify_event_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# modify_event_subscription method definition

await def modify_event_subscription(
    self,
    *,
    SubscriptionName: str,
    SnsTopicArn: str = ...,
    SourceType: str = ...,
    SourceIds: Sequence[str] = ...,
    EventCategories: Sequence[str] = ...,
    Severity: str = ...,
    Enabled: bool = ...,
) -> ModifyEventSubscriptionResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ModifyEventSubscriptionResultTypeDef](./type_defs.md#modifyeventsubscriptionresulttypedef) 


```python
# modify_event_subscription method usage example with argument unpacking

kwargs: ModifyEventSubscriptionMessageRequestTypeDef = {  # (1)
    "SubscriptionName": ...,
}

parent.modify_event_subscription(**kwargs)
```

1. See [:material-code-braces: ModifyEventSubscriptionMessageRequestTypeDef](./type_defs.md#modifyeventsubscriptionmessagerequesttypedef) 

### modify\_integration

Modifies a zero-ETL integration or S3 event integration with Amazon Redshift.

Type annotations and code completion for `#!python session.client("redshift").modify_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# modify_integration method definition

await def modify_integration(
    self,
    *,
    IntegrationArn: str,
    Description: str = ...,
    IntegrationName: str = ...,
) -> IntegrationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: IntegrationResponseTypeDef](./type_defs.md#integrationresponsetypedef) 


```python
# modify_integration method usage example with argument unpacking

kwargs: ModifyIntegrationMessageRequestTypeDef = {  # (1)
    "IntegrationArn": ...,
}

parent.modify_integration(**kwargs)
```

1. See [:material-code-braces: ModifyIntegrationMessageRequestTypeDef](./type_defs.md#modifyintegrationmessagerequesttypedef) 

### modify\_redshift\_idc\_application

Changes an existing Amazon Redshift IAM Identity Center application.

Type annotations and code completion for `#!python session.client("redshift").modify_redshift_idc_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# modify_redshift_idc_application method definition

await def modify_redshift_idc_application(
    self,
    *,
    RedshiftIdcApplicationArn: str,
    IdentityNamespace: str = ...,
    IamRoleArn: str = ...,
    IdcDisplayName: str = ...,
    AuthorizedTokenIssuerList: Sequence[AuthorizedTokenIssuerTypeDef] = ...,  # (1)
    ServiceIntegrations: Sequence[ServiceIntegrationsUnionTypeDef] = ...,  # (2)
) -> ModifyRedshiftIdcApplicationResultTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AuthorizedTokenIssuerTypeDef](./type_defs.md#authorizedtokenissuertypedef) 
2. See [:material-code-braces: ServiceIntegrationsUnionTypeDef](./type_defs.md#serviceintegrationsuniontypedef) 
3. See [:material-code-braces: ModifyRedshiftIdcApplicationResultTypeDef](./type_defs.md#modifyredshiftidcapplicationresulttypedef) 


```python
# modify_redshift_idc_application method usage example with argument unpacking

kwargs: ModifyRedshiftIdcApplicationMessageRequestTypeDef = {  # (1)
    "RedshiftIdcApplicationArn": ...,
}

parent.modify_redshift_idc_application(**kwargs)
```

1. See [:material-code-braces: ModifyRedshiftIdcApplicationMessageRequestTypeDef](./type_defs.md#modifyredshiftidcapplicationmessagerequesttypedef) 

### modify\_scheduled\_action

Modifies a scheduled action.

Type annotations and code completion for `#!python session.client("redshift").modify_scheduled_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# modify_scheduled_action method definition

await def modify_scheduled_action(
    self,
    *,
    ScheduledActionName: str,
    TargetAction: ScheduledActionTypeTypeDef = ...,  # (1)
    Schedule: str = ...,
    IamRole: str = ...,
    ScheduledActionDescription: str = ...,
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    Enable: bool = ...,
) -> ScheduledActionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ScheduledActionTypeTypeDef](./type_defs.md#scheduledactiontypetypedef) 
2. See [:material-code-braces: ScheduledActionResponseTypeDef](./type_defs.md#scheduledactionresponsetypedef) 


```python
# modify_scheduled_action method usage example with argument unpacking

kwargs: ModifyScheduledActionMessageRequestTypeDef = {  # (1)
    "ScheduledActionName": ...,
}

parent.modify_scheduled_action(**kwargs)
```

1. See [:material-code-braces: ModifyScheduledActionMessageRequestTypeDef](./type_defs.md#modifyscheduledactionmessagerequesttypedef) 

### modify\_snapshot\_copy\_retention\_period

Modifies the number of days to retain snapshots in the destination Amazon Web
Services Region after they are copied from the source Amazon Web Services
Region.

Type annotations and code completion for `#!python session.client("redshift").modify_snapshot_copy_retention_period` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# modify_snapshot_copy_retention_period method definition

await def modify_snapshot_copy_retention_period(
    self,
    *,
    ClusterIdentifier: str,
    RetentionPeriod: int,
    Manual: bool = ...,
) -> ModifySnapshotCopyRetentionPeriodResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ModifySnapshotCopyRetentionPeriodResultTypeDef](./type_defs.md#modifysnapshotcopyretentionperiodresulttypedef) 


```python
# modify_snapshot_copy_retention_period method usage example with argument unpacking

kwargs: ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
    "RetentionPeriod": ...,
}

parent.modify_snapshot_copy_retention_period(**kwargs)
```

1. See [:material-code-braces: ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef](./type_defs.md#modifysnapshotcopyretentionperiodmessagerequesttypedef) 

### modify\_snapshot\_schedule

Modifies a snapshot schedule.

Type annotations and code completion for `#!python session.client("redshift").modify_snapshot_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# modify_snapshot_schedule method definition

await def modify_snapshot_schedule(
    self,
    *,
    ScheduleIdentifier: str,
    ScheduleDefinitions: Sequence[str],
) -> SnapshotScheduleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SnapshotScheduleResponseTypeDef](./type_defs.md#snapshotscheduleresponsetypedef) 


```python
# modify_snapshot_schedule method usage example with argument unpacking

kwargs: ModifySnapshotScheduleMessageRequestTypeDef = {  # (1)
    "ScheduleIdentifier": ...,
    "ScheduleDefinitions": ...,
}

parent.modify_snapshot_schedule(**kwargs)
```

1. See [:material-code-braces: ModifySnapshotScheduleMessageRequestTypeDef](./type_defs.md#modifysnapshotschedulemessagerequesttypedef) 

### modify\_usage\_limit

Modifies a usage limit in a cluster.

Type annotations and code completion for `#!python session.client("redshift").modify_usage_limit` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# modify_usage_limit method definition

await def modify_usage_limit(
    self,
    *,
    UsageLimitId: str,
    Amount: int = ...,
    BreachAction: UsageLimitBreachActionType = ...,  # (1)
) -> UsageLimitResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: UsageLimitBreachActionType](./literals.md#usagelimitbreachactiontype) 
2. See [:material-code-braces: UsageLimitResponseTypeDef](./type_defs.md#usagelimitresponsetypedef) 


```python
# modify_usage_limit method usage example with argument unpacking

kwargs: ModifyUsageLimitMessageRequestTypeDef = {  # (1)
    "UsageLimitId": ...,
}

parent.modify_usage_limit(**kwargs)
```

1. See [:material-code-braces: ModifyUsageLimitMessageRequestTypeDef](./type_defs.md#modifyusagelimitmessagerequesttypedef) 

### pause\_cluster

Pauses a cluster.

Type annotations and code completion for `#!python session.client("redshift").pause_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# pause_cluster method definition

await def pause_cluster(
    self,
    *,
    ClusterIdentifier: str,
) -> PauseClusterResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PauseClusterResultTypeDef](./type_defs.md#pauseclusterresulttypedef) 


```python
# pause_cluster method usage example with argument unpacking

kwargs: PauseClusterMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.pause_cluster(**kwargs)
```

1. See [:material-code-braces: PauseClusterMessageRequestTypeDef](./type_defs.md#pauseclustermessagerequesttypedef) 

### purchase\_reserved\_node\_offering

Allows you to purchase reserved nodes.

Type annotations and code completion for `#!python session.client("redshift").purchase_reserved_node_offering` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# purchase_reserved_node_offering method definition

await def purchase_reserved_node_offering(
    self,
    *,
    ReservedNodeOfferingId: str,
    NodeCount: int = ...,
) -> PurchaseReservedNodeOfferingResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PurchaseReservedNodeOfferingResultTypeDef](./type_defs.md#purchasereservednodeofferingresulttypedef) 


```python
# purchase_reserved_node_offering method usage example with argument unpacking

kwargs: PurchaseReservedNodeOfferingMessageRequestTypeDef = {  # (1)
    "ReservedNodeOfferingId": ...,
}

parent.purchase_reserved_node_offering(**kwargs)
```

1. See [:material-code-braces: PurchaseReservedNodeOfferingMessageRequestTypeDef](./type_defs.md#purchasereservednodeofferingmessagerequesttypedef) 

### put\_resource\_policy

Updates the resource policy for a specified resource.

Type annotations and code completion for `#!python session.client("redshift").put_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# put_resource_policy method definition

await def put_resource_policy(
    self,
    *,
    ResourceArn: str,
    Policy: str,
) -> PutResourcePolicyResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutResourcePolicyResultTypeDef](./type_defs.md#putresourcepolicyresulttypedef) 


```python
# put_resource_policy method usage example with argument unpacking

kwargs: PutResourcePolicyMessageRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Policy": ...,
}

parent.put_resource_policy(**kwargs)
```

1. See [:material-code-braces: PutResourcePolicyMessageRequestTypeDef](./type_defs.md#putresourcepolicymessagerequesttypedef) 

### reboot\_cluster

Reboots a cluster.

Type annotations and code completion for `#!python session.client("redshift").reboot_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# reboot_cluster method definition

await def reboot_cluster(
    self,
    *,
    ClusterIdentifier: str,
) -> RebootClusterResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RebootClusterResultTypeDef](./type_defs.md#rebootclusterresulttypedef) 


```python
# reboot_cluster method usage example with argument unpacking

kwargs: RebootClusterMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.reboot_cluster(**kwargs)
```

1. See [:material-code-braces: RebootClusterMessageRequestTypeDef](./type_defs.md#rebootclustermessagerequesttypedef) 

### register\_namespace

Registers a cluster or serverless namespace to the Amazon Web Services Glue
Data Catalog.

Type annotations and code completion for `#!python session.client("redshift").register_namespace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# register_namespace method definition

await def register_namespace(
    self,
    *,
    NamespaceIdentifier: NamespaceIdentifierUnionTypeDef,  # (1)
    ConsumerIdentifiers: Sequence[str],
) -> RegisterNamespaceOutputMessageTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: NamespaceIdentifierUnionTypeDef](./type_defs.md#namespaceidentifieruniontypedef) 
2. See [:material-code-braces: RegisterNamespaceOutputMessageTypeDef](./type_defs.md#registernamespaceoutputmessagetypedef) 


```python
# register_namespace method usage example with argument unpacking

kwargs: RegisterNamespaceInputMessageRequestTypeDef = {  # (1)
    "NamespaceIdentifier": ...,
    "ConsumerIdentifiers": ...,
}

parent.register_namespace(**kwargs)
```

1. See [:material-code-braces: RegisterNamespaceInputMessageRequestTypeDef](./type_defs.md#registernamespaceinputmessagerequesttypedef) 

### reject\_data\_share

From a datashare consumer account, rejects the specified datashare.

Type annotations and code completion for `#!python session.client("redshift").reject_data_share` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# reject_data_share method definition

await def reject_data_share(
    self,
    *,
    DataShareArn: str,
) -> DataShareResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DataShareResponseTypeDef](./type_defs.md#datashareresponsetypedef) 


```python
# reject_data_share method usage example with argument unpacking

kwargs: RejectDataShareMessageRequestTypeDef = {  # (1)
    "DataShareArn": ...,
}

parent.reject_data_share(**kwargs)
```

1. See [:material-code-braces: RejectDataShareMessageRequestTypeDef](./type_defs.md#rejectdatasharemessagerequesttypedef) 

### reset\_cluster\_parameter\_group

Sets one or more parameters of the specified parameter group to their default
values and sets the source values of the parameters to "engine-default".

Type annotations and code completion for `#!python session.client("redshift").reset_cluster_parameter_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# reset_cluster_parameter_group method definition

await def reset_cluster_parameter_group(
    self,
    *,
    ParameterGroupName: str,
    ResetAllParameters: bool = ...,
    Parameters: Sequence[ParameterTypeDef] = ...,  # (1)
) -> ClusterParameterGroupNameMessageTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
2. See [:material-code-braces: ClusterParameterGroupNameMessageTypeDef](./type_defs.md#clusterparametergroupnamemessagetypedef) 


```python
# reset_cluster_parameter_group method usage example with argument unpacking

kwargs: ResetClusterParameterGroupMessageRequestTypeDef = {  # (1)
    "ParameterGroupName": ...,
}

parent.reset_cluster_parameter_group(**kwargs)
```

1. See [:material-code-braces: ResetClusterParameterGroupMessageRequestTypeDef](./type_defs.md#resetclusterparametergroupmessagerequesttypedef) 

### resize\_cluster

Changes the size of the cluster.

Type annotations and code completion for `#!python session.client("redshift").resize_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# resize_cluster method definition

await def resize_cluster(
    self,
    *,
    ClusterIdentifier: str,
    ClusterType: str = ...,
    NodeType: str = ...,
    NumberOfNodes: int = ...,
    Classic: bool = ...,
    ReservedNodeId: str = ...,
    TargetReservedNodeOfferingId: str = ...,
) -> ResizeClusterResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ResizeClusterResultTypeDef](./type_defs.md#resizeclusterresulttypedef) 


```python
# resize_cluster method usage example with argument unpacking

kwargs: ResizeClusterMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.resize_cluster(**kwargs)
```

1. See [:material-code-braces: ResizeClusterMessageRequestTypeDef](./type_defs.md#resizeclustermessagerequesttypedef) 

### restore\_from\_cluster\_snapshot

Creates a new cluster from a snapshot.

Type annotations and code completion for `#!python session.client("redshift").restore_from_cluster_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# restore_from_cluster_snapshot method definition

await def restore_from_cluster_snapshot(
    self,
    *,
    ClusterIdentifier: str,
    SnapshotIdentifier: str = ...,
    SnapshotArn: str = ...,
    SnapshotClusterIdentifier: str = ...,
    Port: int = ...,
    AvailabilityZone: str = ...,
    AllowVersionUpgrade: bool = ...,
    ClusterSubnetGroupName: str = ...,
    PubliclyAccessible: bool = ...,
    OwnerAccount: str = ...,
    HsmClientCertificateIdentifier: str = ...,
    HsmConfigurationIdentifier: str = ...,
    ElasticIp: str = ...,
    ClusterParameterGroupName: str = ...,
    ClusterSecurityGroups: Sequence[str] = ...,
    VpcSecurityGroupIds: Sequence[str] = ...,
    PreferredMaintenanceWindow: str = ...,
    AutomatedSnapshotRetentionPeriod: int = ...,
    ManualSnapshotRetentionPeriod: int = ...,
    KmsKeyId: str = ...,
    NodeType: str = ...,
    EnhancedVpcRouting: bool = ...,
    AdditionalInfo: str = ...,
    IamRoles: Sequence[str] = ...,
    MaintenanceTrackName: str = ...,
    SnapshotScheduleIdentifier: str = ...,
    NumberOfNodes: int = ...,
    AvailabilityZoneRelocation: bool = ...,
    AquaConfigurationStatus: AquaConfigurationStatusType = ...,  # (1)
    DefaultIamRoleArn: str = ...,
    ReservedNodeId: str = ...,
    TargetReservedNodeOfferingId: str = ...,
    Encrypted: bool = ...,
    ManageMasterPassword: bool = ...,
    MasterPasswordSecretKmsKeyId: str = ...,
    IpAddressType: str = ...,
    MultiAZ: bool = ...,
) -> RestoreFromClusterSnapshotResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AquaConfigurationStatusType](./literals.md#aquaconfigurationstatustype) 
2. See [:material-code-braces: RestoreFromClusterSnapshotResultTypeDef](./type_defs.md#restorefromclustersnapshotresulttypedef) 


```python
# restore_from_cluster_snapshot method usage example with argument unpacking

kwargs: RestoreFromClusterSnapshotMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.restore_from_cluster_snapshot(**kwargs)
```

1. See [:material-code-braces: RestoreFromClusterSnapshotMessageRequestTypeDef](./type_defs.md#restorefromclustersnapshotmessagerequesttypedef) 

### restore\_table\_from\_cluster\_snapshot

Creates a new table from a table in an Amazon Redshift cluster snapshot.

Type annotations and code completion for `#!python session.client("redshift").restore_table_from_cluster_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# restore_table_from_cluster_snapshot method definition

await def restore_table_from_cluster_snapshot(
    self,
    *,
    ClusterIdentifier: str,
    SnapshotIdentifier: str,
    SourceDatabaseName: str,
    SourceTableName: str,
    NewTableName: str,
    SourceSchemaName: str = ...,
    TargetDatabaseName: str = ...,
    TargetSchemaName: str = ...,
    EnableCaseSensitiveIdentifier: bool = ...,
) -> RestoreTableFromClusterSnapshotResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RestoreTableFromClusterSnapshotResultTypeDef](./type_defs.md#restoretablefromclustersnapshotresulttypedef) 


```python
# restore_table_from_cluster_snapshot method usage example with argument unpacking

kwargs: RestoreTableFromClusterSnapshotMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
    "SnapshotIdentifier": ...,
    "SourceDatabaseName": ...,
    "SourceTableName": ...,
    "NewTableName": ...,
}

parent.restore_table_from_cluster_snapshot(**kwargs)
```

1. See [:material-code-braces: RestoreTableFromClusterSnapshotMessageRequestTypeDef](./type_defs.md#restoretablefromclustersnapshotmessagerequesttypedef) 

### resume\_cluster

Resumes a paused cluster.

Type annotations and code completion for `#!python session.client("redshift").resume_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# resume_cluster method definition

await def resume_cluster(
    self,
    *,
    ClusterIdentifier: str,
) -> ResumeClusterResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ResumeClusterResultTypeDef](./type_defs.md#resumeclusterresulttypedef) 


```python
# resume_cluster method usage example with argument unpacking

kwargs: ResumeClusterMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.resume_cluster(**kwargs)
```

1. See [:material-code-braces: ResumeClusterMessageRequestTypeDef](./type_defs.md#resumeclustermessagerequesttypedef) 

### revoke\_cluster\_security\_group\_ingress

Revokes an ingress rule in an Amazon Redshift security group for a previously
authorized IP range or Amazon EC2 security group.

Type annotations and code completion for `#!python session.client("redshift").revoke_cluster_security_group_ingress` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# revoke_cluster_security_group_ingress method definition

await def revoke_cluster_security_group_ingress(
    self,
    *,
    ClusterSecurityGroupName: str,
    CIDRIP: str = ...,
    EC2SecurityGroupName: str = ...,
    EC2SecurityGroupOwnerId: str = ...,
) -> RevokeClusterSecurityGroupIngressResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RevokeClusterSecurityGroupIngressResultTypeDef](./type_defs.md#revokeclustersecuritygroupingressresulttypedef) 


```python
# revoke_cluster_security_group_ingress method usage example with argument unpacking

kwargs: RevokeClusterSecurityGroupIngressMessageRequestTypeDef = {  # (1)
    "ClusterSecurityGroupName": ...,
}

parent.revoke_cluster_security_group_ingress(**kwargs)
```

1. See [:material-code-braces: RevokeClusterSecurityGroupIngressMessageRequestTypeDef](./type_defs.md#revokeclustersecuritygroupingressmessagerequesttypedef) 

### revoke\_endpoint\_access

Revokes access to a cluster.

Type annotations and code completion for `#!python session.client("redshift").revoke_endpoint_access` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# revoke_endpoint_access method definition

await def revoke_endpoint_access(
    self,
    *,
    ClusterIdentifier: str = ...,
    Account: str = ...,
    VpcIds: Sequence[str] = ...,
    Force: bool = ...,
) -> EndpointAuthorizationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EndpointAuthorizationResponseTypeDef](./type_defs.md#endpointauthorizationresponsetypedef) 


```python
# revoke_endpoint_access method usage example with argument unpacking

kwargs: RevokeEndpointAccessMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.revoke_endpoint_access(**kwargs)
```

1. See [:material-code-braces: RevokeEndpointAccessMessageRequestTypeDef](./type_defs.md#revokeendpointaccessmessagerequesttypedef) 

### revoke\_snapshot\_access

Removes the ability of the specified Amazon Web Services account to restore the
specified snapshot.

Type annotations and code completion for `#!python session.client("redshift").revoke_snapshot_access` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# revoke_snapshot_access method definition

await def revoke_snapshot_access(
    self,
    *,
    AccountWithRestoreAccess: str,
    SnapshotIdentifier: str = ...,
    SnapshotArn: str = ...,
    SnapshotClusterIdentifier: str = ...,
) -> RevokeSnapshotAccessResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RevokeSnapshotAccessResultTypeDef](./type_defs.md#revokesnapshotaccessresulttypedef) 


```python
# revoke_snapshot_access method usage example with argument unpacking

kwargs: RevokeSnapshotAccessMessageRequestTypeDef = {  # (1)
    "AccountWithRestoreAccess": ...,
}

parent.revoke_snapshot_access(**kwargs)
```

1. See [:material-code-braces: RevokeSnapshotAccessMessageRequestTypeDef](./type_defs.md#revokesnapshotaccessmessagerequesttypedef) 

### rotate\_encryption\_key

Rotates the encryption keys for a cluster.

Type annotations and code completion for `#!python session.client("redshift").rotate_encryption_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# rotate_encryption_key method definition

await def rotate_encryption_key(
    self,
    *,
    ClusterIdentifier: str,
) -> RotateEncryptionKeyResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RotateEncryptionKeyResultTypeDef](./type_defs.md#rotateencryptionkeyresulttypedef) 


```python
# rotate_encryption_key method usage example with argument unpacking

kwargs: RotateEncryptionKeyMessageRequestTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.rotate_encryption_key(**kwargs)
```

1. See [:material-code-braces: RotateEncryptionKeyMessageRequestTypeDef](./type_defs.md#rotateencryptionkeymessagerequesttypedef) 

### update\_partner\_status

Updates the status of a partner integration.

Type annotations and code completion for `#!python session.client("redshift").update_partner_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# update_partner_status method definition

await def update_partner_status(
    self,
    *,
    AccountId: str,
    ClusterIdentifier: str,
    DatabaseName: str,
    PartnerName: str,
    Status: PartnerIntegrationStatusType,  # (1)
    StatusMessage: str = ...,
) -> PartnerIntegrationOutputMessageTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PartnerIntegrationStatusType](./literals.md#partnerintegrationstatustype) 
2. See [:material-code-braces: PartnerIntegrationOutputMessageTypeDef](./type_defs.md#partnerintegrationoutputmessagetypedef) 


```python
# update_partner_status method usage example with argument unpacking

kwargs: UpdatePartnerStatusInputMessageRequestTypeDef = {  # (1)
    "AccountId": ...,
    "ClusterIdentifier": ...,
    "DatabaseName": ...,
    "PartnerName": ...,
    "Status": ...,
}

parent.update_partner_status(**kwargs)
```

1. See [:material-code-braces: UpdatePartnerStatusInputMessageRequestTypeDef](./type_defs.md#updatepartnerstatusinputmessagerequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("redshift").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("redshift").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)

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

Type annotations and code completion for `#!python session.client("redshift").get_paginator` method with overloads.

- `client.get_paginator("describe_cluster_db_revisions")` -> [DescribeClusterDbRevisionsPaginator](./paginators.md#describeclusterdbrevisionspaginator)
- `client.get_paginator("describe_cluster_parameter_groups")` -> [DescribeClusterParameterGroupsPaginator](./paginators.md#describeclusterparametergroupspaginator)
- `client.get_paginator("describe_cluster_parameters")` -> [DescribeClusterParametersPaginator](./paginators.md#describeclusterparameterspaginator)
- `client.get_paginator("describe_cluster_security_groups")` -> [DescribeClusterSecurityGroupsPaginator](./paginators.md#describeclustersecuritygroupspaginator)
- `client.get_paginator("describe_cluster_snapshots")` -> [DescribeClusterSnapshotsPaginator](./paginators.md#describeclustersnapshotspaginator)
- `client.get_paginator("describe_cluster_subnet_groups")` -> [DescribeClusterSubnetGroupsPaginator](./paginators.md#describeclustersubnetgroupspaginator)
- `client.get_paginator("describe_cluster_tracks")` -> [DescribeClusterTracksPaginator](./paginators.md#describeclustertrackspaginator)
- `client.get_paginator("describe_cluster_versions")` -> [DescribeClusterVersionsPaginator](./paginators.md#describeclusterversionspaginator)
- `client.get_paginator("describe_clusters")` -> [DescribeClustersPaginator](./paginators.md#describeclusterspaginator)
- `client.get_paginator("describe_custom_domain_associations")` -> [DescribeCustomDomainAssociationsPaginator](./paginators.md#describecustomdomainassociationspaginator)
- `client.get_paginator("describe_data_shares_for_consumer")` -> [DescribeDataSharesForConsumerPaginator](./paginators.md#describedatasharesforconsumerpaginator)
- `client.get_paginator("describe_data_shares_for_producer")` -> [DescribeDataSharesForProducerPaginator](./paginators.md#describedatasharesforproducerpaginator)
- `client.get_paginator("describe_data_shares")` -> [DescribeDataSharesPaginator](./paginators.md#describedatasharespaginator)
- `client.get_paginator("describe_default_cluster_parameters")` -> [DescribeDefaultClusterParametersPaginator](./paginators.md#describedefaultclusterparameterspaginator)
- `client.get_paginator("describe_endpoint_access")` -> [DescribeEndpointAccessPaginator](./paginators.md#describeendpointaccesspaginator)
- `client.get_paginator("describe_endpoint_authorization")` -> [DescribeEndpointAuthorizationPaginator](./paginators.md#describeendpointauthorizationpaginator)
- `client.get_paginator("describe_event_subscriptions")` -> [DescribeEventSubscriptionsPaginator](./paginators.md#describeeventsubscriptionspaginator)
- `client.get_paginator("describe_events")` -> [DescribeEventsPaginator](./paginators.md#describeeventspaginator)
- `client.get_paginator("describe_hsm_client_certificates")` -> [DescribeHsmClientCertificatesPaginator](./paginators.md#describehsmclientcertificatespaginator)
- `client.get_paginator("describe_hsm_configurations")` -> [DescribeHsmConfigurationsPaginator](./paginators.md#describehsmconfigurationspaginator)
- `client.get_paginator("describe_inbound_integrations")` -> [DescribeInboundIntegrationsPaginator](./paginators.md#describeinboundintegrationspaginator)
- `client.get_paginator("describe_integrations")` -> [DescribeIntegrationsPaginator](./paginators.md#describeintegrationspaginator)
- `client.get_paginator("describe_node_configuration_options")` -> [DescribeNodeConfigurationOptionsPaginator](./paginators.md#describenodeconfigurationoptionspaginator)
- `client.get_paginator("describe_orderable_cluster_options")` -> [DescribeOrderableClusterOptionsPaginator](./paginators.md#describeorderableclusteroptionspaginator)
- `client.get_paginator("describe_redshift_idc_applications")` -> [DescribeRedshiftIdcApplicationsPaginator](./paginators.md#describeredshiftidcapplicationspaginator)
- `client.get_paginator("describe_reserved_node_exchange_status")` -> [DescribeReservedNodeExchangeStatusPaginator](./paginators.md#describereservednodeexchangestatuspaginator)
- `client.get_paginator("describe_reserved_node_offerings")` -> [DescribeReservedNodeOfferingsPaginator](./paginators.md#describereservednodeofferingspaginator)
- `client.get_paginator("describe_reserved_nodes")` -> [DescribeReservedNodesPaginator](./paginators.md#describereservednodespaginator)
- `client.get_paginator("describe_scheduled_actions")` -> [DescribeScheduledActionsPaginator](./paginators.md#describescheduledactionspaginator)
- `client.get_paginator("describe_snapshot_copy_grants")` -> [DescribeSnapshotCopyGrantsPaginator](./paginators.md#describesnapshotcopygrantspaginator)
- `client.get_paginator("describe_snapshot_schedules")` -> [DescribeSnapshotSchedulesPaginator](./paginators.md#describesnapshotschedulespaginator)
- `client.get_paginator("describe_table_restore_status")` -> [DescribeTableRestoreStatusPaginator](./paginators.md#describetablerestorestatuspaginator)
- `client.get_paginator("describe_tags")` -> [DescribeTagsPaginator](./paginators.md#describetagspaginator)
- `client.get_paginator("describe_usage_limits")` -> [DescribeUsageLimitsPaginator](./paginators.md#describeusagelimitspaginator)
- `client.get_paginator("get_reserved_node_exchange_configuration_options")` -> [GetReservedNodeExchangeConfigurationOptionsPaginator](./paginators.md#getreservednodeexchangeconfigurationoptionspaginator)
- `client.get_paginator("get_reserved_node_exchange_offerings")` -> [GetReservedNodeExchangeOfferingsPaginator](./paginators.md#getreservednodeexchangeofferingspaginator)
- `client.get_paginator("list_recommendations")` -> [ListRecommendationsPaginator](./paginators.md#listrecommendationspaginator)




### get_waiter

Type annotations and code completion for `#!python session.client("redshift").get_waiter` method with overloads.

- `client.get_waiter("cluster_available")` -> [ClusterAvailableWaiter](./waiters.md#clusteravailablewaiter)
- `client.get_waiter("cluster_deleted")` -> [ClusterDeletedWaiter](./waiters.md#clusterdeletedwaiter)
- `client.get_waiter("cluster_restored")` -> [ClusterRestoredWaiter](./waiters.md#clusterrestoredwaiter)
- `client.get_waiter("snapshot_available")` -> [SnapshotAvailableWaiter](./waiters.md#snapshotavailablewaiter)
