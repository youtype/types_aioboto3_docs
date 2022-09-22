# Paginators

> [Index](../README.md) > [Redshift](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Redshift](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
    type annotations stubs module [types-aiobotocore-redshift](https://pypi.org/project/types-aiobotocore-redshift/).

## DescribeClusterDbRevisionsPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_cluster_db_revisions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterDbRevisions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeClusterDbRevisionsPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeClusterDbRevisionsPaginator = client.get_paginator("describe_cluster_db_revisions")  # (2)
    async for item in paginator.paginate(...):
        item: ClusterDbRevisionsMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeClusterDbRevisionsPaginator](./paginators.md#describeclusterdbrevisionspaginator)
3. item: [:material-code-braces: ClusterDbRevisionsMessageTypeDef](./type_defs.md#clusterdbrevisionsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClusterDbRevisionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ClusterIdentifier: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ClusterDbRevisionsMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ClusterDbRevisionsMessageTypeDef](./type_defs.md#clusterdbrevisionsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef](./type_defs.md#describeclusterdbrevisionsmessagedescribeclusterdbrevisionspaginatetypedef) 
## DescribeClusterParameterGroupsPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_cluster_parameter_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterParameterGroups)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeClusterParameterGroupsPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeClusterParameterGroupsPaginator = client.get_paginator("describe_cluster_parameter_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ClusterParameterGroupsMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeClusterParameterGroupsPaginator](./paginators.md#describeclusterparametergroupspaginator)
3. item: [:material-code-braces: ClusterParameterGroupsMessageTypeDef](./type_defs.md#clusterparametergroupsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClusterParameterGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ParameterGroupName: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ClusterParameterGroupsMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ClusterParameterGroupsMessageTypeDef](./type_defs.md#clusterparametergroupsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef = {  # (1)
    "ParameterGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef](./type_defs.md#describeclusterparametergroupsmessagedescribeclusterparametergroupspaginatetypedef) 
## DescribeClusterParametersPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_cluster_parameters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterParameters)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeClusterParametersPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeClusterParametersPaginator = client.get_paginator("describe_cluster_parameters")  # (2)
    async for item in paginator.paginate(...):
        item: ClusterParameterGroupDetailsTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeClusterParametersPaginator](./paginators.md#describeclusterparameterspaginator)
3. item: [:material-code-braces: ClusterParameterGroupDetailsTypeDef](./type_defs.md#clusterparametergroupdetailstypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClusterParametersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ParameterGroupName: str,
    Source: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ClusterParameterGroupDetailsTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ClusterParameterGroupDetailsTypeDef](./type_defs.md#clusterparametergroupdetailstypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = {  # (1)
    "ParameterGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef](./type_defs.md#describeclusterparametersmessagedescribeclusterparameterspaginatetypedef) 
## DescribeClusterSecurityGroupsPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_cluster_security_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSecurityGroups)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeClusterSecurityGroupsPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeClusterSecurityGroupsPaginator = client.get_paginator("describe_cluster_security_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ClusterSecurityGroupMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeClusterSecurityGroupsPaginator](./paginators.md#describeclustersecuritygroupspaginator)
3. item: [:material-code-braces: ClusterSecurityGroupMessageTypeDef](./type_defs.md#clustersecuritygroupmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClusterSecurityGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ClusterSecurityGroupName: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ClusterSecurityGroupMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ClusterSecurityGroupMessageTypeDef](./type_defs.md#clustersecuritygroupmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef = {  # (1)
    "ClusterSecurityGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef](./type_defs.md#describeclustersecuritygroupsmessagedescribeclustersecuritygroupspaginatetypedef) 
## DescribeClusterSnapshotsPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_cluster_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSnapshots)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeClusterSnapshotsPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeClusterSnapshotsPaginator = client.get_paginator("describe_cluster_snapshots")  # (2)
    async for item in paginator.paginate(...):
        item: SnapshotMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeClusterSnapshotsPaginator](./paginators.md#describeclustersnapshotspaginator)
3. item: [:material-code-braces: SnapshotMessageTypeDef](./type_defs.md#snapshotmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClusterSnapshotsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ClusterIdentifier: str = ...,
    SnapshotIdentifier: str = ...,
    SnapshotArn: str = ...,
    SnapshotType: str = ...,
    StartTime: Union[datetime, str] = ...,
    EndTime: Union[datetime, str] = ...,
    OwnerAccount: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    ClusterExists: bool = ...,
    SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[SnapshotMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SnapshotSortingEntityTypeDef](./type_defs.md#snapshotsortingentitytypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SnapshotMessageTypeDef](./type_defs.md#snapshotmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef](./type_defs.md#describeclustersnapshotsmessagedescribeclustersnapshotspaginatetypedef) 
## DescribeClusterSubnetGroupsPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_cluster_subnet_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSubnetGroups)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeClusterSubnetGroupsPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeClusterSubnetGroupsPaginator = client.get_paginator("describe_cluster_subnet_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ClusterSubnetGroupMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeClusterSubnetGroupsPaginator](./paginators.md#describeclustersubnetgroupspaginator)
3. item: [:material-code-braces: ClusterSubnetGroupMessageTypeDef](./type_defs.md#clustersubnetgroupmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClusterSubnetGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ClusterSubnetGroupName: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ClusterSubnetGroupMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ClusterSubnetGroupMessageTypeDef](./type_defs.md#clustersubnetgroupmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef = {  # (1)
    "ClusterSubnetGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef](./type_defs.md#describeclustersubnetgroupsmessagedescribeclustersubnetgroupspaginatetypedef) 
## DescribeClusterTracksPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_cluster_tracks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterTracks)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeClusterTracksPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeClusterTracksPaginator = client.get_paginator("describe_cluster_tracks")  # (2)
    async for item in paginator.paginate(...):
        item: TrackListMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeClusterTracksPaginator](./paginators.md#describeclustertrackspaginator)
3. item: [:material-code-braces: TrackListMessageTypeDef](./type_defs.md#tracklistmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClusterTracksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    MaintenanceTrackName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[TrackListMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: TrackListMessageTypeDef](./type_defs.md#tracklistmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef = {  # (1)
    "MaintenanceTrackName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef](./type_defs.md#describeclustertracksmessagedescribeclustertrackspaginatetypedef) 
## DescribeClusterVersionsPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_cluster_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterVersions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeClusterVersionsPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeClusterVersionsPaginator = client.get_paginator("describe_cluster_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ClusterVersionsMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeClusterVersionsPaginator](./paginators.md#describeclusterversionspaginator)
3. item: [:material-code-braces: ClusterVersionsMessageTypeDef](./type_defs.md#clusterversionsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClusterVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ClusterVersion: str = ...,
    ClusterParameterGroupFamily: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ClusterVersionsMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ClusterVersionsMessageTypeDef](./type_defs.md#clusterversionsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef = {  # (1)
    "ClusterVersion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef](./type_defs.md#describeclusterversionsmessagedescribeclusterversionspaginatetypedef) 
## DescribeClustersPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusters)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeClustersPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeClustersPaginator = client.get_paginator("describe_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: ClustersMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeClustersPaginator](./paginators.md#describeclusterspaginator)
3. item: [:material-code-braces: ClustersMessageTypeDef](./type_defs.md#clustersmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClustersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ClusterIdentifier: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ClustersMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ClustersMessageTypeDef](./type_defs.md#clustersmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeClustersMessageDescribeClustersPaginateTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClustersMessageDescribeClustersPaginateTypeDef](./type_defs.md#describeclustersmessagedescribeclusterspaginatetypedef) 
## DescribeDataSharesPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_data_shares")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataShares)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeDataSharesPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeDataSharesPaginator = client.get_paginator("describe_data_shares")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDataSharesResultTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeDataSharesPaginator](./paginators.md#describedatasharespaginator)
3. item: [:material-code-braces: DescribeDataSharesResultTypeDef](./type_defs.md#describedatasharesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDataSharesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DataShareArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeDataSharesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeDataSharesResultTypeDef](./type_defs.md#describedatasharesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef = {  # (1)
    "DataShareArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef](./type_defs.md#describedatasharesmessagedescribedatasharespaginatetypedef) 
## DescribeDataSharesForConsumerPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_data_shares_for_consumer")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataSharesForConsumer)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeDataSharesForConsumerPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeDataSharesForConsumerPaginator = client.get_paginator("describe_data_shares_for_consumer")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDataSharesForConsumerResultTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeDataSharesForConsumerPaginator](./paginators.md#describedatasharesforconsumerpaginator)
3. item: [:material-code-braces: DescribeDataSharesForConsumerResultTypeDef](./type_defs.md#describedatasharesforconsumerresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDataSharesForConsumerPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ConsumerArn: str = ...,
    Status: DataShareStatusForConsumerType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeDataSharesForConsumerResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DataShareStatusForConsumerType](./literals.md#datasharestatusforconsumertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeDataSharesForConsumerResultTypeDef](./type_defs.md#describedatasharesforconsumerresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef = {  # (1)
    "ConsumerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef](./type_defs.md#describedatasharesforconsumermessagedescribedatasharesforconsumerpaginatetypedef) 
## DescribeDataSharesForProducerPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_data_shares_for_producer")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataSharesForProducer)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeDataSharesForProducerPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeDataSharesForProducerPaginator = client.get_paginator("describe_data_shares_for_producer")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDataSharesForProducerResultTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeDataSharesForProducerPaginator](./paginators.md#describedatasharesforproducerpaginator)
3. item: [:material-code-braces: DescribeDataSharesForProducerResultTypeDef](./type_defs.md#describedatasharesforproducerresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDataSharesForProducerPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ProducerArn: str = ...,
    Status: DataShareStatusForProducerType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeDataSharesForProducerResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DataShareStatusForProducerType](./literals.md#datasharestatusforproducertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeDataSharesForProducerResultTypeDef](./type_defs.md#describedatasharesforproducerresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef = {  # (1)
    "ProducerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef](./type_defs.md#describedatasharesforproducermessagedescribedatasharesforproducerpaginatetypedef) 
## DescribeDefaultClusterParametersPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_default_cluster_parameters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDefaultClusterParameters)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeDefaultClusterParametersPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeDefaultClusterParametersPaginator = client.get_paginator("describe_default_cluster_parameters")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDefaultClusterParametersResultTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeDefaultClusterParametersPaginator](./paginators.md#describedefaultclusterparameterspaginator)
3. item: [:material-code-braces: DescribeDefaultClusterParametersResultTypeDef](./type_defs.md#describedefaultclusterparametersresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDefaultClusterParametersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ParameterGroupFamily: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeDefaultClusterParametersResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeDefaultClusterParametersResultTypeDef](./type_defs.md#describedefaultclusterparametersresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = {  # (1)
    "ParameterGroupFamily": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef](./type_defs.md#describedefaultclusterparametersmessagedescribedefaultclusterparameterspaginatetypedef) 
## DescribeEndpointAccessPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_endpoint_access")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEndpointAccess)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeEndpointAccessPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeEndpointAccessPaginator = client.get_paginator("describe_endpoint_access")  # (2)
    async for item in paginator.paginate(...):
        item: EndpointAccessListTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeEndpointAccessPaginator](./paginators.md#describeendpointaccesspaginator)
3. item: [:material-code-braces: EndpointAccessListTypeDef](./type_defs.md#endpointaccesslisttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEndpointAccessPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ClusterIdentifier: str = ...,
    ResourceOwner: str = ...,
    EndpointName: str = ...,
    VpcId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[EndpointAccessListTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: EndpointAccessListTypeDef](./type_defs.md#endpointaccesslisttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef](./type_defs.md#describeendpointaccessmessagedescribeendpointaccesspaginatetypedef) 
## DescribeEndpointAuthorizationPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_endpoint_authorization")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEndpointAuthorization)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeEndpointAuthorizationPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeEndpointAuthorizationPaginator = client.get_paginator("describe_endpoint_authorization")  # (2)
    async for item in paginator.paginate(...):
        item: EndpointAuthorizationListTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeEndpointAuthorizationPaginator](./paginators.md#describeendpointauthorizationpaginator)
3. item: [:material-code-braces: EndpointAuthorizationListTypeDef](./type_defs.md#endpointauthorizationlisttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEndpointAuthorizationPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ClusterIdentifier: str = ...,
    Account: str = ...,
    Grantee: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[EndpointAuthorizationListTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: EndpointAuthorizationListTypeDef](./type_defs.md#endpointauthorizationlisttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef](./type_defs.md#describeendpointauthorizationmessagedescribeendpointauthorizationpaginatetypedef) 
## DescribeEventSubscriptionsPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_event_subscriptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEventSubscriptions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeEventSubscriptionsPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeEventSubscriptionsPaginator = client.get_paginator("describe_event_subscriptions")  # (2)
    async for item in paginator.paginate(...):
        item: EventSubscriptionsMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeEventSubscriptionsPaginator](./paginators.md#describeeventsubscriptionspaginator)
3. item: [:material-code-braces: EventSubscriptionsMessageTypeDef](./type_defs.md#eventsubscriptionsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEventSubscriptionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    SubscriptionName: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[EventSubscriptionsMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: EventSubscriptionsMessageTypeDef](./type_defs.md#eventsubscriptionsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = {  # (1)
    "SubscriptionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef](./type_defs.md#describeeventsubscriptionsmessagedescribeeventsubscriptionspaginatetypedef) 
## DescribeEventsPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEvents)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeEventsPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeEventsPaginator = client.get_paginator("describe_events")  # (2)
    async for item in paginator.paginate(...):
        item: EventsMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeEventsPaginator](./paginators.md#describeeventspaginator)
3. item: [:material-code-braces: EventsMessageTypeDef](./type_defs.md#eventsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEventsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    SourceIdentifier: str = ...,
    SourceType: SourceTypeType = ...,  # (1)
    StartTime: Union[datetime, str] = ...,
    EndTime: Union[datetime, str] = ...,
    Duration: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[EventsMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: EventsMessageTypeDef](./type_defs.md#eventsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEventsMessageDescribeEventsPaginateTypeDef = {  # (1)
    "SourceIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventsMessageDescribeEventsPaginateTypeDef](./type_defs.md#describeeventsmessagedescribeeventspaginatetypedef) 
## DescribeHsmClientCertificatesPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_hsm_client_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeHsmClientCertificates)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeHsmClientCertificatesPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeHsmClientCertificatesPaginator = client.get_paginator("describe_hsm_client_certificates")  # (2)
    async for item in paginator.paginate(...):
        item: HsmClientCertificateMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeHsmClientCertificatesPaginator](./paginators.md#describehsmclientcertificatespaginator)
3. item: [:material-code-braces: HsmClientCertificateMessageTypeDef](./type_defs.md#hsmclientcertificatemessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeHsmClientCertificatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    HsmClientCertificateIdentifier: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[HsmClientCertificateMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: HsmClientCertificateMessageTypeDef](./type_defs.md#hsmclientcertificatemessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef = {  # (1)
    "HsmClientCertificateIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef](./type_defs.md#describehsmclientcertificatesmessagedescribehsmclientcertificatespaginatetypedef) 
## DescribeHsmConfigurationsPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_hsm_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeHsmConfigurations)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeHsmConfigurationsPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeHsmConfigurationsPaginator = client.get_paginator("describe_hsm_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: HsmConfigurationMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeHsmConfigurationsPaginator](./paginators.md#describehsmconfigurationspaginator)
3. item: [:material-code-braces: HsmConfigurationMessageTypeDef](./type_defs.md#hsmconfigurationmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeHsmConfigurationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    HsmConfigurationIdentifier: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[HsmConfigurationMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: HsmConfigurationMessageTypeDef](./type_defs.md#hsmconfigurationmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef = {  # (1)
    "HsmConfigurationIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef](./type_defs.md#describehsmconfigurationsmessagedescribehsmconfigurationspaginatetypedef) 
## DescribeNodeConfigurationOptionsPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_node_configuration_options")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeNodeConfigurationOptions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeNodeConfigurationOptionsPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeNodeConfigurationOptionsPaginator = client.get_paginator("describe_node_configuration_options")  # (2)
    async for item in paginator.paginate(...):
        item: NodeConfigurationOptionsMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeNodeConfigurationOptionsPaginator](./paginators.md#describenodeconfigurationoptionspaginator)
3. item: [:material-code-braces: NodeConfigurationOptionsMessageTypeDef](./type_defs.md#nodeconfigurationoptionsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeNodeConfigurationOptionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ActionType: ActionTypeType,  # (1)
    ClusterIdentifier: str = ...,
    SnapshotIdentifier: str = ...,
    SnapshotArn: str = ...,
    OwnerAccount: str = ...,
    Filters: Sequence[NodeConfigurationOptionsFilterTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[NodeConfigurationOptionsMessageTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
2. See [:material-code-braces: NodeConfigurationOptionsFilterTypeDef](./type_defs.md#nodeconfigurationoptionsfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: NodeConfigurationOptionsMessageTypeDef](./type_defs.md#nodeconfigurationoptionsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef = {  # (1)
    "ActionType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef](./type_defs.md#describenodeconfigurationoptionsmessagedescribenodeconfigurationoptionspaginatetypedef) 
## DescribeOrderableClusterOptionsPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_orderable_cluster_options")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeOrderableClusterOptions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeOrderableClusterOptionsPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeOrderableClusterOptionsPaginator = client.get_paginator("describe_orderable_cluster_options")  # (2)
    async for item in paginator.paginate(...):
        item: OrderableClusterOptionsMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeOrderableClusterOptionsPaginator](./paginators.md#describeorderableclusteroptionspaginator)
3. item: [:material-code-braces: OrderableClusterOptionsMessageTypeDef](./type_defs.md#orderableclusteroptionsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeOrderableClusterOptionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ClusterVersion: str = ...,
    NodeType: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[OrderableClusterOptionsMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: OrderableClusterOptionsMessageTypeDef](./type_defs.md#orderableclusteroptionsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef = {  # (1)
    "ClusterVersion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef](./type_defs.md#describeorderableclusteroptionsmessagedescribeorderableclusteroptionspaginatetypedef) 
## DescribeReservedNodeExchangeStatusPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_reserved_node_exchange_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodeExchangeStatus)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeReservedNodeExchangeStatusPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeReservedNodeExchangeStatusPaginator = client.get_paginator("describe_reserved_node_exchange_status")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeReservedNodeExchangeStatusOutputMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeReservedNodeExchangeStatusPaginator](./paginators.md#describereservednodeexchangestatuspaginator)
3. item: [:material-code-braces: DescribeReservedNodeExchangeStatusOutputMessageTypeDef](./type_defs.md#describereservednodeexchangestatusoutputmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReservedNodeExchangeStatusPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ReservedNodeId: str = ...,
    ReservedNodeExchangeRequestId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeReservedNodeExchangeStatusOutputMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeReservedNodeExchangeStatusOutputMessageTypeDef](./type_defs.md#describereservednodeexchangestatusoutputmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef = {  # (1)
    "ReservedNodeId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef](./type_defs.md#describereservednodeexchangestatusinputmessagedescribereservednodeexchangestatuspaginatetypedef) 
## DescribeReservedNodeOfferingsPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_reserved_node_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodeOfferings)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeReservedNodeOfferingsPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeReservedNodeOfferingsPaginator = client.get_paginator("describe_reserved_node_offerings")  # (2)
    async for item in paginator.paginate(...):
        item: ReservedNodeOfferingsMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeReservedNodeOfferingsPaginator](./paginators.md#describereservednodeofferingspaginator)
3. item: [:material-code-braces: ReservedNodeOfferingsMessageTypeDef](./type_defs.md#reservednodeofferingsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReservedNodeOfferingsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ReservedNodeOfferingId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ReservedNodeOfferingsMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ReservedNodeOfferingsMessageTypeDef](./type_defs.md#reservednodeofferingsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef = {  # (1)
    "ReservedNodeOfferingId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef](./type_defs.md#describereservednodeofferingsmessagedescribereservednodeofferingspaginatetypedef) 
## DescribeReservedNodesPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_reserved_nodes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodes)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeReservedNodesPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeReservedNodesPaginator = client.get_paginator("describe_reserved_nodes")  # (2)
    async for item in paginator.paginate(...):
        item: ReservedNodesMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeReservedNodesPaginator](./paginators.md#describereservednodespaginator)
3. item: [:material-code-braces: ReservedNodesMessageTypeDef](./type_defs.md#reservednodesmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReservedNodesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ReservedNodeId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ReservedNodesMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ReservedNodesMessageTypeDef](./type_defs.md#reservednodesmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef = {  # (1)
    "ReservedNodeId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef](./type_defs.md#describereservednodesmessagedescribereservednodespaginatetypedef) 
## DescribeScheduledActionsPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_scheduled_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeScheduledActions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeScheduledActionsPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeScheduledActionsPaginator = client.get_paginator("describe_scheduled_actions")  # (2)
    async for item in paginator.paginate(...):
        item: ScheduledActionsMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeScheduledActionsPaginator](./paginators.md#describescheduledactionspaginator)
3. item: [:material-code-braces: ScheduledActionsMessageTypeDef](./type_defs.md#scheduledactionsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeScheduledActionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ScheduledActionName: str = ...,
    TargetActionType: ScheduledActionTypeValuesType = ...,  # (1)
    StartTime: Union[datetime, str] = ...,
    EndTime: Union[datetime, str] = ...,
    Active: bool = ...,
    Filters: Sequence[ScheduledActionFilterTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ScheduledActionsMessageTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: ScheduledActionTypeValuesType](./literals.md#scheduledactiontypevaluestype) 
2. See [:material-code-braces: ScheduledActionFilterTypeDef](./type_defs.md#scheduledactionfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ScheduledActionsMessageTypeDef](./type_defs.md#scheduledactionsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef = {  # (1)
    "ScheduledActionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef](./type_defs.md#describescheduledactionsmessagedescribescheduledactionspaginatetypedef) 
## DescribeSnapshotCopyGrantsPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_snapshot_copy_grants")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeSnapshotCopyGrants)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeSnapshotCopyGrantsPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeSnapshotCopyGrantsPaginator = client.get_paginator("describe_snapshot_copy_grants")  # (2)
    async for item in paginator.paginate(...):
        item: SnapshotCopyGrantMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeSnapshotCopyGrantsPaginator](./paginators.md#describesnapshotcopygrantspaginator)
3. item: [:material-code-braces: SnapshotCopyGrantMessageTypeDef](./type_defs.md#snapshotcopygrantmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSnapshotCopyGrantsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    SnapshotCopyGrantName: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[SnapshotCopyGrantMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: SnapshotCopyGrantMessageTypeDef](./type_defs.md#snapshotcopygrantmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef = {  # (1)
    "SnapshotCopyGrantName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef](./type_defs.md#describesnapshotcopygrantsmessagedescribesnapshotcopygrantspaginatetypedef) 
## DescribeSnapshotSchedulesPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_snapshot_schedules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeSnapshotSchedules)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeSnapshotSchedulesPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeSnapshotSchedulesPaginator = client.get_paginator("describe_snapshot_schedules")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSnapshotSchedulesOutputMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeSnapshotSchedulesPaginator](./paginators.md#describesnapshotschedulespaginator)
3. item: [:material-code-braces: DescribeSnapshotSchedulesOutputMessageTypeDef](./type_defs.md#describesnapshotschedulesoutputmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSnapshotSchedulesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ClusterIdentifier: str = ...,
    ScheduleIdentifier: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeSnapshotSchedulesOutputMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeSnapshotSchedulesOutputMessageTypeDef](./type_defs.md#describesnapshotschedulesoutputmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef](./type_defs.md#describesnapshotschedulesmessagedescribesnapshotschedulespaginatetypedef) 
## DescribeTableRestoreStatusPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_table_restore_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeTableRestoreStatus)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeTableRestoreStatusPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeTableRestoreStatusPaginator = client.get_paginator("describe_table_restore_status")  # (2)
    async for item in paginator.paginate(...):
        item: TableRestoreStatusMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeTableRestoreStatusPaginator](./paginators.md#describetablerestorestatuspaginator)
3. item: [:material-code-braces: TableRestoreStatusMessageTypeDef](./type_defs.md#tablerestorestatusmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTableRestoreStatusPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ClusterIdentifier: str = ...,
    TableRestoreRequestId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[TableRestoreStatusMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: TableRestoreStatusMessageTypeDef](./type_defs.md#tablerestorestatusmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef = {  # (1)
    "ClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef](./type_defs.md#describetablerestorestatusmessagedescribetablerestorestatuspaginatetypedef) 
## DescribeTagsPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeTags)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeTagsPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")  # (2)
    async for item in paginator.paginate(...):
        item: TaggedResourceListMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeTagsPaginator](./paginators.md#describetagspaginator)
3. item: [:material-code-braces: TaggedResourceListMessageTypeDef](./type_defs.md#taggedresourcelistmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTagsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceName: str = ...,
    ResourceType: str = ...,
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[TaggedResourceListMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: TaggedResourceListMessageTypeDef](./type_defs.md#taggedresourcelistmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTagsMessageDescribeTagsPaginateTypeDef = {  # (1)
    "ResourceName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTagsMessageDescribeTagsPaginateTypeDef](./type_defs.md#describetagsmessagedescribetagspaginatetypedef) 
## DescribeUsageLimitsPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("describe_usage_limits")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeUsageLimits)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import DescribeUsageLimitsPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: DescribeUsageLimitsPaginator = client.get_paginator("describe_usage_limits")  # (2)
    async for item in paginator.paginate(...):
        item: UsageLimitListTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeUsageLimitsPaginator](./paginators.md#describeusagelimitspaginator)
3. item: [:material-code-braces: UsageLimitListTypeDef](./type_defs.md#usagelimitlisttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeUsageLimitsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    UsageLimitId: str = ...,
    ClusterIdentifier: str = ...,
    FeatureType: UsageLimitFeatureTypeType = ...,  # (1)
    TagKeys: Sequence[str] = ...,
    TagValues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[UsageLimitListTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: UsageLimitFeatureTypeType](./literals.md#usagelimitfeaturetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: UsageLimitListTypeDef](./type_defs.md#usagelimitlisttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef = {  # (1)
    "UsageLimitId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef](./type_defs.md#describeusagelimitsmessagedescribeusagelimitspaginatetypedef) 
## GetReservedNodeExchangeConfigurationOptionsPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("get_reserved_node_exchange_configuration_options")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.GetReservedNodeExchangeConfigurationOptions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import GetReservedNodeExchangeConfigurationOptionsPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: GetReservedNodeExchangeConfigurationOptionsPaginator = client.get_paginator("get_reserved_node_exchange_configuration_options")  # (2)
    async for item in paginator.paginate(...):
        item: GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [GetReservedNodeExchangeConfigurationOptionsPaginator](./paginators.md#getreservednodeexchangeconfigurationoptionspaginator)
3. item: [:material-code-braces: GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef](./type_defs.md#getreservednodeexchangeconfigurationoptionsoutputmessagetypedef) 


### paginate

Type annotations and code completion for `#!python GetReservedNodeExchangeConfigurationOptionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ActionType: ReservedNodeExchangeActionTypeType,  # (1)
    ClusterIdentifier: str = ...,
    SnapshotIdentifier: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ReservedNodeExchangeActionTypeType](./literals.md#reservednodeexchangeactiontypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef](./type_defs.md#getreservednodeexchangeconfigurationoptionsoutputmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = {  # (1)
    "ActionType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef](./type_defs.md#getreservednodeexchangeconfigurationoptionsinputmessagegetreservednodeexchangeconfigurationoptionspaginatetypedef) 
## GetReservedNodeExchangeOfferingsPaginator

Type annotations and code completion for `#!python session.client("redshift").get_paginator("get_reserved_node_exchange_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.GetReservedNodeExchangeOfferings)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift.paginator import GetReservedNodeExchangeOfferingsPaginator

session = Session()

session = get_session()
async with session.client("redshift") as client:  # (1)
    paginator: GetReservedNodeExchangeOfferingsPaginator = client.get_paginator("get_reserved_node_exchange_offerings")  # (2)
    async for item in paginator.paginate(...):
        item: GetReservedNodeExchangeOfferingsOutputMessageTypeDef
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [GetReservedNodeExchangeOfferingsPaginator](./paginators.md#getreservednodeexchangeofferingspaginator)
3. item: [:material-code-braces: GetReservedNodeExchangeOfferingsOutputMessageTypeDef](./type_defs.md#getreservednodeexchangeofferingsoutputmessagetypedef) 


### paginate

Type annotations and code completion for `#!python GetReservedNodeExchangeOfferingsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ReservedNodeId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetReservedNodeExchangeOfferingsOutputMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetReservedNodeExchangeOfferingsOutputMessageTypeDef](./type_defs.md#getreservednodeexchangeofferingsoutputmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = {  # (1)
    "ReservedNodeId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef](./type_defs.md#getreservednodeexchangeofferingsinputmessagegetreservednodeexchangeofferingspaginatetypedef) 
