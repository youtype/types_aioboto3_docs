# Examples

> [Index](../README.md) > [RDS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [RDS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#rds)
    type annotations stubs module [types-aiobotocore-rds](https://pypi.org/project/types-aiobotocore-rds/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[rds]` package installed.

Write your `RDS` code as usual,
type checking and code completion should work out of the box.



```python
# RDSClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("rds") as client:  # (1)
    result = await client.add_role_to_db_cluster()  # (2)
```

1. client: [RDSClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# DescribeBlueGreenDeploymentsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("rds") as client:  # (1)
    paginator = client.get_paginator("describe_blue_green_deployments")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeBlueGreenDeploymentsPaginator](./paginators.md#describebluegreendeploymentspaginator)
3. item: [:material-code-braces: DescribeBlueGreenDeploymentsResponseTypeDef](./type_defs.md#describebluegreendeploymentsresponsetypedef) 



```python
# DBClusterAvailableWaiter usage example

from aioboto3.session import Session


session = Session()

async with session.client("rds") as client:  # (1)
    waiter = client.get_waiter("db_cluster_available")  # (2)
    await waiter.wait()
```

1. client: [RDSClient](./client.md)
2. waiter: [DBClusterAvailableWaiter](./waiters.md#dbclusteravailablewaiter)


### Explicit type annotations

With `types-aioboto3-lite[rds]`
or a standalone `types_aiobotocore_rds` package, you have to explicitly specify
`client: RDSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# RDSClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_rds.client import RDSClient
from types_aiobotocore_rds.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_rds.type_defs import AddRoleToDBClusterMessageRequestTypeDef


session = Session()

client: RDSClient
async with session.client("rds") as client:  # (1)
    kwargs: AddRoleToDBClusterMessageRequestTypeDef = {...}  # (2)
    result: EmptyResponseMetadataTypeDef = await client.add_role_to_db_cluster(**kwargs)  # (3)
```

1. client: [RDSClient](./client.md)
2. kwargs: [:material-code-braces: AddRoleToDBClusterMessageRequestTypeDef](./type_defs.md#addroletodbclustermessagerequesttypedef) 
3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# DescribeBlueGreenDeploymentsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_rds.client import RDSClient
from types_aiobotocore_rds.paginator import DescribeBlueGreenDeploymentsPaginator
from types_aiobotocore_rds.type_defs import DescribeBlueGreenDeploymentsResponseTypeDef


session = Session()

client: RDSClient
async with session.client("rds") as client:  # (1)
    paginator: DescribeBlueGreenDeploymentsPaginator = client.get_paginator("describe_blue_green_deployments")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeBlueGreenDeploymentsResponseTypeDef
        print(item)  # (3)
```

1. client: [RDSClient](./client.md)
2. paginator: [DescribeBlueGreenDeploymentsPaginator](./paginators.md#describebluegreendeploymentspaginator)
3. item: [:material-code-braces: DescribeBlueGreenDeploymentsResponseTypeDef](./type_defs.md#describebluegreendeploymentsresponsetypedef) 



```python
# DBClusterAvailableWaiter usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_rds.client import RDSClient
from types_aiobotocore_rds.waiter import DBClusterAvailableWaiter


session = Session()

async with session.client("rds") as client:  # (1)
    waiter = client.get_waiter("db_cluster_available")  # (2)
    await waiter.wait()
```

1. client: [RDSClient](./client.md)
2. waiter: [DBClusterAvailableWaiter](./waiters.md#dbclusteravailablewaiter)

