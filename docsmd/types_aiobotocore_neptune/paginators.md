# Paginators

> [Index](../README.md) > [Neptune](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Neptune](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
    type annotations stubs module [types-aiobotocore-neptune](https://pypi.org/project/types-aiobotocore-neptune/).

## DescribeDBClusterEndpointsPaginator

Type annotations and code completion for `#!python session.client("neptune").get_paginator("describe_db_cluster_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterEndpoints)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_neptune.paginator import DescribeDBClusterEndpointsPaginator

session = Session()

session = get_session()
async with session.client("neptune") as client:  # (1)
    paginator: DescribeDBClusterEndpointsPaginator = client.get_paginator("describe_db_cluster_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: DBClusterEndpointMessageTypeDef
        print(item)  # (3)
```

1. client: [NeptuneClient](./client.md)
2. paginator: [DescribeDBClusterEndpointsPaginator](./paginators.md#describedbclusterendpointspaginator)
3. item: [:material-code-braces: DBClusterEndpointMessageTypeDef](./type_defs.md#dbclusterendpointmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBClusterEndpointsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DBClusterIdentifier: str = ...,
    DBClusterEndpointIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DBClusterEndpointMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBClusterEndpointMessageTypeDef](./type_defs.md#dbclusterendpointmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef = {  # (1)
    "DBClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef](./type_defs.md#describedbclusterendpointsmessagedescribedbclusterendpointspaginatetypedef) 
## DescribeDBClusterParameterGroupsPaginator

Type annotations and code completion for `#!python session.client("neptune").get_paginator("describe_db_cluster_parameter_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterParameterGroups)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_neptune.paginator import DescribeDBClusterParameterGroupsPaginator

session = Session()

session = get_session()
async with session.client("neptune") as client:  # (1)
    paginator: DescribeDBClusterParameterGroupsPaginator = client.get_paginator("describe_db_cluster_parameter_groups")  # (2)
    async for item in paginator.paginate(...):
        item: DBClusterParameterGroupsMessageTypeDef
        print(item)  # (3)
```

1. client: [NeptuneClient](./client.md)
2. paginator: [DescribeDBClusterParameterGroupsPaginator](./paginators.md#describedbclusterparametergroupspaginator)
3. item: [:material-code-braces: DBClusterParameterGroupsMessageTypeDef](./type_defs.md#dbclusterparametergroupsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBClusterParameterGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DBClusterParameterGroupName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DBClusterParameterGroupsMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBClusterParameterGroupsMessageTypeDef](./type_defs.md#dbclusterparametergroupsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef = {  # (1)
    "DBClusterParameterGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef](./type_defs.md#describedbclusterparametergroupsmessagedescribedbclusterparametergroupspaginatetypedef) 
## DescribeDBClusterParametersPaginator

Type annotations and code completion for `#!python session.client("neptune").get_paginator("describe_db_cluster_parameters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterParameters)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_neptune.paginator import DescribeDBClusterParametersPaginator

session = Session()

session = get_session()
async with session.client("neptune") as client:  # (1)
    paginator: DescribeDBClusterParametersPaginator = client.get_paginator("describe_db_cluster_parameters")  # (2)
    async for item in paginator.paginate(...):
        item: DBClusterParameterGroupDetailsTypeDef
        print(item)  # (3)
```

1. client: [NeptuneClient](./client.md)
2. paginator: [DescribeDBClusterParametersPaginator](./paginators.md#describedbclusterparameterspaginator)
3. item: [:material-code-braces: DBClusterParameterGroupDetailsTypeDef](./type_defs.md#dbclusterparametergroupdetailstypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBClusterParametersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DBClusterParameterGroupName: str,
    Source: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DBClusterParameterGroupDetailsTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBClusterParameterGroupDetailsTypeDef](./type_defs.md#dbclusterparametergroupdetailstypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = {  # (1)
    "DBClusterParameterGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef](./type_defs.md#describedbclusterparametersmessagedescribedbclusterparameterspaginatetypedef) 
## DescribeDBClusterSnapshotsPaginator

Type annotations and code completion for `#!python session.client("neptune").get_paginator("describe_db_cluster_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterSnapshots)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_neptune.paginator import DescribeDBClusterSnapshotsPaginator

session = Session()

session = get_session()
async with session.client("neptune") as client:  # (1)
    paginator: DescribeDBClusterSnapshotsPaginator = client.get_paginator("describe_db_cluster_snapshots")  # (2)
    async for item in paginator.paginate(...):
        item: DBClusterSnapshotMessageTypeDef
        print(item)  # (3)
```

1. client: [NeptuneClient](./client.md)
2. paginator: [DescribeDBClusterSnapshotsPaginator](./paginators.md#describedbclustersnapshotspaginator)
3. item: [:material-code-braces: DBClusterSnapshotMessageTypeDef](./type_defs.md#dbclustersnapshotmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBClusterSnapshotsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DBClusterIdentifier: str = ...,
    DBClusterSnapshotIdentifier: str = ...,
    SnapshotType: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    IncludeShared: bool = ...,
    IncludePublic: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DBClusterSnapshotMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBClusterSnapshotMessageTypeDef](./type_defs.md#dbclustersnapshotmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef = {  # (1)
    "DBClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef](./type_defs.md#describedbclustersnapshotsmessagedescribedbclustersnapshotspaginatetypedef) 
## DescribeDBClustersPaginator

Type annotations and code completion for `#!python session.client("neptune").get_paginator("describe_db_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusters)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_neptune.paginator import DescribeDBClustersPaginator

session = Session()

session = get_session()
async with session.client("neptune") as client:  # (1)
    paginator: DescribeDBClustersPaginator = client.get_paginator("describe_db_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: DBClusterMessageTypeDef
        print(item)  # (3)
```

1. client: [NeptuneClient](./client.md)
2. paginator: [DescribeDBClustersPaginator](./paginators.md#describedbclusterspaginator)
3. item: [:material-code-braces: DBClusterMessageTypeDef](./type_defs.md#dbclustermessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBClustersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DBClusterIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DBClusterMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBClusterMessageTypeDef](./type_defs.md#dbclustermessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef = {  # (1)
    "DBClusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef](./type_defs.md#describedbclustersmessagedescribedbclusterspaginatetypedef) 
## DescribeDBEngineVersionsPaginator

Type annotations and code completion for `#!python session.client("neptune").get_paginator("describe_db_engine_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBEngineVersions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_neptune.paginator import DescribeDBEngineVersionsPaginator

session = Session()

session = get_session()
async with session.client("neptune") as client:  # (1)
    paginator: DescribeDBEngineVersionsPaginator = client.get_paginator("describe_db_engine_versions")  # (2)
    async for item in paginator.paginate(...):
        item: DBEngineVersionMessageTypeDef
        print(item)  # (3)
```

1. client: [NeptuneClient](./client.md)
2. paginator: [DescribeDBEngineVersionsPaginator](./paginators.md#describedbengineversionspaginator)
3. item: [:material-code-braces: DBEngineVersionMessageTypeDef](./type_defs.md#dbengineversionmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBEngineVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Engine: str = ...,
    EngineVersion: str = ...,
    DBParameterGroupFamily: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DefaultOnly: bool = ...,
    ListSupportedCharacterSets: bool = ...,
    ListSupportedTimezones: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DBEngineVersionMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBEngineVersionMessageTypeDef](./type_defs.md#dbengineversionmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef = {  # (1)
    "Engine": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef](./type_defs.md#describedbengineversionsmessagedescribedbengineversionspaginatetypedef) 
## DescribeDBInstancesPaginator

Type annotations and code completion for `#!python session.client("neptune").get_paginator("describe_db_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBInstances)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_neptune.paginator import DescribeDBInstancesPaginator

session = Session()

session = get_session()
async with session.client("neptune") as client:  # (1)
    paginator: DescribeDBInstancesPaginator = client.get_paginator("describe_db_instances")  # (2)
    async for item in paginator.paginate(...):
        item: DBInstanceMessageTypeDef
        print(item)  # (3)
```

1. client: [NeptuneClient](./client.md)
2. paginator: [DescribeDBInstancesPaginator](./paginators.md#describedbinstancespaginator)
3. item: [:material-code-braces: DBInstanceMessageTypeDef](./type_defs.md#dbinstancemessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBInstancesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DBInstanceIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DBInstanceMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBInstanceMessageTypeDef](./type_defs.md#dbinstancemessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef = {  # (1)
    "DBInstanceIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef](./type_defs.md#describedbinstancesmessagedescribedbinstancespaginatetypedef) 
## DescribeDBParameterGroupsPaginator

Type annotations and code completion for `#!python session.client("neptune").get_paginator("describe_db_parameter_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBParameterGroups)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_neptune.paginator import DescribeDBParameterGroupsPaginator

session = Session()

session = get_session()
async with session.client("neptune") as client:  # (1)
    paginator: DescribeDBParameterGroupsPaginator = client.get_paginator("describe_db_parameter_groups")  # (2)
    async for item in paginator.paginate(...):
        item: DBParameterGroupsMessageTypeDef
        print(item)  # (3)
```

1. client: [NeptuneClient](./client.md)
2. paginator: [DescribeDBParameterGroupsPaginator](./paginators.md#describedbparametergroupspaginator)
3. item: [:material-code-braces: DBParameterGroupsMessageTypeDef](./type_defs.md#dbparametergroupsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBParameterGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DBParameterGroupName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DBParameterGroupsMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBParameterGroupsMessageTypeDef](./type_defs.md#dbparametergroupsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef = {  # (1)
    "DBParameterGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef](./type_defs.md#describedbparametergroupsmessagedescribedbparametergroupspaginatetypedef) 
## DescribeDBParametersPaginator

Type annotations and code completion for `#!python session.client("neptune").get_paginator("describe_db_parameters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBParameters)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_neptune.paginator import DescribeDBParametersPaginator

session = Session()

session = get_session()
async with session.client("neptune") as client:  # (1)
    paginator: DescribeDBParametersPaginator = client.get_paginator("describe_db_parameters")  # (2)
    async for item in paginator.paginate(...):
        item: DBParameterGroupDetailsTypeDef
        print(item)  # (3)
```

1. client: [NeptuneClient](./client.md)
2. paginator: [DescribeDBParametersPaginator](./paginators.md#describedbparameterspaginator)
3. item: [:material-code-braces: DBParameterGroupDetailsTypeDef](./type_defs.md#dbparametergroupdetailstypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBParametersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DBParameterGroupName: str,
    Source: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DBParameterGroupDetailsTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBParameterGroupDetailsTypeDef](./type_defs.md#dbparametergroupdetailstypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef = {  # (1)
    "DBParameterGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef](./type_defs.md#describedbparametersmessagedescribedbparameterspaginatetypedef) 
## DescribeDBSubnetGroupsPaginator

Type annotations and code completion for `#!python session.client("neptune").get_paginator("describe_db_subnet_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBSubnetGroups)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_neptune.paginator import DescribeDBSubnetGroupsPaginator

session = Session()

session = get_session()
async with session.client("neptune") as client:  # (1)
    paginator: DescribeDBSubnetGroupsPaginator = client.get_paginator("describe_db_subnet_groups")  # (2)
    async for item in paginator.paginate(...):
        item: DBSubnetGroupMessageTypeDef
        print(item)  # (3)
```

1. client: [NeptuneClient](./client.md)
2. paginator: [DescribeDBSubnetGroupsPaginator](./paginators.md#describedbsubnetgroupspaginator)
3. item: [:material-code-braces: DBSubnetGroupMessageTypeDef](./type_defs.md#dbsubnetgroupmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDBSubnetGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DBSubnetGroupName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DBSubnetGroupMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DBSubnetGroupMessageTypeDef](./type_defs.md#dbsubnetgroupmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef = {  # (1)
    "DBSubnetGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef](./type_defs.md#describedbsubnetgroupsmessagedescribedbsubnetgroupspaginatetypedef) 
## DescribeEngineDefaultParametersPaginator

Type annotations and code completion for `#!python session.client("neptune").get_paginator("describe_engine_default_parameters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEngineDefaultParameters)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_neptune.paginator import DescribeEngineDefaultParametersPaginator

session = Session()

session = get_session()
async with session.client("neptune") as client:  # (1)
    paginator: DescribeEngineDefaultParametersPaginator = client.get_paginator("describe_engine_default_parameters")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEngineDefaultParametersResultTypeDef
        print(item)  # (3)
```

1. client: [NeptuneClient](./client.md)
2. paginator: [DescribeEngineDefaultParametersPaginator](./paginators.md#describeenginedefaultparameterspaginator)
3. item: [:material-code-braces: DescribeEngineDefaultParametersResultTypeDef](./type_defs.md#describeenginedefaultparametersresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEngineDefaultParametersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DBParameterGroupFamily: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeEngineDefaultParametersResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeEngineDefaultParametersResultTypeDef](./type_defs.md#describeenginedefaultparametersresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = {  # (1)
    "DBParameterGroupFamily": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef](./type_defs.md#describeenginedefaultparametersmessagedescribeenginedefaultparameterspaginatetypedef) 
## DescribeEventSubscriptionsPaginator

Type annotations and code completion for `#!python session.client("neptune").get_paginator("describe_event_subscriptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEventSubscriptions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_neptune.paginator import DescribeEventSubscriptionsPaginator

session = Session()

session = get_session()
async with session.client("neptune") as client:  # (1)
    paginator: DescribeEventSubscriptionsPaginator = client.get_paginator("describe_event_subscriptions")  # (2)
    async for item in paginator.paginate(...):
        item: EventSubscriptionsMessageTypeDef
        print(item)  # (3)
```

1. client: [NeptuneClient](./client.md)
2. paginator: [DescribeEventSubscriptionsPaginator](./paginators.md#describeeventsubscriptionspaginator)
3. item: [:material-code-braces: EventSubscriptionsMessageTypeDef](./type_defs.md#eventsubscriptionsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEventSubscriptionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    SubscriptionName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[EventSubscriptionsMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: EventSubscriptionsMessageTypeDef](./type_defs.md#eventsubscriptionsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = {  # (1)
    "SubscriptionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef](./type_defs.md#describeeventsubscriptionsmessagedescribeeventsubscriptionspaginatetypedef) 
## DescribeEventsPaginator

Type annotations and code completion for `#!python session.client("neptune").get_paginator("describe_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEvents)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_neptune.paginator import DescribeEventsPaginator

session = Session()

session = get_session()
async with session.client("neptune") as client:  # (1)
    paginator: DescribeEventsPaginator = client.get_paginator("describe_events")  # (2)
    async for item in paginator.paginate(...):
        item: EventsMessageTypeDef
        print(item)  # (3)
```

1. client: [NeptuneClient](./client.md)
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
    EventCategories: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[EventsMessageTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: EventsMessageTypeDef](./type_defs.md#eventsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEventsMessageDescribeEventsPaginateTypeDef = {  # (1)
    "SourceIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventsMessageDescribeEventsPaginateTypeDef](./type_defs.md#describeeventsmessagedescribeeventspaginatetypedef) 
## DescribeOrderableDBInstanceOptionsPaginator

Type annotations and code completion for `#!python session.client("neptune").get_paginator("describe_orderable_db_instance_options")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeOrderableDBInstanceOptions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_neptune.paginator import DescribeOrderableDBInstanceOptionsPaginator

session = Session()

session = get_session()
async with session.client("neptune") as client:  # (1)
    paginator: DescribeOrderableDBInstanceOptionsPaginator = client.get_paginator("describe_orderable_db_instance_options")  # (2)
    async for item in paginator.paginate(...):
        item: OrderableDBInstanceOptionsMessageTypeDef
        print(item)  # (3)
```

1. client: [NeptuneClient](./client.md)
2. paginator: [DescribeOrderableDBInstanceOptionsPaginator](./paginators.md#describeorderabledbinstanceoptionspaginator)
3. item: [:material-code-braces: OrderableDBInstanceOptionsMessageTypeDef](./type_defs.md#orderabledbinstanceoptionsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeOrderableDBInstanceOptionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Engine: str,
    EngineVersion: str = ...,
    DBInstanceClass: str = ...,
    LicenseModel: str = ...,
    Vpc: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[OrderableDBInstanceOptionsMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: OrderableDBInstanceOptionsMessageTypeDef](./type_defs.md#orderabledbinstanceoptionsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = {  # (1)
    "Engine": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef](./type_defs.md#describeorderabledbinstanceoptionsmessagedescribeorderabledbinstanceoptionspaginatetypedef) 
## DescribePendingMaintenanceActionsPaginator

Type annotations and code completion for `#!python session.client("neptune").get_paginator("describe_pending_maintenance_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribePendingMaintenanceActions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_neptune.paginator import DescribePendingMaintenanceActionsPaginator

session = Session()

session = get_session()
async with session.client("neptune") as client:  # (1)
    paginator: DescribePendingMaintenanceActionsPaginator = client.get_paginator("describe_pending_maintenance_actions")  # (2)
    async for item in paginator.paginate(...):
        item: PendingMaintenanceActionsMessageTypeDef
        print(item)  # (3)
```

1. client: [NeptuneClient](./client.md)
2. paginator: [DescribePendingMaintenanceActionsPaginator](./paginators.md#describependingmaintenanceactionspaginator)
3. item: [:material-code-braces: PendingMaintenanceActionsMessageTypeDef](./type_defs.md#pendingmaintenanceactionsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribePendingMaintenanceActionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[PendingMaintenanceActionsMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: PendingMaintenanceActionsMessageTypeDef](./type_defs.md#pendingmaintenanceactionsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef = {  # (1)
    "ResourceIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef](./type_defs.md#describependingmaintenanceactionsmessagedescribependingmaintenanceactionspaginatetypedef) 
